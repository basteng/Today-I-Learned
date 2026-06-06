# AS02MC04 FPGA — taxi cndm NIC Bitstream 编译烧录全流程

## 环境说明

| 项目 | 说明 |
|------|------|
| 目标板 | AS02MC04，芯片 XCKU3P-FFVB676-1-E |
| 源码仓库 | github.com/fpganinja/taxi，项目 `cndm` |
| Windows | Vivado ML Standard 2025.2，路径 `D:\AMDDesignTools\2025.2\Vivado` |
| Pi 5 | 用于烧录，通过 OpenOCD + J-Link |
| 源码目录 | `D:\14_Github\taxi\` |

---

## 一、源码准备（Windows）

### 1. 克隆仓库（建议开发者模式 + symlinks）

```bash
# Git Bash，需要开启 Windows 开发者模式
git clone -c core.symlinks=true https://github.com/fpganinja/taxi.git
```

> ⚠️ 如果没有开发者模式，仓库里的符号链接会变成普通文本文件，后续路径处理会很麻烦。

### 2. 在 Pi 上生成 Tcl 文件

taxi 项目需要在 Linux 上用 `make` 展开 `.f` 文件生成 Tcl，Windows 上没有 make。

```bash
# Pi 上
cd ~/github/taxi/src/cndm/board/AS02MC04/fpga/fpga
make create_project.tcl
# 会生成：create_project.tcl, run_synth.tcl, run_impl.tcl, generate_bit.tcl, config.tcl
```

然后 SCP 到 Windows（或用 Git Bash 复制）。

---

## 二、Windows 上的路径问题处理

### 背景

taxi 仓库用符号链接组织 lib 依赖，Linux 上正常，Windows 上 Vivado 无法解析 `..` 叠加的路径，如：

```
../lib/taxi/src/cndm/rtl/../lib/taxi/src/prim/rtl/taxi_ram_2rw_1c.sv
```

### 解决方案：复制源码 + Python 修复 TCL

**Step 1：** 复制 taxi 源码到 lib 目录（Git Bash，用临时目录绕过递归复制限制）

```bash
cd /d/14_Github && mkdir taxi_temp && cd taxi_temp
cp -r /d/14_Github/taxi/src/cndm . && cp -r /d/14_Github/taxi/src/prim .
cp -r /d/14_Github/taxi/src/dma . && cp -r /d/14_Github/taxi/src/eth .
cp -r /d/14_Github/taxi/src/axis . && cp -r /d/14_Github/taxi/src/pcie .
cp -r /d/14_Github/taxi/src/sync . && cp -r /d/14_Github/taxi/src/pyrite .
cp -r /d/14_Github/taxi/src/apb . && cp -r /d/14_Github/taxi/src/lss .
cp -r /d/14_Github/taxi/src/axi . && cp -r /d/14_Github/taxi/src/hip .
cp -r /d/14_Github/taxi/src/lfsr . && cp -r /d/14_Github/taxi/src/stats .
cp -r /d/14_Github/taxi/src/ptp .

rm -rf /d/14_Github/taxi/src/cndm/board/AS02MC04/fpga/lib/taxi
mkdir -p /d/14_Github/taxi/src/cndm/board/AS02MC04/fpga/lib/taxi
mv /d/14_Github/taxi_temp /d/14_Github/taxi/src/cndm/board/AS02MC04/fpga/lib/taxi/src
```

**Step 2：** 用 Python 修复 TCL 里的双重路径（在任意 Python IDE 运行）

```python
import re

tcl_path = r"D:\14_Github\taxi\src\cndm\board\AS02MC04\fpga\fpga\create_project.tcl"
src_base = r"D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/lib/taxi/src"

with open(tcl_path, "r") as f:
    content = f.read()

# 先用 normpath 展开所有 ..
def collapse(path):
    parts = path.replace("\\", "/").split("/")
    stack = []
    for p in parts:
        if p == ".." and stack and stack[-1] != "..":
            stack.pop()
        else:
            stack.append(p)
    return "/".join(stack)

content = re.sub(r'[^\s"]+\.(?:sv|v|tcl|xdc)', lambda m: collapse(m.group(0)), content)

# 再去掉多余的 lib/taxi/src 嵌套
for _ in range(10):
    new_content = re.sub(
        r'(D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/lib/taxi/src)/\w+/lib/taxi/src/(\w)',
        r'\1/\2',
        content
    )
    if new_content == content:
        break
    content = new_content

with open(tcl_path, "w") as f:
    f.write(content)

print("Done")
```

---

## 三、Vivado 编译流程

在 **Vivado Tcl Console** 中执行：

### 1. 创建工程

```tcl
cd D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga
source create_project.tcl
```

### 2. 综合（约 20-30 分钟）

```tcl
source run_synth.tcl
```

或手动：

```tcl
reset_run synth_1
launch_runs -jobs 4 synth_1
wait_on_run synth_1
```

### 3. 实现/布局布线（约 30-90 分钟）

```tcl
reset_run impl_1
launch_runs -jobs 4 impl_1
wait_on_run impl_1
```

> Log 文件位置：`fpga.runs/impl_1/runme.log`

### 4. 生成 Bitstream（约 5-10 分钟）

```tcl
launch_runs impl_1 -to_step write_bitstream -jobs 4
wait_on_run impl_1
```

生成文件：`fpga.runs/impl_1/fpga.bit`

---

## 四、生成 SVF 文件

SVF 用于通过 OpenOCD 烧录，需要借助 Vivado Hardware Manager 虚拟连接生成。

在 Vivado Tcl Console 中：

```tcl
# 先加载 checkpoint
open_checkpoint D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga/fpga.runs/impl_1/fpga_routed.dcp

# 生成 SVF
open_hw_manager
connect_hw_server
create_hw_target alibaba_board_svf_target
open_hw_target
create_hw_device -part xcku3p
set_property PROGRAM.FILE {D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga/fpga.runs/impl_1/fpga.bit} [get_hw_device]
program_hw_device [get_hw_device]
write_hw_svf -force D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga/fpga.svf
close_hw_manager
```

生成文件：`fpga.svf`

---

## 五、传输到 Pi 并烧录

### 传输

```bash
# Git Bash
scp -P 6051 /d/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga/fpga.svf \
    basteng@8.130.93.178:/home/basteng/fpga_bitstreams/AS02MC04/fpga.svf
```

### Pi 上烧录

```bash
openocd -f ~/openocd_xcku3p.cfg \
    -c "svf /home/basteng/fpga_bitstreams/AS02MC04/fpga.svf -progress; exit"
```

---

## 六、关键说明

### JTAG 扫描链

AS02MC04 上只有一个 JTAG 设备，IDCODE = `0x04a63093`（XCKU3P），IR 长度 6 bit。

### 文件路径一览

| 文件 | 路径 |
|------|------|
| TCL 脚本 | `fpga/fpga/create_project.tcl` 等 |
| 综合 checkpoint | `fpga.runs/synth_1/fpga.dcp` |
| 实现 checkpoint | `fpga.runs/impl_1/fpga_routed.dcp` |
| Bitstream | `fpga.runs/impl_1/fpga.bit` |
| SVF | `fpga/fpga/fpga.svf` |

### 下次重建时

如果源码没有变化，直接从 Vivado TCL Console 跑：

```tcl
cd D:/14_Github/taxi/src/cndm/board/AS02MC04/fpga/fpga
open_project fpga.xpr
reset_run synth_1
launch_runs -jobs 4 synth_1
wait_on_run synth_1
reset_run impl_1
launch_runs -jobs 4 impl_1
wait_on_run impl_1
launch_runs impl_1 -to_step write_bitstream -jobs 4
wait_on_run impl_1
```

然后按第四步生成 SVF。

---

## 参考资料

- [AS02MC04 详细介绍（含 JTAG/pinout）](https://essenceia.github.io/projects/alibaba_cloud_fpga/)
- [taxi 项目 AS02MC04 板级支持](https://github.com/fpganinja/taxi/tree/master/src/cndm/board/AS02MC04)
- Xilinx UG570 UltraScale Architecture Configuration User Guide

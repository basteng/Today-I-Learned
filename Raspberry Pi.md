- [1. 使用 Raspberry Pi Pico 制作任意波发生器](#1-使用-raspberry-pi-pico-制作任意波发生器)
- [2.Raspberry Pi Pico 2 上的实时 ML 音频噪声抑制](#2raspberry-pi-pico-2-上的实时-ml-音频噪声抑制)
- [3.使用 Raspberry Pi Pico 创建 USB 麦克风](#3使用-raspberry-pi-pico-创建-usb-麦克风)
- [4.Google Pigweed 登陆我们全新的 RP2350](#4google-pigweed-登陆我们全新的-rp2350)
- [5. Pico 2 文档](#5-pico-2-文档)
- [6. Raspberry Pi Pico W 初学者课程](#6-raspberry-pi-pico-w-初学者课程)
- [7. 如何构建 Raspberry Pi 集群](#7-如何构建-raspberry-pi-集群)
  - [7.1 官方教程](#71-官方教程)
  - [7.2 Raspberry Pi 3B 构建集群教程](#72-raspberry-pi-3b-构建集群教程)
  - [7.3 ClusterHat 教程 Pi Zero W](#73-clusterhat-教程-pi-zero-w)
- [8. Raspberry Pi Pico 2 构筑自己的音序器](#8-raspberry-pi-pico-2-构筑自己的音序器)
- [9. Raspberry运行Deepseek 200 token/s](#9-raspberry运行deepseek-200-tokens)
- [9. FPGA](#9-fpga)
  - [❌ 报错信息分析](#-报错信息分析)
  - [✅ 解决方法（3 步）](#-解决方法3-步)
    - [**① 初始化 Git 子模块**](#-初始化-git-子模块)
    - [**② 然后重新编译**](#-然后重新编译)
    - [**③ 安装 Yosys（可选）**](#-安装-yosys可选)
  - [🧪 验证是否成功](#-验证是否成功)
  - [✅ 总结](#-总结)
    - [✅ 解释：](#-解释)
  - [✅ 解决方法：](#-解决方法)
    - [**方法 1：重试几次**](#方法-1重试几次)
    - [**方法 2：切换使用 SSH 拉取**](#方法-2切换使用-ssh-拉取)
    - [**方法 3：使用代理或 VPN**](#方法-3使用代理或-vpn)
    - [**方法 4：手动克隆子模块**](#方法-4手动克隆子模块)
  - [✅ 总结](#-总结-1)
  - [🔍 根本原因](#-根本原因)
  - [✅ 解决步骤](#-解决步骤)
    - [🔁 **步骤 1：确认子模块状态**](#-步骤-1确认子模块状态)
    - [🔧 **步骤 2：重新拉取子模块（推荐使用手动克隆）**](#-步骤-2重新拉取子模块推荐使用手动克隆)
      - [✅ 方法 1：逐个手动克隆](#-方法-1逐个手动克隆)
      - [✅ 方法 2：如果网络稳定了，也可以重新尝试自动拉取](#-方法-2如果网络稳定了也可以重新尝试自动拉取)
    - [✅ 步骤 3：编译验证](#-步骤-3编译验证)
    - [🔚 总结](#-总结-2)
    - [✅ 解决方案：单独拉取 `libs/cxxopts` 子模块](#-解决方案单独拉取-libscxxopts-子模块)
    - [💡 如果仍失败（网络不稳），可以手动拉取](#-如果仍失败网络不稳可以手动拉取)
    - [✅ 然后重新编译](#-然后重新编译-1)
  - [✅ 正确的构建方式如下（请严格照做）：](#-正确的构建方式如下请严格照做)
    - [步骤 1：新建构建目录并进入](#步骤-1新建构建目录并进入)
    - [步骤 2：配置 CMake（仍然在 `build` 目录中）](#步骤-2配置-cmake仍然在-build-目录中)
    - [步骤 3：编译并安装](#步骤-3编译并安装)
    - [✅ 正确做法是：**从 nextpnr 根目录外的 `build` 子目录中调用 `cmake` 并指定 `..` 为源码路径**](#-正确做法是从-nextpnr-根目录外的-build-子目录中调用-cmake-并指定--为源码路径)
    - [总结](#总结)
    - [✅ 解决方法如下：](#-解决方法如下)
      - [第一步：**清除源码目录中的缓存文件**](#第一步清除源码目录中的缓存文件)
      - [第二步：**重新创建 build 目录并配置编译**](#第二步重新创建-build-目录并配置编译)
- [10. 树莓派4B bookworm设置成热点](#10-树莓派4b-bookworm设置成热点)
  - [📌 为何 `RPI4B-basteng` 没变成热点，反而被当作 Wi-Fi 去连接？](#-为何-rpi4b-basteng-没变成热点反而被当作-wi-fi-去连接)
    - [🔍 原因可能有以下几种：](#-原因可能有以下几种)
  - [✅ 解决方法：彻底清掉错误配置，重新用命令方式创建热点](#-解决方法彻底清掉错误配置重新用命令方式创建热点)
    - [🧹 步骤 1：删除错误连接配置](#-步骤-1删除错误连接配置)
    - [🚀 步骤 2：创建正确的热点（AP）连接](#-步骤-2创建正确的热点ap连接)
    - [✅ 验证成功](#-验证成功)
  - [💡 总结一句话：](#-总结一句话)
- [11. 树莓派翻墙自动配置](#11-树莓派翻墙自动配置)
  - [✅ 脚本用途说明](#-脚本用途说明)
  - [📜 脚本内容（文件名建议为：`setup-hotspot-proxy.sh`）](#-脚本内容文件名建议为setup-hotspot-proxysh)
  - [🔧 使用说明](#-使用说明)
  - [📌 注意事项](#-注意事项)
  - [如果原有服务器失效，操作如下](#如果原有服务器失效操作如下)
- [12. RPi USB Wi-Fi 适配器](#12-rpi-usb-wi-fi-适配器)
- [13. 树莓派5运行claude，现在使用claude-start即可](#13-树莓派5运行claude现在使用claude-start即可)
  - [正常情况下：](#正常情况下)
  - [但可能需要的情况：](#但可能需要的情况)
  - [我建议创建一个别名：](#我建议创建一个别名)
  - [或者更简单，创建软链接：](#或者更简单创建软链接)
- [14. 需要使用grafcp才能在树莓派上运行claude](#14-需要使用grafcp才能在树莓派上运行claude)
  - [创建一个便捷的启动脚本：](#创建一个便捷的启动脚本)
- [15. 树莓派科学上网修改IP](#15-树莓派科学上网修改ip)
    - [1. **编辑配置文件**](#1-编辑配置文件)
    - [2. **修改服务器 IP 地址**](#2-修改服务器-ip-地址)
    - [3. **保存并退出**](#3-保存并退出)
    - [4.找出之前占用1080端口的PID，并且kill](#4找出之前占用1080端口的pid并且kill)
- [找出占用1080端口的进程](#找出占用1080端口的进程)
- [停止该进程（假设PID是12345）](#停止该进程假设pid是12345)
    - [5. **重启 Shadowsocks 服务**](#5-重启-shadowsocks-服务)
    - [6. **检查服务状态**](#6-检查服务状态)
    - [7. **测试翻墙是否正常**](#7-测试翻墙是否正常)
    - [总结：](#总结-1)
- [16. 树莓派透明代理设置](#16-树莓派透明代理设置)
  - [解决方案](#解决方案)
    - [1. 修正绑定参数](#1-修正绑定参数)
    - [2. 检查配置文件](#2-检查配置文件)
    - [3. 检查端口占用](#3-检查端口占用)
    - [4. 测试网络连接](#4-测试网络连接)
    - [5. 推荐的启动命令](#5-推荐的启动命令)
    - [6. 更新加密方法](#6-更新加密方法)
    - [2. 重启服务](#2-重启服务)
    - [3. 验证监听地址](#3-验证监听地址)
    - [4. 配置 iptables 透明代理规则](#4-配置-iptables-透明代理规则)
    - [5. 启用 IP 转发](#5-启用-ip-转发)
    - [6. 验证配置](#6-验证配置)
  - [当前配置状态检查](#当前配置状态检查)
    - [1. 检查 ss-redir 配置](#1-检查-ss-redir-配置)
    - [2. 启用 IP 转发](#2-启用-ip-转发)
    - [3. 测试透明代理](#3-测试透明代理)
    - [4. 如果不工作，检查日志](#4-如果不工作检查日志)
    - [5. 保存 iptables 规则（重要）](#5-保存-iptables-规则重要)
  - [解决方法](#解决方法)
    - [方法1: 使用 tee 命令](#方法1-使用-tee-命令)
    - [方法2: 先创建目录](#方法2-先创建目录)
    - [方法3: 使用 iptables-persistent 包](#方法3-使用-iptables-persistent-包)
    - [方法4: 手动创建启动脚本](#方法4-手动创建启动脚本)

<div STYLE="page-break-after: always;"></div>

# 1. 使用 Raspberry Pi Pico 制作任意波发生器
一个很有意思的使用pico制作任意波形发生器的项目，主要需要材料如下：
- Raspberry pi pico microcontroller with male pin headers
- 1 5x7cm prototype board
- 2 20-pin female pin headers
- 23 resistors of identical value, near 2kOhm
相关示意图
![](/picture/F3WUUI0KKY0JSMW.webp)
![](/picture/F6Z9RB0KKY0JU0D.webp)
![](/picture/F8RIICRKKY0JU0B.webp)
![](/picture/FUH1QK9KKY0JU0A.webp)
![](/picture/FYYDWX2KKY0JSLL.webp)
代码包括
- DMA 的配置
- PIO 的配置和编程
- 用波形填充数组
- 启动 DMA。

此时波形已生成，pico 的 CPU 可自由执行其他任务。总线上会有数据通信，但 pico 具有高度并行的总线结构，我预计不会出现明显的速度减慢。

<https://www.instructables.com/Arbitrary-Wave-Generator-With-the-Raspberry-Pi-Pic/>

# 2.Raspberry Pi Pico 2 上的实时 ML 音频噪声抑制

Sandeep Mistry 是我们 Arm 朋友的首席软件工程师，他向我们介绍了一种巧妙的方法，将音频噪声抑制应用于我们全新的 Raspberry Pi Pico 2 上的麦克风输入。

机器学习 (ML) 技术彻底改变了许多软件应用程序的开发方式。应用程序开发人员现在会为所需系统整理包含大量示例输入和输出的数据集，然后使用这些数据集来训练 ML 模型。在训练期间，ML 模型会从输入和输出中学习模式。然后，将训练好的模型部署到设备上，这些设备会对来自现实世界的输入进行推理，并使用 ML 模型的预测输出来执行一项或多项操作。

需要数千字节内存的小型机器学习模型可以部署到基于微控制器的设备中，例如新Pico 2开发板中使用的基于Arm Cortex-M33的 Raspberry Pi RP2350 微控制器。将机器学习模型部署到微控制器可降低系统的延迟，因为数据是在靠近输入数据源的设备上处理的。

本博客将深入探讨如何将现有的基于 ML 的音频噪声抑制算法部署到新 Pico 2 板中使用的Raspberry Pi RP2350 微控制器中。RP2350 的双核 Arm Cortex-M33 CPU 使应用程序开发人员能够部署更多计算密集型应用程序，这些应用程序的性能超过了原始 Raspberry Pi Pico 板中使用的 RP2040 微控制器的性能。

然后，该算法将集成到我为原始 Pico 板开发的 USB 麦克风应用程序中。原始应用程序从数字脉冲密度调制 (PDM) 麦克风捕获数据，并将其处理为与 USB 音频标准兼容的格式，以便通过 USB 传输。

算法背景
2018 年，Jean-Marc Valin 发表了一篇论文，题为《一种用于实时全频带语音增强的混合 DSP/深度学习方法》。该​​论文介绍了如何使用基于循环神经网络 (RNN) 的 ML 模型来抑制音频源中的噪声。如果您有兴趣了解有关该算法的更多信息，请阅读 Jean-Marc 的RNNoise：学习噪声抑制页面。该页面介绍了该算法的细节，并包含交互式示例。该项目的源代码可在RNNoise Git 存储库中找到。

从高层次上讲，该算法通过将信号分成 22 个频带，从 48 kHz 音频源的 10 毫秒中提取 42 个特征。

然后将这 42 个特征用作神经网络的输入，该神经网络计算 22 个频带的增益。然后可以将计算出的增益应用于原始音频信号以产生去噪版本。神经网络还输出“语音活动检测”输出，该输出表示语音在输入信号中存在的预测置信度，值介于 0 和 1 之间。

移植和基准测试算法
RNNoise 项目的原始 C 代码可以集成到使用 Raspberry Pi Pico SDK的CMake项目中。移植的所有源代码都可以在GitHub 上的rnnoise-examples-for-pico-2存储库中找到。使用 RNNoise 项目 v0.1.1 中的、、、、和文件创建了一个新的 CMake 库目标。celt_lpc.cdenoise.ckiss_fft.cpitch.crnn.crnn_data.c

对双二阶函数中的单精度浮点计算进行了一些小修改denoise.c，以及使用log10f(…)和sqrtf(…)代替log10(…)和sqrt(…)函数。

然后，可以将该库集成到基准测试应用程序中，该应用程序调用该函数来初始化模型，然后测量该函数处理 480 个样本所需的rrnoise_create(…)时间。rnnoise_process_frame(…)

该基准测试应用程序可以部署到 Raspberry Pi Pico 1 或 Pico 2 开发板上，首先按照“Raspberry Pi Pico 入门” C/C++ SDK 指南的第 2 节和第 9 节进行操作，然后运行以下命令来构建 .uf2 应用程序以部署到开发板上：

git clone --recurse-submodules \ https://github.com/ArmDeveloperEcosystem/rnnoise-examples-for-pico-2.git
cd rnnoise-examples-for-pico-2
mkdir build
cmake .. -DPICO_BOARD=pico2
make rnnoise-benchmark

编译后，examples/benchmark/rnnoise-benchmark.uf2可以通过按住电路板的白色 BOOTSEL 按钮，同时将 USB 电缆插入计算机并将 .uf2 文件复制到 Pico 的 USB 磁盘，将文件部署到电路板。

以下是 Pico 1 和 Pico 2 板上的基准测试结果：

原始 Pico 1 大约需要 372.6 毫秒，而新 Pico 2 则需要 22.1 毫秒：两个板之间的速度提高了 16.87 倍。

修改 16 kHz 音频的算法
对于以 48 kHz 采样率处理 480 个音频样本的开发板来说，完成该功能所需的时间必须少于 0.01 秒 (480 / 48,000) 或 10 毫秒rnnoise_process_frame(…)。我们对 Pico 2 的基准测试结果需要 22.1 毫秒，对于 48 kHz 音频来说速度不够快，但对于以 16 kHz 采样率处理音频来说速度足够快，需要在 30 毫秒内处理音频。

可以轻松修改变量eband5ms​​ indenoise.c以调整处理 16 kHz 数据的算法。此变量控制 22 个频带中使用的起始范围。可以通过将原始值乘以 3 来调整它，因为 16 kHz 音频收集样本的时间是 48 kHz 音频的 3 倍，并将最大起始位置设置为 120。

这是原始值：

static const opus_int16 eband5ms[] = {
/*0  200 400 600 800  1k 1.2 1.4 1.6  2k 2.4 2.8 3.2  4k 4.8 5.6 6.8  8k 9.6 12k 15.6 20k*/
0,  1,  2,  3,  4,  5,  6,  7,  8, 10, 12, 14, 16, 20, 24, 28, 34, 40, 48, 60, 78, 100
};

与 16 kHz 音频一起使用的修改值：

static const opus_int16 eband5ms[] = {
/*0  200 400 600 800  1k 1.2 1.4 1.6  2k 2.4 2.8 3.2  4k 4.8 5.6 6.8  8k 9.6 12k 15.6 20k*/
0,  3,  6,  9,  12, 15, 18, 21, 24, 60, 36, 42, 48, 60, 72, 84, 102, 120, 120, 120, 120, 120
};

可以编译串行示例并将其部署到板上以测试修改后的算法。此示例不断循环通过 USB 接收 480 个 16 位音频样本，使用去噪算法对其进行处理，然后通过 USB 传输去噪后的样本。在 PC 上，可以使用serial_denoise.py Python 脚本从文件发送原始 16 位、16 kHz 音频，并将去噪后的音频保存到文件中。

这些原始值可以导入到Audacity等应用程序中进行可视化和回放。以下是示例：第一条音轨是原始音频（有噪音），其下方的第二条音轨是在 Pico 2 上去噪的版本。

我选择了一个噪音明显减少的区域。到目前为止一切顺利；该算法已通过验证，可以在主板上运行，并使用通过 USB 从 PC 流式传输的 16 kHz 音频源！

将算法集成到 USB 麦克风应用程序中
最初为 Pico 1 构建的 USB 麦克风应用程序现在可以通过板载去噪功能进行增强。

硬件
此应用程序需要以下硬件：

Raspberry Pi Pico 2开发板
Adafruit PDM MEMS 麦克风分线板
半尺寸面包板
跳线
（可选）滑动开关
（可选）触觉按钮
可选的滑动开关将用作在运行时禁用或启用噪声抑制处理的切换开关，而可选的触觉开关将提供一种方便的方法来重置电路板。

硬件连接如下：

软件
应用程序将使用microphone-library-for-pico以 16 kHz 的采样率从 PDM 麦克风收集 480 个 16 位样本。该库将 RP2350 的可编程 I/O (PIO) 和直接内存访问 (DMA) 功能与OpenPDM2PCM库相结合，将原始 PDM 数据转换为脉冲编码调制 (PCM) 格式。16 位 PCM 数据转换为 32 位浮点，并使用 RNNoise 算法进行去噪。此后，去噪后的帧将转换为 16 位整数，并使用TinyUSB库通过 USB 发送。USB 传输将每 1 毫秒发送 16 个去噪样本。

此应用使用了 RP2350 的两个 Cortex-M33 内核。内核 1 从 PDM 麦克风捕获原始数据，并对其进行过滤和去噪。内核 0 使用 TinyUSB 库和 RP2350 的 USB 接口通过 USB 传输去噪数据。

RNNoise 模型的语音活动检测输出将通过脉冲宽度调制 (PWM) 显示在 Pico 2 的内置 LED 上。当 VAD 输出接近 1.0 时，LED 将变亮，而当接近 0.0 时，LED 将熄灭。


该应用程序的源代码可以在rnnoise-examples-for-pico-2 GitHub 存储库的 examples/usb_pdm_microphone 文件夹中找到。该应用程序可以以与基准测试应用程序类似的方式进行编译，使用以下make命令：

make rnnoise_usb_pdm_microphone

编译完成后，examples/usb_pdm_microphone/rnnoise_usb_pdm_microphone.uf2按住 BOOTSEL 按钮并重置此板后，即可将文件复制到 Pico 2 的 USB 磁盘。

测试
一旦应用程序加载到主板上，您就可以使用 Audacity 测试录制音频，方法是先单击“音频设置”按钮-> “重新扫描音频设备”，然后单击“音频设置”按钮-> “录音设备”->“ MicNode”，然后单击“录制”按钮。

如果您连接了可选的滑动开关，则可以通过将开关滑向 Pico 2 的 USB 连接器来禁用噪声抑制，并通过将开关滑离 USB 连接器来重新启用噪声抑制。

下面录制的演示视频使用 Pico 2 作为 USB 麦克风，首先关闭噪音抑制，然后启用噪音抑制，输入相同。查看并听取噪音抑制算法的结果！

后续步骤Next steps
本博客演示了如何使用 Raspberry Pi Pico 2 的 Arm Cortex-M33 CPU 的额外计算能力，通过 ML 模型对从 16 kHz 的 PDM 麦克风捕获的实时 16 位音频数据进行降噪。降噪算法利用了 Cortex-M33 的浮点单元 (FPU)，运行速度比原始 Pico 板上的 Cortex-M0+ 快 16.87 倍。该应用程序利用一个 CPU 来捕获、过滤和降噪数据，另一个 CPU 通过 USB 将音频数据传输到 PC。

下一步，您可以修改应用程序，在降噪数据通过 USB 发送到 PC 之前添加自动增益控制 (AGC)。或者，降噪数据可以直接在板上使用，作为另一个数字信号处理 (DSP) 算法的输入，或在 Core 0 而不是 USB 堆栈上运行的 ML 模型。

<https://www.raspberrypi.com/news/real-time-ml-audio-noise-suppression-on-raspberry-pi-pico-2/>

# 3.使用 Raspberry Pi Pico 创建 USB 麦克风

本指南将引导您使用 RP2040 的 PIO、DMA 和 USB 功能在 Raspberry Pi Pico 上创建 USB 麦克风。

介绍
本指南将介绍如何使用Raspberry Pi Pico开发板和外部数字麦克风创建自己的 USB 麦克风设备。该项目将利用开发板RP2040微控制器 (MCU)的编程 I/O (PIO)、直接内存访问 (DMA) 和通用串行总线 (USB) 功能。

USB
USB 是一种非常流行的标准，于 1996 年发布，适用于有线计算机外围设备，例如键盘、鼠标、打印机、扫描仪和麦克风。

Raspberry Pi Pico板的RP2040 MCU具有“USB 1.1 主机/设备”功能，可让您连接到现有的 USB 外围设备（主机模式）或创建自己的 USB 外围设备（设备模式）。Raspberry Pi Pico SDK使用TinyUSB 库作为其 USB 软件堆栈。

Tiny USB 库是“用于嵌入式系统的开源跨平台 USB 堆栈” ，支持多种类型的 MCU，包括 Raspberry Pi RP2040。并且支持设备和主机模式。我们可以使用它内置的 USB 音频类支持将我们的 Pico 转换为 USB 麦克风设备。

选择麦克风
RP2040 MCU 具有内置 4 通道模数转换器 (ADC) 功能，具有 12 位精度，可用于从外部模拟麦克风收集音频，但我们发现模拟麦克风的音频质量包含很多噪音，因此将改用数字麦克风。

数字麦克风常见的接口有两种：

脉冲密度调制（PDM）
IC 间声音(I2S)
虽然 RP2040 不具备对这两种接口类型的内置支持，但超灵活的可编程 I/O (PIO) 功能可用于在软件中创建我们自己的 PDM 或 I2S 外设接口。我将在一个引脚上向麦克风生成输出时钟信号，并使用另一个引脚从麦克风接收数据。在本指南中，我们将使用 Adafruit PDM MEMS 麦克风分线板。

PDM 如何工作？
当 PDM 麦克风接收到时钟信号时，它会根据从麦克风捕获的模拟音频值输出 0 或 1 信号。要以每秒 16,000 个样本（16 kHz）的速度捕获音频，PDM 麦克风的时钟输入必须以 1.024 MHz = 64 x 16kHz 驱动，然后可以对 PDM 的麦克风数据信号进行过滤和下采样。对于每个样本，64 个值的 0 或 1 输出被平均，从而为样本创建一个介于 -32678 和 32767 之间的 16 位值。

您可以使用逻辑分析仪（例如Saleae）来查看 PDM CLK 和 DAT 信号。

处理管道
系统将执行以下操作：

1. 使用 PIO 生成 1.024 MHz 时钟信号送入 PDM 麦克风。

2. 使用 PIO 每个时钟周期从 PDM 麦克风捕获一次数字值。

3. DMA 将配置为捕获 1 毫秒的音频，采样率为 16 kHz，每毫秒生成 16 个样本。16 个样本将包含 64 x 16 = 1024 位。

4. 一旦收到 16 个样本的原始 PDM 数据，它将使用OpenPDM2PCM库对 1024 位原始 PDM 数据进行过滤和下采样为 16 个脉冲编码调制(PCM) 16 位音频样本。

5. 通过 USB 将 16 个 PCM 音频样本发送至 PC。

概述
事物
故事
介绍
USB
选择麦克风
PDM 如何工作
处理管道
硬件设置
设置 Pico SDK 开发环境
获取并编译微型麦克风库和示例
录制音频数据
结论
其他 Raspberry Pi RP2040 资源
示意图
代码
致谢
评论(35)

四十八

桑迪普·米斯特里
桑迪普·米斯特里
2021 年 5 月 20 日 发布© CC BY
使用 Raspberry Pi Pico 创建 USB 麦克风 🎤
本指南将引导您使用 RP2040 的 PIO、DMA 和 USB 功能在 Raspberry Pi Pico 上创建 USB 麦克风。

中间的
提供完整说明
30 分钟
49,580
使用 Raspberry Pi Pico 创建 USB 麦克风 🎤
这个项目中使用的东西
硬件组件
树莓派 Pico	
树莓派 Pico
×	1	
Adafruit PDM MEMS 麦克风分线板
×	1	
面包板（通用）	
面包板（通用）
×	1	
跳线（通用）	
跳线（通用）
×	1	
故事
本指南由Arm 软件开发人员团队创建，请在 Twitter 上关注我们：@ArmSoftwareDev和 YouTube：Arm 软件开发人员，获取更多资源！

介绍
本指南将介绍如何使用Raspberry Pi Pico开发板和外部数字麦克风创建自己的 USB 麦克风设备。该项目将利用开发板RP2040微控制器 (MCU)的编程 I/O (PIO)、直接内存访问 (DMA) 和通用串行总线 (USB) 功能。

USB
USB 是一种非常流行的标准，于 1996 年发布，适用于有线计算机外围设备，例如键盘、鼠标、打印机、扫描仪和麦克风。

Raspberry Pi Pico板的RP2040 MCU具有“USB 1.1 主机/设备”功能，可让您连接到现有的 USB 外围设备（主机模式）或创建自己的 USB 外围设备（设备模式）。Raspberry Pi Pico SDK使用TinyUSB 库作为其 USB 软件堆栈。

Tiny USB 库是“用于嵌入式系统的开源跨平台 USB 堆栈” ，支持多种类型的 MCU，包括 Raspberry Pi RP2040。并且支持设备和主机模式。我们可以使用它内置的 USB 音频类支持将我们的 Pico 转换为 USB 麦克风设备。

选择麦克风
RP2040 MCU 具有内置 4 通道模数转换器 (ADC) 功能，具有 12 位精度，可用于从外部模拟麦克风收集音频，但我们发现模拟麦克风的音频质量包含很多噪音，因此将改用数字麦克风。

数字麦克风常见的接口有两种：

脉冲密度调制（PDM）
IC 间声音(I2S)
虽然 RP2040 不具备对这两种接口类型的内置支持，但超灵活的可编程 I/O (PIO) 功能可用于在软件中创建我们自己的 PDM 或 I2S 外设接口。我将在一个引脚上向麦克风生成输出时钟信号，并使用另一个引脚从麦克风接收数据。在本指南中，我们将使用 Adafruit PDM MEMS 麦克风分线板。

PDM 如何工作？
当 PDM 麦克风接收到时钟信号时，它会根据从麦克风捕获的模拟音频值输出 0 或 1 信号。要以每秒 16,000 个样本（16 kHz）的速度捕获音频，PDM 麦克风的时钟输入必须以 1.024 MHz = 64 x 16kHz 驱动，然后可以对 PDM 的麦克风数据信号进行过滤和下采样。对于每个样本，64 个值的 0 或 1 输出被平均，从而为样本创建一个介于 -32678 和 32767 之间的 16 位值。

您可以使用逻辑分析仪（例如Saleae）来查看 PDM CLK 和 DAT 信号。

处理管道
系统将执行以下操作：

1. 使用 PIO 生成 1.024 MHz 时钟信号送入 PDM 麦克风。

2. 使用 PIO 每个时钟周期从 PDM 麦克风捕获一次数字值。

3. DMA 将配置为捕获 1 毫秒的音频，采样率为 16 kHz，每毫秒生成 16 个样本。16 个样本将包含 64 x 16 = 1024 位。

4. 一旦收到 16 个样本的原始 PDM 数据，它将使用OpenPDM2PCM库对 1024 位原始 PDM 数据进行过滤和下采样为 16 个脉冲编码调制(PCM) 16 位音频样本。

5. 通过 USB 将 16 个 PCM 音频样本发送至 PC。

硬件设置
将公头焊接到 Raspberry Pi Pico 板和Adafruit PDM MEMS 麦克风分线板上，以便将它们插入面包板。有关将针头焊接到 Raspberry Pi Pico 板的更多详细信息，请参阅 MagPi 的“如何将 GPIO 针头焊接到 Raspberry Pi Pico”指南。

将两个部件焊接好后，将它们放在面包板上，并按如下方式设置接线：

+---------+-------------------+
| PDM Mic | Raspberry Pi Pico |
|---------+-------------------|
|    3V   |        3V3        |
|---------+-------------------|
|    GND  |        GND        |
|---------+-------------------|
|    SEL  |        GND        |
|---------+-------------------|
|    DAT  |       GPIO2       |
|---------+-------------------|
|    CLK  |       GPIO3       |
+---------+-------------------+

注意：将 PDM Mic. SEL 连接至 GND 将导致其在时钟信号下降（从逻辑电平 1 变为 0）后输出新数据。


概述
事物
故事
介绍
USB
选择麦克风
PDM 如何工作
处理管道
硬件设置
设置 Pico SDK 开发环境
获取并编译微型麦克风库和示例
录制音频数据
结论
其他 Raspberry Pi RP2040 资源
示意图
代码
致谢
评论(35)

四十八

桑迪普·米斯特里
桑迪普·米斯特里
2021 年 5 月 20 日 发布© CC BY
使用 Raspberry Pi Pico 创建 USB 麦克风 🎤
本指南将引导您使用 RP2040 的 PIO、DMA 和 USB 功能在 Raspberry Pi Pico 上创建 USB 麦克风。

中间的
提供完整说明
30 分钟
49,580
使用 Raspberry Pi Pico 创建 USB 麦克风 🎤
这个项目中使用的东西
硬件组件
树莓派 Pico	
树莓派 Pico
×	1	
Adafruit PDM MEMS 麦克风分线板
×	1	
面包板（通用）	
面包板（通用）
×	1	
跳线（通用）	
跳线（通用）
×	1	
故事
本指南由Arm 软件开发人员团队创建，请在 Twitter 上关注我们：@ArmSoftwareDev和 YouTube：Arm 软件开发人员，获取更多资源！

介绍
本指南将介绍如何使用Raspberry Pi Pico开发板和外部数字麦克风创建自己的 USB 麦克风设备。该项目将利用开发板RP2040微控制器 (MCU)的编程 I/O (PIO)、直接内存访问 (DMA) 和通用串行总线 (USB) 功能。

USB
USB 是一种非常流行的标准，于 1996 年发布，适用于有线计算机外围设备，例如键盘、鼠标、打印机、扫描仪和麦克风。

Raspberry Pi Pico板的RP2040 MCU具有“USB 1.1 主机/设备”功能，可让您连接到现有的 USB 外围设备（主机模式）或创建自己的 USB 外围设备（设备模式）。Raspberry Pi Pico SDK使用TinyUSB 库作为其 USB 软件堆栈。

Tiny USB 库是“用于嵌入式系统的开源跨平台 USB 堆栈” ，支持多种类型的 MCU，包括 Raspberry Pi RP2040。并且支持设备和主机模式。我们可以使用它内置的 USB 音频类支持将我们的 Pico 转换为 USB 麦克风设备。

选择麦克风
RP2040 MCU 具有内置 4 通道模数转换器 (ADC) 功能，具有 12 位精度，可用于从外部模拟麦克风收集音频，但我们发现模拟麦克风的音频质量包含很多噪音，因此将改用数字麦克风。

数字麦克风常见的接口有两种：

脉冲密度调制（PDM）
IC 间声音(I2S)
虽然 RP2040 不具备对这两种接口类型的内置支持，但超灵活的可编程 I/O (PIO) 功能可用于在软件中创建我们自己的 PDM 或 I2S 外设接口。我将在一个引脚上向麦克风生成输出时钟信号，并使用另一个引脚从麦克风接收数据。在本指南中，我们将使用 Adafruit PDM MEMS 麦克风分线板。

PDM 如何工作？
当 PDM 麦克风接收到时钟信号时，它会根据从麦克风捕获的模拟音频值输出 0 或 1 信号。要以每秒 16,000 个样本（16 kHz）的速度捕获音频，PDM 麦克风的时钟输入必须以 1.024 MHz = 64 x 16kHz 驱动，然后可以对 PDM 的麦克风数据信号进行过滤和下采样。对于每个样本，64 个值的 0 或 1 输出被平均，从而为样本创建一个介于 -32678 和 32767 之间的 16 位值。

您可以使用逻辑分析仪（例如Saleae）来查看 PDM CLK 和 DAT 信号。

处理管道
系统将执行以下操作：

1. 使用 PIO 生成 1.024 MHz 时钟信号送入 PDM 麦克风。

2. 使用 PIO 每个时钟周期从 PDM 麦克风捕获一次数字值。

3. DMA 将配置为捕获 1 毫秒的音频，采样率为 16 kHz，每毫秒生成 16 个样本。16 个样本将包含 64 x 16 = 1024 位。

4. 一旦收到 16 个样本的原始 PDM 数据，它将使用OpenPDM2PCM库对 1024 位原始 PDM 数据进行过滤和下采样为 16 个脉冲编码调制(PCM) 16 位音频样本。

5. 通过 USB 将 16 个 PCM 音频样本发送至 PC。

硬件设置
将公头焊接到 Raspberry Pi Pico 板和Adafruit PDM MEMS 麦克风分线板上，以便将它们插入面包板。有关将针头焊接到 Raspberry Pi Pico 板的更多详细信息，请参阅 MagPi 的“如何将 GPIO 针头焊接到 Raspberry Pi Pico”指南。

将两个部件焊接好后，将它们放在面包板上，并按如下方式设置接线：

+---------+-------------------+
| PDM Mic | Raspberry Pi Pico |
|---------+-------------------|
|    3V   |        3V3        |
|---------+-------------------|
|    GND  |        GND        |
|---------+-------------------|
|    SEL  |        GND        |
|---------+-------------------|
|    DAT  |       GPIO2       |
|---------+-------------------|
|    CLK  |       GPIO3       |
+---------+-------------------+
注意：将 PDM Mic. SEL 连接至 GND 将导致其在时钟信号下降（从逻辑电平 1 变为 0）后输出新数据。

设置 Pico SDK 开发环境
您首先需要使用 Raspberry Pi 的 Pico SDK 和所需的工具链设置您的计算机。

请参阅“ Raspberry Pi Pico 入门”了解更多信息。

该指南的2.1部分可用于所有操作系统，后面是具体操作部分：

Linux：第 2.2 节
macOS：第 9.1 节
Windows：第 9.2 节
获取并编译微型麦克风库和示例
确保PICO_SDK环境变量已设置。

export PICO_SDK_PATH=/path/to/pico-sdk
在终端窗口中，克隆 git 存储库并更改目录：

cd ~/ 

git clone https://github.com/sandeepmistry/pico-microphone.git


cd pico-microphone
创建一个构建目录并将目录更改为该目录：

mkdir build

cd build
运行cmake并make进行编译：

cmake .. -DPICO_BOARD=pico

make
按住开发板上的BOOTSEL按钮，同时使用 USB 线将开发板插入计算机。

将examples/usb_microphone/usb_microphone.uf2文件复制到已安装的 Raspberry Pi Pico 启动 ROM 磁盘：

cp -a examples/usb_microphone/usb_microphone.uf2 /Volumes/RPI-RP2/.
您应该会看到一个名为“ MicNode ”的新麦克风设备连接到您的系统：

录制音频数据
现在我们已将 Raspberry Pi Pico 开发板配置为 USB 麦克风，任何桌面录音应用程序（例如Audacity）都可用于通过 USB 从设备捕获数据。

在您的计算机上下载并安装 Audacity 。

安装完成后打开应用程序，并选择“ MicNode ”设备作为输入。

单击“录制”⏺ 按钮开始为 Raspberry Pi Pico 录制音频。按“停止”⏹ 按钮停止录制音频。

结论
我们使用 Raspberry Pi Pico 开发板和外部 PDM 麦克风创建了自己的 USB 麦克风。该项目使用了 Raspberry Pi RP2040 的 PIO、DMA 和 USB 硬件功能，以及 RP2040 的 Arm Cortex-M0+ 处理器之一上的 OpenPDM2PCM 和 TinyUSB 软件库。

我们的 USB 麦克风从 PDM 麦克风捕获 PDM 音频数据，将 PDM 数据转换为 PCM 格式，然后通过 USB 将 PCM 数据实时发送到 PC！由于 USB 音频标准用于 Raspberry Pi Pico 板和 PC 之间的通信，因此 PC 端不需要自定义软件。

虽然本指南通过 USB 将音频数据从 Raspberry Pi Pico 传输到 PC，但您也可以将pico-microphone库与模拟或 PDM 麦克风一起使用，并在设备上执行数字信号处理 (DSP)，以在没有 PC 的情况下对主板的音频环境做出反应。

<https://www.hackster.io/sandeep-mistry/create-a-usb-microphone-with-the-raspberry-pi-pico-cc9bd5>

# 4.Google Pigweed 登陆我们全新的 RP2350

我们喜欢 Google Pigweed！Pigweed 是Google 于 2020 年推出的一个开源项目。我们喜欢它，因为它可以帮助程序员和开发团队为使用微控制器（如我们的新RP2350及其前身RP2040 ）的嵌入式设备构建出色的软件。我们也偏爱有趣的产品名称；我们很高兴我们的 Pico W 在社区的俗语中被称为“pie cow”。

我们与 Pigweed 团队合作已近一年。上个月，他们将Bazel支持添加到我们的 Pico SDK 中，并将继续对其进行维护。

Bazel 是 Pigweed 项目的重要组成部分，该团队相信它将成为嵌入式软件开发的未来，使大型专业嵌入式开发团队能够更轻松地在 RP2350 之上构建原型和产品。请前往Bazel 的发布博客文章，了解有关 Bazel 对嵌入式的好处的更多信息。

Pigweed 团队已经构建了一个很棒的演示，供您在 Raspberry Pi Pico 1 或Pico 2上试用。这个演示展示了 Pigweed 处理和启用的许多复杂的东西，包括：

通过 Bazel 进行密封构建、刷新和测试
完全开源的嵌入式 Clang/LLVM 工具链，包括具有现代性能、功能和标准合规性的编译器、链接器和 C/C++ 库
通过 Pigweed 丰富的库集合，围绕合理、与硬件无关的 C++ 构建代码库
通过 RPC 与 Pico 通信
通过交互式和可定制的 REPL 查看 Pico 日志并向 Pico 发送命令
使用 C++、Starlark 代码智能和 Bazel 命令集成在 Visual Studio Code 中创作
跨平台构建和工具链，在 macOS 或 Linux 上进行开发（Windows 支持即将推出）
主机上的设备模拟
使用 GitHub Actions 持续构建和测试

**<font color=red>构建Pigweed系统</font>**

<https://pigweed.dev/docs/showcases/sense/tutorial/setup.html>

# 5. Pico 2 文档


<https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-python-sdk.pdf>

这也适用于 Pico2。

对于设置 C 环境来说，这很方便（如果你想放弃 python 并使用 C，这相当高级）：

<https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf>

它看起来很新，并且因为它引用了新的 VSCode 插件，所以应该很容易遵循。

最后，但并非最不重要的是 C SDK 上的文档：

<https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf>

from

<https://www.reddit.com/r/raspberrypipico/comments/1exqudf/pico_2_documentation/>

# 6. Raspberry Pi Pico W 初学者课程

Paul McWhorter

<https://www.youtube.com/playlist?list=PLGs0VKk2DiYz8js1SJog21cDhkBqyAhC5>

# 7. 如何构建 Raspberry Pi 集群

## 7.1 官方教程

清单
- 8 个 Raspberry Pi 4
- 8 个 Raspberry Pi PoE+ HAT
- 8 端口千兆 PoE 交换机
- USB 3 转千兆以太网适配器
- USB 3 转 SATA 适配器
- SSD SATA 驱动器
- 8 条以太网电缆
- 16 GB SD 卡
- 集群架

<https://www.raspberrypi.com/tutorials/cluster-raspberry-pi-tutorial/>

## 7.2 Raspberry Pi 3B 构建集群教程

清单
- 3 个 Raspberry Pi 3 Model B — 用于计算节点
- 1 个 Raspberry Pi 3 Model B — 用于主/登录节点
- 4 张 MicroSD 卡
- 4 条微型 USB 电源线
- 1 个 8 端口 10/100/1000 网络交换机
- 1x 6 端口 USB 电源
- 1x 64GB USB 驱动器（或 NAS，见下文）

第一部分 — 基础知识
<https://glmdev.medium.com/building-a-raspberry-pi-cluster-784f0df9afbd>

第二部分 - 一些简单的工作
<https://glmdev.medium.com/building-a-raspberry-pi-cluster-aaa8d1f3d2ca>

第三部分 —OpenMPI、Python 和并行作业
<https://glmdev.medium.com/building-a-raspberry-pi-cluster-f5f2446702e8>

## 7.3 ClusterHat 教程 Pi Zero W

- 1 x ClusterHat — 购买链接有单品或套件可供选择
- 1 x Raspberry Pi 3 或 4 —我正在使用 Raspberry Pi 3，它运行良好。
- 4 个 Raspberry Pi Zero 或 Zero W —无线网络不是必需的，但如果你已经有一个 W，你可以把它插上
- 5 张 MicroSD 卡 —这将保存每个 Raspberry Pi 的操作系统。ClusterHat网站上有一个教程，可让您通过网络运行节点映像。但是，虽然这种方法可以为您节省一点钱，但您应该知道，节点的运行速度很可能会更慢，因为它们将通过网络运行其操作系统。
- 1 个拇指驱动器或外部硬盘驱动器 —可选，但推荐
- PSU —主控制器 Raspberry Pi 将为其他控制器供电，因此您需要确保电源足够强大，能够为所有三个控制器供电。整个系统的最低功率要求为 1–1.2A（取决于您使用的是 Zeros 还是 Zero Ws），我使用 2.5A PSU 运行该设置时没有遇到任何问题
- 耐心 —我花了一整个下午才看完 Mill 的教程，因为我必须将他的方法翻译成 ClusterHat，并解决自他第一次写教程以来似乎出现的一些问题。我非常熟悉 Linux 和命令行，本教程也反映了这一点。您的情况可能会有所不同！

<https://medium.com/@dhuck/the-missing-clusterhat-tutorial-45ad2241d738>

ClusterHat 淘宝链接
<https://item.taobao.com/item.htm?abbucket=1&id=706903663956&ns=1&pisk=gAF-LkbuTijoxk82TH6mKZUgoKQcmWUPquz6tDmkdoEYRmAhzbXE9knYY0DoN0AK9yEUxkUFz2iQAkn3EtfgzzlEOGAds14za-rP3kHSOqTbuVpBF1x8Pb8SOGjG9KYjUgcQKCvNtm9j7mgSRY95ksgK8XgSV2_xc23wd3ZIOZQxW2YWPLgBhngZc3iIRLajcV3MNUgSRZUj02Gz-diFrDOLLkFbbwdikBOQM4HfnzifKoFjy7oTP7dBOeu-ecaSDGxrO5kb8vFe8BH3PRrE5ut5vDPYl7w_fivoVR3LSJE1-Lump7lxA71wWmN8JSHzn39SWbn-C7ZX7N4xd-FxZ7seQr4xVAh0ntSoKbE8Qck53irLk0qQwxtRmD2go7MYfiAYYveQZjN5c1IzL5V9dOxiX2v5kZpeLYg4yzM6eaL4LhgxjZ4eLpkDkqnGkZpeLYgqkcbmhpJEnEC..&priceTId=213e386217273227471263717e3f46&skuId=5137159806411&spm=a21n57.1.item.4.44fe523cX52glq&utparam=%7B%22aplus_abtest%22%3A%2275ef080006834215d1113927bd8c76b1%22%7D&xxc=taobaoSearch>

# 8. Raspberry Pi Pico 2 构筑自己的音序器

大家非常熟悉 Raspberry Pi 和 Raspberry Pi Pico 在音乐行业的潜力，并且都梦想着组建自己的 Pi 乐队。正是像 Arnov Sharma 这样的项目，通过展示最小的 Raspberry Pi Raspberry Pi Pico 的酷炫潜力，永远重新点燃了这种幻想。使用大家最喜欢的微控制器，他组装了一个由 Pico 提供支持的音序器。

![](/picture/pico_music.png)

根据 Sharma 的说法，这个项目的灵感来自 Teenage Engineering 的 Pocket Operator 合成音序器。顾名思义，这些是小型袖珍的音序器，可以使用其集成的工具套件在您喜欢的任何地方轻松召唤音乐。

这个定制的 Raspberry Pi Pico 迭代由 25 个按钮组成，这些按钮排列在一个矩阵中，使用 Pico 上的 GPIO 进行作。它有一个用于音频输出的扬声器，并依靠音频放大模块来处理声音。最终结果是一个类似的音序器，还有一个额外的好处，那就是从头开始为自己构建一些东西。

![](/picture/pico_music1.png)

控制一切的主板是最新的 Raspberry Pi Pico 2。它连接到一个定制的 PCB，该 PCB 为以 5 x 5 网格模式布局的所有按钮留出了空间。选择的音频放大模块是一种PAM8403，它使 Pico 能够通过连接的扬声器输出音乐。该项目的源代码已在 Hackster 上提供，供任何人探索。在其中，我们很好地了解了 Sharma 编程到这个特定音序器中的一些工具，其中包括录制音频序列、添加延迟甚至从 Pico 生成音调的能力

<https://www.hackster.io/Arnov_Sharma_makes/pico-sequencer-173a5f>

# 9. Raspberry运行Deepseek 200 token/s

<https://itsfoss.com/deepseek-r1-raspberry-pi-5/#performance-stats>

<https://mp.weixin.qq.com/s/DKayTUXhsR_eJ7jnqzi7jg>

推特原文，但是没给设备清单

<https://x.com/BrianRoemmele/status/1882436734774043055>

可以设置集群

<https://turingpi.com/>

# 9. FPGA

人们通常使用两大 FPGA 供应商 Alter（现为 Intel）和 Xilinx。这两家供应商都提供应用程序，允许用户使用 Verilog 和 VHDL 为其 FPGA 编写 HDL。他们会将代码编译成 FPGA 所需的逻辑连接，并允许将配置下载到 FPGA。

但这两家供应商都不适用于树莓派。Alter 和 Xilinx 提供适用于 Windows 和 Linux 的工具，但不适用于树莓派的 ARM 处理器。

不过好消息是，您可以使用 Lattice Inc 提供的免费开源工具对 FPGA 进行编程，该工具可以编译 Verilog 并下载到 FPGA。Yosys
信息：http://www.clifford.at/yosys/

这里有一个关于如何安装 Yosys 工具的详细说明：http://chiphack.org/chiphack-2017-install-linux.html

<https://forums.raspberrypi.com/viewtopic.php?t=262231>

Yosys安装需要修改

http://chiphack.org/chiphack-2017-install-linux.html

Downloading and installing pre-requisites
These are needed for compiling and installing the icestorm, Arachne-PNR and yosys tools later.

For Debian-based distributions, use the following command:

~~~
sudo apt-get install build-essential clang bison flex libreadline-dev \
gawk tcl-dev libffi-dev git mercurial graphviz xdot pkg-config python \
	  python3 libftdi-dev vim htop screen iverilog
~~~

需要修改成以下命令

sudo apt-get install build-essential clang bison flex libreadline-dev \
gawk tcl-dev libffi-dev git mercurial graphviz xdot pkg-config \
python3 python-is-python3 libftdi-dev vim htop screen iverilog

加上 python-is-python3，让 python 命令自动等于 python3。

避免了废弃的 python 包引发错误。

| 包名                      | 用途说明                                     |
| ----------------------- | ---------------------------------------- |
| `build-essential`       | 安装 GCC 编译器及基本开发工具（make、g++ 等）            |
| `clang`                 | LLVM 的 C/C++ 编译器，现代开发常用                  |
| `bison`, `flex`         | 分别是语法分析器/词法分析器生成器，常用于编译器前端               |
| `libreadline-dev`       | 用于命令行界面支持（如带箭头键历史的 CLI 工具）               |
| `gawk`                  | GNU AWK，处理文本和脚本语言工具                      |
| `tcl-dev`               | 支持 Tcl 脚本语言的开发库（例如 openROAD 工具依赖）        |
| `libffi-dev`            | 支持 C 与其他语言交互的 Foreign Function Interface |
| `git`, `mercurial`      | 两种主流版本控制系统，获取源代码常用                       |
| `graphviz`, `xdot`      | 图可视化工具，例如显示电路图、状态机图                      |
| `pkg-config`            | 协助编译器找到正确的头文件和库路径                        |
| `python`, `python3`     | Python 2/3 运行环境，很多脚本依赖（见下文说明）            |
| `libftdi-dev`           | 用于与 FTDI USB 转串口芯片通信，适用于 FPGA 开发板        |
| `vim`, `htop`, `screen` | 常用编辑器/系统监控/多终端工具                         |
| `iverilog`              | Verilog 模拟器，用于测试/验证数字逻辑设计                |



 执行到这里时出错了

 Downloading and installing Yosys
Starting in the same directory:

git clone https://github.com/cliffordwolf/yosys.git yosys
cd yosys
make -j8
sudo make install

你的 Yosys 编译报错了，原因非常明确，是 **缺少子模块（submodule）和依赖的头文件**。下面详细说明并提供修复方法。

---

## ❌ 报错信息分析

关键错误信息是：

```
fatal error: libs/cxxopts/include/cxxopts.hpp: No such file or directory
```

说明 Yosys 依赖的 **`cxxopts.hpp` 文件没下载到**，而这个文件本应该在 Git 的子模块中。

同时还有：

```
make: *** [Makefile:794: check-git-abc] Error 1
Initialize the submodule: Run 'git submodule update --init' to set up 'abc' as a submodule.
```

说明你**还没有初始化 Git 子模块**，包括 `abc` 这个用于逻辑优化的核心工具。

---

## ✅ 解决方法（3 步）

### **① 初始化 Git 子模块**

在 Yosys 项目目录下运行以下命令：

```bash
git submodule update --init --recursive
```

这将会拉取所有 Yosys 所需的子模块（包括 `abc`、`cxxopts` 等）。

> 📌 **必须执行，否则 make 会找不到依赖项**

---

### **② 然后重新编译**

子模块初始化完成后，重新执行：

```bash
make -j8
```

---

### **③ 安装 Yosys（可选）**

编译成功后，执行安装命令：

```bash
sudo make install
```

这会将 Yosys 安装到 `/usr/local/bin/yosys`，你就可以直接运行：

```bash
yosys
```

---

## 🧪 验证是否成功

```bash
yosys -V
```

输出示例：

```
Yosys 0.26+123 (git sha1 abc123, clang 14.0.0 -fPIC -Os)
```

---

## ✅ 总结

| 问题                          | 原因              | 解决                                        |
| --------------------------- | --------------- | ----------------------------------------- |
| `cxxopts.hpp: No such file` | 缺少子模块 `cxxopts` | `git submodule update --init --recursive` |
| `check-git-abc` 报错          | 缺少子模块 `abc`     | 同上                                        |
| 编译失败                        | 缺文件、依赖未拉取       | 拉取子模块并重新 make                             |

---

如你后续还要编译 openFPGA、NextPNR 或 sky130 toolchain，也会遇到类似的 `submodule` 问题，通用命令是：

```bash
git clone --recursive <repo_url>
```

或者：

```bash
git submodule update --init --recursive
```

是的，这个报错确实是 **网络问题** 引起的，尤其是访问 GitHub 时 TLS 连接中断。错误信息：

```
GnuTLS recv error (-110): The TLS connection was non-properly terminated.
fatal: clone of 'https://github.com/YosysHQ/abc' into submodule path '/home/basteng/icestorm/yosys/abc' failed
```

### ✅ 解释：

* 这是 `git` 在使用 HTTPS 协议连接 GitHub 拉取子模块时发生的 TLS 层连接超时或被中断。
* 这类问题在 **国内网络环境** 或 **不稳定 WiFi/VPN** 下较常见。

---

## ✅ 解决方法：

### **方法 1：重试几次**

最简单直接的方法，有时候是 GitHub 一时不稳定或网络波动，重新执行：

```bash
git submodule update --init --recursive
```

---

### **方法 2：切换使用 SSH 拉取**

如果你配置了 GitHub 的 SSH key，可以使用 SSH 替代 HTTPS，避免 TLS 问题。

1. 修改子模块地址：

```bash
git config --file .gitmodules submodule.abc.url git@github.com:YosysHQ/abc.git
```

2. 再运行子模块更新命令：

```bash
git submodule sync
git submodule update --init --recursive
```

如果你还未配置 GitHub 的 SSH key，可参考 GitHub 指南：[https://docs.github.com/en/authentication/connecting-to-github-with-ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

---

### **方法 3：使用代理或 VPN**

如果你处于中国大陆或公司网络环境，访问 GitHub 被限，可以考虑：

* 启用 VPN。
* 配置 git 使用代理，例如：

```bash
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890
```

> 将 `7890` 替换为你本地代理工具的端口。

---

### **方法 4：手动克隆子模块**

如果仍然失败，可以手动克隆子模块：

```bash
cd yosys
git clone https://github.com/YosysHQ/abc.git abc
```

然后再继续编译。

---

## ✅ 总结

| 方法     | 适用场景                    |
| ------ | ----------------------- |
| 重试命令   | 一般网络波动                  |
| 切换 SSH | 已配置 SSH key，跳过 HTTPS 问题 |
| 配置代理   | 境内访问 GitHub 不稳定         |
| 手动克隆   | 临时解决子模块拉取失败问题           |


**可以选择方法4**

你现在这个错误：

```
fatal error: libs/cxxopts/include/cxxopts.hpp: No such file or directory
```

说明 Yosys 的依赖库 **`cxxopts` 子模块仍未成功拉取**，导致 `make` 编译失败。

---

## 🔍 根本原因

你在上一步执行了：

```bash
git submodule update --init --recursive
```

但因为网络问题（`GnuTLS recv error`），子模块没有拉取成功，**`abc` 和 `cxxopts` 都缺失**。Yosys 使用 `libs/cxxopts` 提供命令行参数解析功能，编译 `driver.cc` 时必须用到。

---

## ✅ 解决步骤

### 🔁 **步骤 1：确认子模块状态**

在 Yosys 根目录下运行：

```bash
git submodule status
```

如果看到如下类似内容，表示子模块未初始化成功：

```
-<hash> abc
-<hash> libs/cxxopts
```

说明你 **还需要重新拉取子模块**。

---

### 🔧 **步骤 2：重新拉取子模块（推荐使用手动克隆）**

#### ✅ 方法 1：逐个手动克隆

你可以手动拉取子模块，避免网络中断带来的问题。

```bash
cd yosys
# 克隆 abc 子模块
git clone https://github.com/YosysHQ/abc.git abc

# 克隆 cxxopts 子模块
git clone https://github.com/jarro2783/cxxopts.git libs/cxxopts
```

然后重新编译：

```bash
make -j8
```

---

#### ✅ 方法 2：如果网络稳定了，也可以重新尝试自动拉取

```bash
git submodule update --init --recursive
```

如果还是失败，建议优先用方法 1。

---

### ✅ 步骤 3：编译验证

执行：

```bash
make -j8
```

如无报错，再执行：

```bash
sudo make install
```

最后验证：

```bash
yosys -V
```

---

### 🔚 总结

| 问题               | 原因               | 解决方案                            |
| ---------------- | ---------------- | ------------------------------- |
| `cxxopts.hpp` 缺失 | 子模块没拉到           | 手动 `git clone` 到 `libs/cxxopts` |
| `abc` 缺失也会报错     | 同上               | 手动 `git clone` 到 `abc/`         |
| 网络 TLS 报错        | 境内访问 GitHub 慢或中断 | 使用 VPN 或代理，或改成 SSH 克隆           |

是否还准备安装下一步的 `nextpnr`？我可以继续帮你配置完整 iCE40 工具链。


你的输出说明：

* ✅ `abc` 子模块已经成功拉取（前面没有 `-` 号）。
* ❌ `libs/cxxopts` 子模块 **没有拉取成功**（前面有 `-` 号，表示未初始化）。

---

### ✅ 解决方案：单独拉取 `libs/cxxopts` 子模块

在 `yosys` 根目录下执行以下命令：

```bash
git submodule update --init libs/cxxopts
```

这会只拉取缺失的 `cxxopts` 子模块，避免重新尝试拉全部（提高成功率）。

---

### 💡 如果仍失败（网络不稳），可以手动拉取

```bash
git clone https://github.com/jarro2783/cxxopts.git libs/cxxopts
```

---

### ✅ 然后重新编译

```bash
make -j8
sudo make install
```

完成后验证：

```bash
yosys -V
```

---

是否还要继续搭建 `nextpnr`？它是和 `yosys + icestorm + arachne-pnr` 配套的 iCE40 P\&R 工具。需要我继续帮你安装下一步吗？


你的最后一步出现错误是因为 **你在源代码目录中尝试了“in-tree build”**，而 `nextpnr` 项目强制要求“out-of-tree build”（即构建目录和源码目录必须分离）。

---

## ✅ 正确的构建方式如下（请严格照做）：

你当前目录应该是：

```
~/nextpnr
```

### 步骤 1：新建构建目录并进入

```bash
mkdir build
cd build
```

### 步骤 2：配置 CMake（仍然在 `build` 目录中）

```bash
cmake -DARCH=ice40 -DCMAKE_INSTALL_PREFIX=/usr/local ..
```

注意：这里的 `..` 表示指向上级的源代码目录。

### 步骤 3：编译并安装

```bash
make -j$(nproc)
sudo make install
```

---

执行以上三步后，`nextpnr` 就会被正确编译并安装到 `/usr/local/bin/nextpnr-ice40`。

是否要我帮你检查后续如何与 `yosys` 一起使用编译 Verilog 程序？


你还是在用**错误的方式**运行 `cmake`，报错提示也说得很清楚：

> ❌ **“In-tree builds are not supported.”**

---

### ✅ 正确做法是：**从 nextpnr 根目录外的 `build` 子目录中调用 `cmake` 并指定 `..` 为源码路径**

你现在已经在 `~/nextpnr/build` 目录下了，所以只需运行这条命令即可：

```bash
cmake .. -DARCH=ice40 -DCMAKE_INSTALL_PREFIX=/usr/local
```

接着继续执行：

```bash
make -j$(nproc)
sudo make install
```

---

### 总结

你已经创建好了 `build/` 子目录，现在只要在里面执行 `cmake ..` 并加上选项即可。不需要像提示里的 `cmake . -B build`，因为你已经进入了 `build` 目录。

你要不要我提供一个完整的一键构建脚本？


你收到这个报错的原因是你之前可能在 `~/nextpnr` 目录下直接运行过 `cmake` 命令，结果污染了源码目录。虽然你后来新建了 `build/` 子目录，但源码目录中的缓存文件还在，导致 `cmake` 仍然报错。

---

### ✅ 解决方法如下：

#### 第一步：**清除源码目录中的缓存文件**

回到 `nextpnr` 根目录并删除缓存文件：

```bash
cd ~/nextpnr
rm -rf CMakeCache.txt CMakeFiles
```

如果你不确定有哪些残留，可以更彻底地清除所有非源码文件（别担心，git 会保护源码）：

```bash
git clean -fdx
```

> 这会删除所有没有被 Git 跟踪的文件，包括你错误生成的 CMake 缓存。

---

#### 第二步：**重新创建 build 目录并配置编译**

```bash
mkdir -p ~/nextpnr/build
cd ~/nextpnr/build
cmake .. -DARCH=ice40 -DCMAKE_INSTALL_PREFIX=/usr/local
make -j$(nproc)
sudo make install
```

---

这样就能正确完成 `nextpnr` 的构建了。

你需要我帮你写一个自动构建的 shell 脚本吗？

# 10. 树莓派4B bookworm设置成热点

你问得非常到位。这个问题的根源在于：**你创建热点失败后，系统误把你设置的热点名 `RPI4B-basteng` 当成了一个普通 Wi-Fi 网络（client 模式）来尝试连接**，而不是作为一个热点（Access Point）去广播它。

---

## 📌 为何 `RPI4B-basteng` 没变成热点，反而被当作 Wi-Fi 去连接？

### 🔍 原因可能有以下几种：

1. **图形界面创建热点失败时，NetworkManager 保存了一个“类型为 Wi-Fi”的连接配置，但默认是 `client` 模式（managed），不是 `ap` 模式。**

   * 你设了 SSID 为 `RPI4B-basteng`，但 NetworkManager 只记录了名称，没能切换模式。
   * 所以系统尝试“连接”这个 SSID，而不是“广播”它。

2. **NetworkManager 没成功创建 `Hotspot` 类型的连接，而是保留了一个残缺配置，处于“connecting”状态。**

3. **配置中“Wi-Fi 模式”选错了，默认是“客户端模式（managed）”而不是“热点模式（ap）”。**

---

## ✅ 解决方法：彻底清掉错误配置，重新用命令方式创建热点

### 🧹 步骤 1：删除错误连接配置

```bash
nmcli connection delete "RPI4B-basteng"
```

你也可以同时删除其他不需要的 Wi-Fi 记录：

```bash
nmcli connection delete preconfigured
```

---

### 🚀 步骤 2：创建正确的热点（AP）连接

```bash
nmcli dev wifi hotspot ifname wlan0 ssid RPI4B-basteng password 12345678
```

这条命令会：

* 创建临时热点配置，名称默认叫 `Hotspot`，SSID 是你设置的 `RPI4B-basteng`
* 将 wlan0 设置为 AP 模式
* 分配静态 IP 地址（如 10.42.0.1）
* 启动内置 DHCP 服务

---

### ✅ 验证成功

运行：

```bash
nmcli device show wlan0
```

你应该看到：

* `GENERAL.STATE: 100 (connected)`
* `WI-FI.MODE: AP`
* `WI-FI.SSID: RPI4B-basteng`

用手机就能看到这个热点。

---

## 💡 总结一句话：

你设置热点失败时，`RPI4B-basteng` 被 NetworkManager 错误地保存为“客户端连接配置”，所以系统试图去连它，而不是广播它。正确方法是删除旧配置，用 `nmcli` 重新创建一个**AP模式的热点**。

是否需要我生成一个脚本文件，今后你一键执行就能创建热点？

# 11. 树莓派翻墙自动配置

太好了！下面是为你量身定制的脚本 ✅，用于：

> 📦 一键配置树莓派热点 + 自动开机自启 + 设置 Shadowsocks 翻墙透明代理（含 iptables 规则）+ 自动保存规则。

---

## ✅ 脚本用途说明

* 创建热点：`RPI4B-basteng`，密码 `12345678`
* 设置 NetworkManager 热点自动连接
* 设置 `ss-redir` 自启并监听 1081
* 设置 iptables NAT 转发规则
* 保存规则并确保开机加载

---

## 📜 脚本内容（文件名建议为：`setup-hotspot-proxy.sh`）

```bash
#!/bin/bash
set -e

echo "🚀 配置热点和翻墙代理环境..."

### 1. 创建热点连接（如果不存在）
if ! nmcli connection show | grep -q "RPI4B-basteng"; then
    echo "📡 创建热点连接 RPI4B-basteng..."
    nmcli dev wifi hotspot ifname wlan0 ssid RPI4B-basteng password 12345678
fi

### 2. 设置热点开机自启
echo "🔧 设置热点开机自动连接..."
sudo nmcli connection modify Hotspot connection.id RPI4B-basteng
sudo nmcli connection modify RPI4B-basteng connection.autoconnect yes

### 3. 禁用其他 Wi-Fi 自动连接
for conn in $(nmcli -t -f NAME,TYPE connection show | grep wifi | cut -d':' -f1); do
    if [[ "$conn" != "RPI4B-basteng" ]]; then
        echo "⛔ 禁用自动连接：$conn"
        sudo nmcli connection modify "$conn" connection.autoconnect no
    fi
done

### 4. 启动 Shadowsocks-redir 服务
echo "🛡️ 启动 Shadowsocks-redir..."
sudo systemctl enable shadowsocks-libev-redir@redir
sudo systemctl restart shadowsocks-libev-redir@redir

### 5. 启用 IP 转发
echo "🌐 启用 IP 转发..."
sudo sysctl -w net.ipv4.ip_forward=1
sudo sed -i 's/^#\?net.ipv4.ip_forward=.*/net.ipv4.ip_forward=1/' /etc/sysctl.conf

### 6. 写入 iptables NAT 规则
echo "📦 写入 iptables 规则..."
sudo iptables -t nat -F
sudo iptables -t nat -A PREROUTING -i wlan0 -d 192.168.0.0/16 -j RETURN
sudo iptables -t nat -A PREROUTING -i wlan0 -d 10.0.0.0/8 -j RETURN
sudo iptables -t nat -A PREROUTING -i wlan0 -d 127.0.0.0/8 -j RETURN
sudo iptables -t nat -A PREROUTING -i wlan0 -p tcp -j REDIRECT --to-ports 1081
sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE

### 7. 安装并保存规则（如果未安装）
if ! dpkg -s iptables-persistent &>/dev/null; then
    echo "📦 安装 iptables-persistent..."
    sudo DEBIAN_FRONTEND=noninteractive apt install -y iptables-persistent
fi

sudo iptables-save | sudo tee /etc/iptables/rules.v4 > /dev/null
sudo chmod -x /usr/share/netfilter-persistent/plugins.d/25-ip6tables
sudo systemctl enable netfilter-persistent
sudo systemctl restart netfilter-persistent

echo "✅ 完成！系统已配置为热点 + 翻墙网关模式。建议重启验证效果。"
```

---

## 🔧 使用说明

1. 将脚本保存为 `setup-hotspot-proxy.sh`
2. 赋予执行权限：

```bash
chmod +x setup-hotspot-proxy.sh
```

3. 运行：

```bash
./setup-hotspot-proxy.sh
```

---

## 📌 注意事项

* 脚本假设你已设置好 `/etc/shadowsocks-libev/redir.json`
* 如果你用的不是 `eth0` 作为出口，请将脚本中的 `-o eth0` 改为对应接口（如 `tun0`）
* 脚本自动跳过旧 Wi-Fi 的自动连接，避免冲突

---

如你还想添加功能（如自动更新 DNS、测试连通性、日志记录等），我可以继续扩展脚本。是否需要？

## 如果原有服务器失效，操作如下

* 重新设置脚本 `sudo nano /etc/shadowsocks-libev/redir.json` 改变IP等信息
* 重启服务 `sudo systemctl restart shadowsocks-libev-redir@redir`

# 12. RPi USB Wi-Fi 适配器

<https://elinux.org/RPi_USB_Wi-Fi_Adapters#Working_USB_Wi-Fi_Adapters>

# 13. 树莓派5运行claude，现在使用claude-start即可

基本上是的！但有几个细节需要注意：

## 正常情况下：
```bash
~/claude-start.sh
```
就够了，会自动检查和启动所有必要的服务。

## 但可能需要的情况：

**1. 第一次重启后：**
```bash
# shadowsocks 可能需要手动启动一次
sudo systemctl start shadowsocks-libev-local@config

# 然后运行脚本
~/claude-start.sh
```

**2. 如果想让 shadowsocks 开机自启：**
```bash
sudo systemctl enable shadowsocks-libev-local@config
```

**3. 更简单的日常使用：**
一旦所有服务都稳定运行后，你甚至可以直接：
```bash
graftcp claude
```

## 我建议创建一个别名：
```bash
echo "alias claude-proxy='~/claude-start.sh'" >> ~/.bashrc
source ~/.bashrc
```

然后就可以：
```bash
claude-proxy
```

## 或者更简单，创建软链接：
```bash
sudo ln -s ~/claude-start.sh /usr/local/bin/claude-start
```

然后在任何地方都可以：
```bash
claude-start
```

**总结：** 是的，基本上运行 `~/claude-start.sh` 就可以了，这个脚本会处理所有的启动和检查工作！🎯

# 14. 需要使用grafcp才能在树莓派上运行claude

哈哈，太好了！🎉

原来是需要一点时间让代理连接稳定！这确实是常见的情况：

1. **graftcp-local 需要时间建立连接**
2. **Claude Code 启动时的网络检测需要通过代理完成**
3. **第一次连接可能需要等待几秒钟**

现在你的 Claude Code 应该可以正常使用了！

## 创建一个便捷的启动脚本：

```bash
nano ~/claude-start.sh
```

内容：
```bash
#!/bin/bash
echo "🚀 启动 Claude 代理环境..."

# 检查 shadowsocks
if ! pgrep ss-local > /dev/null; then
    echo "启动 shadowsocks..."
    sudo systemctl start shadowsocks-libev-local@config
    sleep 2
fi

# 启动 graftcp-local
if ! pgrep graftcp-local > /dev/null; then
    echo "启动 graftcp-local..."
    graftcp-local -socks5 127.0.0.1:1080 -listen 127.0.0.1:2233 &
    sleep 3  # 给更多时间让代理稳定
fi

echo "✅ 代理就绪，启动 Claude Code..."
echo "提示: 如果连接失败，请等待几秒钟再试"
echo "----------------------------------------"

graftcp claude
```

使用：
```bash
chmod +x ~/claude-start.sh
~/claude-start.sh
```

这样以后就可以一键启动整个代理环境和 Claude Code 了！

恭喜你成功在树莓派上运行 Claude Code！现在可以享受 AI 编程助手的强大功能了！ 🎊

# 15. 树莓派科学上网修改IP

要更改 **Shadowsocks-libev** 服务（`shadowsocks-libev-local@config`）的翻墙服务器 **IP 地址**，您需要修改配置文件 `/etc/shadowsocks-libev/config.json` 中的 **`server`** 字段。

以下是修改步骤：

### 1. **编辑配置文件**

在树莓派上，打开 **Shadowsocks-libev** 配置文件 `/etc/shadowsocks-libev/config.json` ：

```bash
sudo nano /etc/shadowsocks-libev/config.json
```

### 2. **修改服务器 IP 地址**

在配置文件中，找到 **`server`** 字段，这里存储的是翻墙服务器的 **IP 地址**。您只需要将 **`server`** 字段更新为新的翻墙服务器的 **IP 地址**。

例如，修改前：

```json
{
  "server": "old-server-ip",   // 之前的服务器 IP
  "server_port": 8388,         // 服务器端口
  "password": "your-password", // 密码
  "method": "aes-256-gcm",     // 加密方式
  "local_address": "127.0.0.1",
  "local_port": 1080,
  "timeout": 300
}
```

修改后：

```json
{
  "server": "new-server-ip",   // 新的服务器 IP
  "server_port": 8388,         // 服务器端口
  "password": "your-password", // 密码
  "method": "aes-256-gcm",     // 加密方式
  "local_address": "127.0.0.1",
  "local_port": 1080,
  "timeout": 300
}
```

确保 **`server`** 字段更新为新的翻墙服务器的 **IP 地址**。

### 3. **保存并退出**

在编辑完成后，按 `Ctrl + X` 退出编辑器，然后按 `Y` 保存文件，再按 `Enter` 确认保存。

### 4.找出之前占用1080端口的PID，并且kill

如果你想保持本地端口为1080，需要先找出并停止占用1080端口的进程：

# 找出占用1080端口的进程
sudo netstat -tlnp | grep 1080

# 停止该进程（假设PID是12345）
sudo kill 12345

### 5. **重启 Shadowsocks 服务**

为了使配置生效，需要重启 **Shadowsocks** 服务：

```bash
sudo systemctl restart shadowsocks-libev-local@config
```

### 6. **检查服务状态**

确认 **Shadowsocks** 服务已成功重启，并且没有错误：

```bash
sudo systemctl status shadowsocks-libev-local@config
```

您应该看到类似以下的输出，说明服务正在运行：

```
● shadowsocks-libev-local@config.service - Shadowsocks-Libev Custom Client Service for config
     Loaded: loaded (/lib/systemd/system/shadowsocks-libev-local@.service; enabled; preset: enabled)
     Active: active (running) since [timestamp]
       Docs: man:ss-local(1)
   Main PID: [PID]
      Tasks: 1 (limit: 9568)
     CPU: 10ms
     CGroup: /system.slice/system-shadowsocks\x2dlibev\x2dlocal.slice/shadowsocks-libev-local@config.service
             └─[PID] /usr/bin/ss-local -c /etc/shadowsocks-libev/config.json
```

### 7. **测试翻墙是否正常**

使用以下命令测试翻墙是否正常工作：

```bash
curl --proxy socks5://127.0.0.1:1080 https://www.google.com
```

如果能够成功访问 Google，说明新的翻墙服务器已正确配置并工作正常。

---

### 总结：

1. 编辑 `/etc/shadowsocks-libev/config.json` 配置文件，将 **`server`** 字段中的 IP 地址更新为新的翻墙服务器的 IP 地址。
2. 重启 **Shadowsocks** 服务使配置生效。
3. 使用 `curl` 测试翻墙是否正常。

如果您遇到任何问题，或者服务无法启动，请提供更多的错误信息，我们可以进一步帮助您排查。

# 16. 树莓派透明代理设置

1.停掉ss-local

要停止 `ss-local` 服务，您可以执行以下命令：

1. **停止 `ss-local` 服务：**

   ```bash
   sudo systemctl stop shadowsocks-libev-local@config
   ```

   这将停止 `ss-local` 服务（假设它使用的是 `config` 配置）。

2. **检查 `ss-local` 是否已停止：**
   您可以使用以下命令确认 `ss-local` 是否已经停止：

   ```bash
   sudo systemctl status shadowsocks-libev-local@config
   ```

   如果显示为 `inactive (dead)`，则表示已成功停止。

3. **禁用 `ss-local`（如果不打算再次启用）：**
   如果您不打算重新启用 `ss-local`，可以禁用它：

   ```bash
   sudo systemctl disable shadowsocks-libev-local@config
   ```

通过这些步骤，您可以停掉 `ss-local` 服务，从而避免 `ss-local` 和 `ss-redir` 之间的端口冲突。


2.设置ss-redir

## 解决方案

### 1. 修正绑定参数
`-b wlan0` 参数有问题，应该使用具体 IP 地址：

```bash
# 查看 wlan0 的 IP 地址
ifconfig wlan0

# 假设 wlan0 IP 是 192.168.4.1，使用：
ss-redir -c /etc/shadowsocks-libev/redir.json -b 192.168.4.1 -l 1081

# 或者简单使用监听所有接口：
ss-redir -c /etc/shadowsocks-libev/redir.json -l 1081
```

### 2. 检查配置文件
确认 `/etc/shadowsocks-libev/redir.json` 的内容：

```bash
cat /etc/shadowsocks-libev/redir.json
```

配置应该类似：
```json
{
    "server": "你的服务器域名或IP",
    "server_port": 443,
    "local_address": "0.0.0.0",
    "local_port": 1081,
    "password": "你的密码",
    "method": "aes-256-gcm",
    "timeout": 300
}
```

### 3. 检查端口占用
```bash
# 检查 1081 端口是否被占用
netstat -tlnp | grep 1081

# 如果被占用，杀掉相关进程或换端口
```

### 4. 测试网络连接
```bash
# 测试能否连接到 SS 服务器
ping 你的服务器IP

# 测试服务器端口
telnet 你的服务器IP 你的服务器端口
```

### 5. 推荐的启动命令
```bash
# 最简单的启动方式
ss-redir -c /etc/shadowsocks-libev/redir.json -v

# 如果需要后台运行
ss-redir -c /etc/shadowsocks-libev/redir.json -f /var/run/ss-redir.pid
```

### 6. 更新加密方法
将配置文件中的 `"method"` 从 `"aes-256-cfb"` 改为：
- `"aes-256-gcm"` (推荐)
- `"chacha20-ietf-poly1305"`
- `"aes-128-gcm"`

先试试不使用 `-b` 参数的简单启动方式，看能否正常运行。

---------------------------------------------

### 2. 重启服务
```bash
sudo systemctl restart shadowsocks-libev-redir@redir
```

### 3. 验证监听地址
```bash
sudo netstat -tlnp | grep 1081
```
应该看到 `0.0.0.0:1081` 而不是 `127.0.0.1:1081`

### 4. 配置 iptables 透明代理规则
```bash
# 创建 SHADOWSOCKS 链
sudo iptables -t nat -N SHADOWSOCKS 2>/dev/null

# 清空可能存在的规则
sudo iptables -t nat -F SHADOWSOCKS

# 排除服务器和本地地址
sudo iptables -t nat -A SHADOWSOCKS -d 149.28.79.242 -j RETURN
sudo iptables -t nat -A SHADOWSOCKS -d 0.0.0.0/8 -j RETURN
sudo iptables -t nat -A SHADOWSOCKS -d 127.0.0.0/8 -j RETURN
sudo iptables -t nat -A SHADOWSOCKS -d 169.254.0.0/16 -j RETURN
sudo iptables -t nat -A SHADOWSOCKS -d 192.168.0.0/16 -j RETURN
sudo iptables -t nat -A SHADOWSOCKS -d 10.0.0.0/8 -j RETURN

# 重定向其他流量到 ss-redir
sudo iptables -t nat -A SHADOWSOCKS -p tcp -j REDIRECT --to-ports 1081

# 应用到 hotspot 客户端流量（假设你的 AP 网段是 192.168.4.0/24）
sudo iptables -t nat -A PREROUTING -s 192.168.4.0/24 -p tcp -j SHADOWSOCKS
```

### 5. 启用 IP 转发
```bash
echo 1 | sudo tee /proc/sys/net/ipv4/ip_forward
echo 'net.ipv4.ip_forward=1' | sudo tee -a /etc/sysctl.conf
```

### 6. 验证配置
```bash
# 检查服务状态
sudo systemctl status shadowsocks-libev-redir@redir

# 检查 iptables 规则
sudo iptables -t nat -L SHADOWSOCKS -n -v

# 检查监听端口
sudo netstat -tlnp | grep 1081
```

完成这些步骤后，手机连接到树莓派 hotspot 就能自动通过透明代理访问网络了。

---------------------------------

很好！iptables 规则已经正确配置了。我注意到你有两条 REDIRECT 规则（可能是重复添加了），但这不会影响功能。

## 当前配置状态检查

现在让我们确认所有组件都正常：

### 1. 检查 ss-redir 配置
确保 ss-redir 监听在 `0.0.0.0:1081`：
```bash
sudo netstat -tlnp | grep 1081
```
应该显示：`0.0.0.0:1081` 而不是 `127.0.0.1:1081`

如果还是 `127.0.0.1`，需要修改配置：
```bash
sudo nano /etc/shadowsocks-libev/redir.json
```
确保 `local_address` 是 `"0.0.0.0"`，然后重启：
```bash
sudo systemctl restart shadowsocks-libev-redir@redir
```

### 2. 启用 IP 转发
```bash
echo 1 | sudo tee /proc/sys/net/ipv4/ip_forward
```

### 3. 测试透明代理

**用手机测试**：
1. 连接到树莓派 hotspot
2. 访问 `whatismyipaddress.com` 或 `ipinfo.io`
3. 看显示的 IP 是否为你的 SS 服务器 IP (`149.28.79.242`)

**在树莓派上监控流量**：
```bash
# 实时查看 iptables 计数器变化
watch -n 1 'sudo iptables -t nat -L SHADOWSOCKS -n -v'
```
当手机访问网站时，应该看到 pkts 和 bytes 数值在增加。

### 4. 如果不工作，检查日志
```bash
# 查看 ss-redir 日志
sudo journalctl -u shadowsocks-libev-redir@redir -f

# 查看系统日志
sudo dmesg | tail -20
```

### 5. 保存 iptables 规则（重要）
配置工作后，保存规则以便重启后自动加载：
```bash
# 安装 iptables-persistent
sudo apt install iptables-persistent

# 保存当前规则
sudo iptables-save > /etc/iptables/rules.v4
```

试试手机连接测试，如果还有问题，贴一下 `sudo netstat -tlnp | grep 1081` 的输出结果。

------------------------------------

权限问题，需要用 `tee` 命令或者先创建目录：

## 解决方法

### 方法1: 使用 tee 命令
```bash
sudo iptables-save | sudo tee /etc/iptables/rules.v4
```

### 方法2: 先创建目录
```bash
# 创建目录
sudo mkdir -p /etc/iptables

# 保存规则
sudo iptables-save | sudo tee /etc/iptables/rules.v4
```

### 方法3: 使用 iptables-persistent 包
```bash
# 安装 iptables-persistent
sudo apt update
sudo apt install iptables-persistent

# 在安装过程中会询问是否保存当前规则，选择 Yes

# 或者安装后手动保存
sudo netfilter-persistent save
```

### 方法4: 手动创建启动脚本
如果上面方法不行，可以创建启动脚本：
```bash
# 创建脚本文件
sudo nano /etc/init.d/iptables-restore

# 添加以下内容：
#!/bin/bash
# 在启动时恢复 iptables 规则

# 你的 iptables 规则
iptables -t nat -N SHADOWSOCKS 2>/dev/null
iptables -t nat -F SHADOWSOCKS
iptables -t nat -A SHADOWSOCKS -d 149.28.79.242 -j RETURN
iptables -t nat -A SHADOWSOCKS -d 0.0.0.0/8 -j RETURN
iptables -t nat -A SHADOWSOCKS -d 127.0.0.0/8 -j RETURN
iptables -t nat -A SHADOWSOCKS -d 169.254.0.0/16 -j RETURN
iptables -t nat -A SHADOWSOCKS -d 192.168.0.0/16 -j RETURN
iptables -t nat -A SHADOWSOCKS -d 10.0.0.0/8 -j RETURN
iptables -t nat -A SHADOWSOCKS -p tcp -j REDIRECT --to-ports 1081
iptables -t nat -A PREROUTING -s 10.42.0.0/24 -p tcp -j SHADOWSOCKS

# 启用 IP 转发
echo 1 > /proc/sys/net/ipv4/ip_forward
```

```bash
# 设置执行权限
sudo chmod +x /etc/init.d/iptables-restore

# 添加到启动项
sudo update-rc.d iptables-restore defaults
```

推荐使用**方法1**或**方法3**，它们是最标准的做法。

-----------------------------------

也就是说，每次服务器失效的时候改变/etc/shadowsocks-libev/redir.json就可以了
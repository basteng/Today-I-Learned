- [1. 基于NTT的PQC乘法器的硬件实现](#1-基于ntt的pqc乘法器的硬件实现)
- [2. 推荐阅读](#2-推荐阅读)
  - [2.1 TCFPGA](#21-tcfpga)
- [3. 选型](#3-选型)
  - [3.1 赛灵思选型网站](#31-赛灵思选型网站)
- [4. Talos V2：在 FPGA 上跑 Karpathy 的 microGPT](#4-talos-v2在-fpga-上跑-karpathy-的-microgpt)
- [5. 1bitSDR：用 Lattice MachXO2 FPGA 做极简中波/短波 SDR 接收机](#5-1bitsdr用-lattice-machxo2-fpga-做极简中波短波-sdr-接收机)
  - [直接链接](#直接链接)
  - [原理](#原理)
  - [最小硬件配置](#最小硬件配置)
  - [调台方式](#调台方式)
  - [阅读顺序与注意事项](#阅读顺序与注意事项)


# 1. 基于NTT的PQC乘法器的硬件实现

我是电子与计算机工程专业即将升入大三的本科生。我拥有扎实的数字电子基础，能够使用 Verilog 语言对有限状态机 (FSM)、自动状态机 (ASM) 等硬件系统进行建模。我最近在一位教授的指导下接了一个项目，下学期将开始使用 FPGA。
在深入研究这个项目之前，他让我在这个暑假期间仔细阅读附件中关于 PQC 中 NTT 算法的研究论文，但我对密码学一无所知。这篇论文涉及大量数学知识，当我提到这一点时，他建议我尝试找出其中的研究空白。
我对研究论文还不熟悉，不确定该如何处理——应该关注什么，或者在没有完全理解数学知识的情况下如何处理数学问题，因为我在这个项目中的重点将主要放在学习如何在 FPGA 上编程和实现一些功能。
如果您能站在我的角度，分享一些关于如何进行这项工作的建议，我将不胜感激。谢谢！

<https://www.reddit.com/r/FPGA/comments/1m17pm5/hardware_implementation_of_ntt_based_multiplier/>

论文链接

A Flexible NTT-Based Multiplier for Post-Quantum Cryptography

<https://ieeexplore.ieee.org/document/10007837>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/A_Flexible_NTT-Based_Multiplier_for_Post-Quantum_Cryptography.pdf>

# 2. 推荐阅读

## 2.1 TCFPGA

<https://tcfpga.org/books/recommended-reading>

# 3. 选型

## 3.1 赛灵思选型网站

<https://docs.amd.com/v/u/en-US/ultrascale-plus-fpga-product-selection-guide>

# 4. Talos V2：在 FPGA 上跑 Karpathy 的 microGPT

Reddit 讨论原帖：

<https://www.reddit.com/r/FPGA/comments/1t2cvqe/karpathys_microgpt_running_at_50000_tps_on_an/>

项目说明（write-up）：

<https://v2.talos.wtf/>

GitHub 仓库：

<https://github.com/Luthiraa/TALOS-V2>

相关公司/路线参考：

<https://taalas.com/>

## 核心信息

- 这是一个把极小版 Transformer（Karpathy 的 microGPT）直接做成 RTL 硬件路径的项目，不是把通用大模型直接搬上 FPGA。
- 项目说明里提到目标板卡是 **DE1-SoC**，核心器件为 **Intel Cyclone V SoC FPGA**。
- 设计使用 **Q4.12 fixed-point（16 位定点）**，权重导出为 ROM 可加载的 hex 文件，尽量把权重放在片上而不是外部存储。
- 其核心思路不是做一套庞大的全并行 Transformer，而是围绕一个可复用的 **16-lane streamed systolic matrix-vector tile** 做时间复用。
- attention、softmax 近似、divider、sampling 等都做成了显式硬件模块/调度流程。
- write-up 中声称在 DE1-SoC 上实现了 **50k+ tokens/s**，但对应模型只有 **4,192 参数**，更偏 proof-of-concept / learning tool，而不是实用大模型推理平台。

## 这件事值得关注的点

- 它说明了“小模型 + 片上权重 + 专用 RTL”这条路线可以获得非常高的 token throughput。
- 真正的瓶颈不是纯算力，而是 **权重是否能放在片上、能否减少外部内存访问**。
- 原文提到如果坚持 16-bit 权重且尽量放片上，当前 FPGA 的片上 ROM/存储大致只能容纳 **20M 到 30M 参数**，这给 FPGA 适合承载的模型规模划出了一条现实边界。
- 因此这更像是 **SLM（small language model）/ 固定功能模型 / 低延迟边缘推理** 的潜在线索，而不是“FPGA 已经能直接替代 GPU 跑通用大模型”。

## 实操与复现判断

- 从公开材料看，它更像是“有完整工程 + 有架构说明”的项目，而不一定是对零基础完全手把手的 step-by-step 教程。
- 如果要自己复现，大概率需要具备：
  - DE1-SoC 板卡
  - Quartus / USB-Blaster / JTAG 基础环境
  - 基本 RTL、定点数、ROM 初始化、时序收敛知识
- 建议后续继续直接阅读 GitHub 仓库中的 README、工程目录和 build/program 说明，确认是否包含：
  - Quartus 工程文件
  - 权重转换脚本
  - board-specific 约束文件
  - bitstream 生成与烧录步骤

# 5. 1bitSDR：用 Lattice MachXO2 FPGA 做极简中波/短波 SDR 接收机

Hackaday.io 和 GitHub 都有该项目，Hackaday.io 上有原理说明、原理图和搭建说明。

## 直接链接

| 资源 | 地址 | 内容 |
|---|---|---|
| Hackaday.io 项目主页 | <https://hackaday.io/project/170916-fpga-3-r-1-c-mw-and-sw-sdr-receiver> | 工作原理、材料清单、项目更新和原理图附件 |
| 搭建说明 | <https://hackaday.io/project/170916/instructions> | UART 连接及晶振相关说明 |
| GitHub 工程 | <https://github.com/alberto-grl/1bitSDR> | MachXO2 FPGA 工程，以及 Steven Groom 的 Cyclone III 移植版 |
| 原理图 PDF | <https://cdn.hackaday.io/files/1709167312470144/1bitSDR.pdf> | 天线输入、音频输出和外部振荡器接线 |
| 作者 Hackaday.io 主页 | <https://hackaday.io/alberto.garlassi> | Alberto Garlassi 的个人资料及其他项目 |

GitHub 仓库信息已核实：`alberto-grl/1bitSDR`，Verilog 编写，Apache-2.0 协议，约 110 star / 17 fork，仓库内含 `AMDemod.v`、`CIC.v`、`Mixer.v`、`NCO.v`、`SinCos.v`、`PWM.v`、`Uart1.v` 等信号处理和 UART 模块，以及 Lattice Diamond 工程文件和一个 `SDR_CycloneIII` 移植目录。Hackaday.io 上的项目主页、搭建说明、原理图 PDF 和作者主页因本地网络策略未能直接抓取核实，以上内容依据用户提供的检索结果转录，复现前建议自行打开链接核对。

## 原理

项目目标是用尽可能少的元件接收中波、短波 AM 广播，不需要独立的传统 ADC 芯片。利用 FPGA 的 LVDS 输入实现一位（1-bit）采样，再在 FPGA 内完成混频、滤波、AM 解调和 PWM 音频输出。

## 最小硬件配置

作者列出的主要材料：

- Lattice MachXO2 Breakout Board
- 3 个 10 kΩ 电阻
- 1 个 220 pF 电容
- 扬声器及天线导线
- 可选的外部晶体振荡器；作者使用 8 MHz 振荡器，称其灵敏度及音质优于内部振荡器

原理图同时给出直接驱动扬声器和接有源音箱的低电平输出方案。外部晶振不是最低配置的必需品。

## 调台方式

通过电脑发送 UART 字符来控制 NCO、改变接收频率。原板卡的 USB 转串口第二通道需要连接到 FPGA；搭建说明要求在板底短接 R14、R15，将第二 UART 通道接到引脚 73、74。

注意：这是作者所用板卡的改接方式，不能直接套用到任意 MachXO2 开发板。复现前应先核对板卡型号、原理图和 FPGA 引脚约束。

## 阅读顺序与注意事项

先看 Hackaday.io 项目页了解结构，再看原理图和 Instructions，最后下载 GitHub 工程进行编译。作者在项目更新中表示 GitHub 托管了完整工程，应可用于综合和烧录，但这不代表已经验证它与手上的板卡或当前工具版本兼容。

- [1. 基于NTT的PQC乘法器的硬件实现](#1-基于ntt的pqc乘法器的硬件实现)
- [2. 推荐阅读](#2-推荐阅读)
  - [2.1 TCFPGA](#21-tcfpga)
- [3. 选型](#3-选型)
  - [3.1 赛灵思选型网站](#31-赛灵思选型网站)
- [4. Talos V2：在 FPGA 上跑 Karpathy 的 microGPT](#4-talos-v2在-fpga-上跑-karpathy-的-microgpt)


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

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
- [1.关于封装内光学 I/O 的三个常见误解](#1关于封装内光学-io-的三个常见误解)
- [2. Lizhenhao Paper](#2-lizhenhao-paper)
- [3. Wanglei Paper](#3-wanglei-paper)
- [4. Ayar Labs](#4-ayar-labs)
  - [4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)](#41-ayar-labs-暗示产品将在未来-2-3-年内出货-hpc-wire)
  - [4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)](#42-ayar-labs-旨在以光速消除人工智能的瓶颈-bloomberg-podcast)
- [5. Avicena](#5-avicena)
  - [5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》](#51high-bandwidth-gan-based-micro-leds-at-temperatures-up-to-400c)
- [6. 《廉价光源可使人工智能更节能》Nature](#6-廉价光源可使人工智能更节能nature)

<div STYLE="page-break-after: always;"></div>

# 1.关于封装内光学 I/O 的三个常见误解
随着光学 I/O 逐渐融入产品设计，一些误解浮现出来，可能会影响利益相关者对这项技术的理解和期望。让我们来解释并消除关于光学 I/O 的三个常见误解。

- 误解一：“共同包装很困难”
一些批评人士认为，封装内/共封装光学 I/O 具有挑战性，因为需要由从事设计、芯片制造、封装、测试、可靠性和认证等工作的多家公司组成的新生态系统。然而，这种观点忽视了过去几年共封装光学(CPO) 取得的重大进步。

    高度集成和一体式封装的解决方案已经达到了一定的成熟度和可靠性，使其能够进行大批量部署。例如，Broadcom 的 Tomahawk5 Bailey 就是一个成功的 CPO 平台的例子，展示了这些技术的可行性和准备就绪性。虽然集成新技术自然会带来复杂性，但该行业的进步表明了可行性以及不断增长的专业知识和标准化，这将促进更顺利、更轻松地采用。

- 误解二：“技术成熟得太晚了”
另一个常见的质疑是光学 I/O 技术的成熟时间表。一些批评人士断言，光学 I/O 解决方案（如 Ayar Labs 的 UCIe 光学小芯片）的推出太晚，无法影响预计在 2026-2027 年左右推出的下一代 AI 计算集群的部署。

    考虑到 Ayar Labs 的发展轨迹和里程碑，这种批评并不成立。自 2015 年以来，Ayar Labs 一直在该领域进行创新并开发光学芯片。UCIe 光学芯片是我们的第二代产品，它基于已经成熟的第一代 AIB 光学芯片的经验。这些 AIB 芯片已经在英特尔的 PIUMA、Stratix® 10 FPGA 和 Agilex™ FPGA 等平台上进行了演示。

    通过利用成熟的 AIB 电接口以及两代 CW-WDM 光接口，Ayar Labs 展示了其产品的持续发展和增强，并强调这些技术能够及时、有效地满足未来的需求。

- 误解三：“可插拔设备将是最优解决方案”
与某些人认为的可插拔光纤连接代表高性能计算的最佳解决方案相反，它们在 GPU 密集型环境中的应用凸显了重大缺陷。可插拔光纤非常适合长途电信，但由于带宽和延迟、功耗、物理密度和成本效益低下，因此不适合 GPU I/O 应用。仅就功耗而言，由于电信号和光信号之间的多次转换，<font color="red">可插拔光纤消耗约 30 皮焦耳/位 (pJ/b)</font>。这与直接连接两个封装的封装内光纤 I/O 解决方案形成了鲜明对比，<font color="red">功耗不到 5 pJ/b</font>，几乎节省了 6 倍的功耗。

    可插拔设备不仅效率低，而且体积庞大。与封装内光学 I/O 的相应指标相比，它们的边缘带宽密度低 10 倍以上，面积密度低 100 倍以上。这一限制严重限制了系统范围的带宽能力，表明该技术已接近其容量阈值。我们还必须考虑与可插拔设备相关的成本因素，它们的价格一直高得令人望而却步，每 Gbps 的价格为 1 至 2 美元，这使得扩展以满足未来的 AI 需求在经济上不可行。相比之下，集成封装内光学 I/O 解决方案可显著节省成本并提高性能。因此，光学 I/O 是下一代计算架构的最佳选择。

总之，光学 I/O 代表着一种变革性的转变，旨在克服 AI 基础设施中传统电气互连的带宽、延迟和能效限制。然而，将光学 I/O 集成到产品设计中需要仔细考虑和规划。通过解决当前 AI 架构中的挑战并消除对光学 I/O 的误解，公司可以做出明智的决策来扩展 AI 功能以满足未来的需求。

行业领先者已经展示了可行的高性能光互连，将光学 I/O 集成到产品设计中的未来道路清晰而有前景。

<https://ayarlabs.com/blog/ai-and-optical-io/?utm_content=302247967&utm_medium=social&utm_source=linkedin&hss_channel=lcp-6627049>

<div STYLE="page-break-after: always;"></div>

# 2. Lizhenhao Paper

《Bandwidth Analysis of High-Speed InGaN Micro-LEDs by an Equivalent Circuit Model》

- 实验装置：带宽测试系统主要由矢量网络分析仪（Keysight P5004A，9 kHz - 20 GHz）、直流电源、偏置T、射频探头（Cascade ACP40-GSG-150）、Si-PIN光电探测器（Alphalas UPD-50，7.0 GHz）和低噪声放大器（Pasternack PE15A3269，10至6000 MHz，34 dB增益）组成。图2（d）的插图显示了光学设置和透镜类型的测量图。微型LED晶圆紧密贴合在导热性良好的铜夹具上，其温度由TEC温控装置加热和稳定，以实现高温测试。
- Micro LED通信示，实验示意图
![system](/picture/2024-08-01%20124219.png)

- 偏置T，bias-T，示意图
  
![bias-T](/picture/BiasT_Banner_GIF_08-01-2023_OPTIMISED.webp)

<https://blog.minicircuits.com/rf-microwave-bias-tee-basics/>

- 半导体二极管中的载流子复合通常用电路中的一对并联电阻和电容来表示[19]，[20]。在模型中，有源区内的复合用RRec-in和CRec-in表示。有源区外的复合用RRec-out和CRec-out表示，它来自于载流子泄漏、溢出或从有源区逃逸的复合。Rs表示微型LED的串联电阻，CP表示微型LED的寄生电容，RL表示测试链路中的50°标准阻抗。

<div STYLE="page-break-after: always;"></div>

# 3. Wanglei Paper

《Green InGaN Quantum Dots Breaking through Efficiency and Bandwidth Bottlenecks of Micro-LEDs》

- 在制造高速 LED 后，进行了切割、引线键合和晶体管轮廓 (TO) 封装以测量调制带宽。图 5i 总结了不同电流密度下所有六个 LED 的 3 dB 调制带宽。所有六个样品的带宽都超过 650 MHz。较大的 LED 具有更高的输出功率但带宽较低。小于 125 µm 的 LED 的带宽超过 800 MHz。75 µm 高速微型 LED 的 3 dB 带宽在 226 A cm-2 的低电流密度下达到 1.12 GHz，50 µm 微型 LED 的带宽在相对较低的 509 A cm-2 电流密度下达到 1.3 GHz。图 5j 展示了 VW QD 绿色微型 LED 和其他报道的蓝色和绿色微型 LED 的调制带宽。可以看出，VW QD 的调制带宽比其他报道的绿色 LED 和蓝色极性 LED 更高，并且与非极性 LED 的最佳结果相当。

<div STYLE="page-break-after: always;"></div>

# 4. Ayar Labs

## 4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)

Ayar Labs 暗示，它即将发布其光学 I/O 技术来取代芯片内的铜线。该公司正在开发将光学 I/O 放入芯片结构中的技术，并已研究该技术十多年。该技术允许芯片内部实现更快的通信，旨在取代速度较慢的铜线。
可以肯定的是，Ayar Labs 首席执行官 Mark Wade 没有透露确切的发布日期，但提供了一些线索。他在彭博社的播客中表示，片上 I/O 市场将在 2026 年至 2028 年期间成熟。

韦德表示：“我们目前在实验室中与客户共同开展的工作，实际上是为了在两到三年后实现首次大规模市场部署。”

该技术将在2026年至2028年间达到转折点，出货量将达到数百万。

韦德表示：“2028 年以后，我们将其视为整个行业基础的广泛扩散。”

光学 I/O 广泛应用于长距离通信，但尚未用于短距离通信。Ayar Labs 正在将其光子技术置于芯片计算堆栈的顶层，从而提高各个层面的通信速度。

“我们已经完成了这项技术的所有科学实验。我们正着手设计制造，加快生产速度，加快部署速度，这是一个令人兴奋的阶段，但这确实需要时间，”韦德说。

AI 市场为 Ayar Labs 提供了突破。芯片和基础设施层面对更快通信的需求永无止境，但电气连接仅限于约 1.5 米的距离和最多 72 个 GPU 的机架。

借助光学 I/O，“你可以突破几十米甚至几百米的距离，然后连接更多的 GPU 或加速器，”Wade 说。

但发布一款产品并不像将其插入系统那么简单。光学 I/O 将改变芯片和服务器的部署方式，因此该公司正紧跟其合作伙伴的步伐，其中包括持有该公司股份的 Nvidia 和英特尔。

众所周知，铜线更便宜，而光学技术的能效也存在问题。韦德表示，Ayar Labs 正在以每美元每瓦吞吐量为衡量标准来衡量成本和能效，其中光学技术位居榜首。

Photonics 使系统和基础设施设计更加简单，降低了设备成本。总体而言，客户将获得更高的性价比和更快的产出。

韦德说：“你确实必须进入整个系统才能看到该指标如何改进。”

高性能计算市场中的一些人通过测量在功率范围内实现的生产力来定义可持续性。例如，使用人工智能来应对气候变化可能比比特币挖矿更能提高能源利用效率。

Nvidia 的 AI 重点还在于高效利用能源。Nvidia 的 GPU 包含自己的芯片技术，可降低功耗。该公司正在将 Hopper 上的空气冷却改为液体冷却。

该公司官员在播客中表示，该公司估计光子 IC 市场规模超过 380 亿美元。到本世纪末，该公司预计小芯片出货量将超过 1 亿。

过去两年，Ayar Labs 以惊人的速度申请了光学 I/O 专利，表明其商业化发布已近在眼前。Ayar 还试图收购Teraphy 商标。

<https://www.hpcwire.com/2024/07/31/ayar-labs-hints-at-product-shipment-in-next-2-3-years/?utm_content=302655617&utm_medium=social&utm_source=linkedin&hss_channel=lcp-6627049>

## 4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)

云端需要高性能的 AI 基础设施来支持日益增长的大型语言模型，这打开了性能瓶颈的潘多拉魔盒。Ayar Labs 首席执行官 Mark Wade 和商业运营副总裁 Terry Thorn 与彭博情报分析师 Woo Jin Ho 坐下来讨论 Ayar 的共封装硅光子技术，旨在颠覆传统的 AI 架构，并在快速发展的 AI 市场中超越当前的输入/输出技术浪潮。

2024 年 7 月 23 日

<https://www.bloomberg.com/news/audio/2024-07-23/ayar-labs-aims-to-eliminate-ai-s-bottlenecks-at-light-speed-tech-disruptors>

<div STYLE="page-break-after: always;"></div>

# 5. Avicena

## 5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》

Daniel J. Rogers; Haotian Xue; Fred A. Kish; Fu-Chen Hsiao;<font color=red> Bardia Pezeshki; Alexander Tselikov</font>; Jonathan J. Wierer

Gallium-nitride-based, blue micro-light-emitting diodes (micro-LEDs) with electro-optical -3 dB modulation bandwidths of <font color=red>3.73 GHz at 11 kA/cm 2 at room temperature</font> and <font color=red>4.00 GHz at 9 kA/cm 2 at 200°C </font>are reported. These bandwidths are the highest reported thus far for micro-LEDs. The micro-LEDs operate at high temperatures, up to 400°C, and bandwidths improve with increased temperatures. The lifetimes and recombination rates of the micro-LEDs active layer are determined by measuring and analyzing the impedance, modulation response, and radiative efficiency. This analysis shows increasing bandwidths with increasing current density and temperature resulting from dominant non-radiative lifetimes.

据报道，氮化镓基蓝色微型发光二极管 (micro-LED) 的电光 -3 dB 调制带宽 在室温下 为 3.73 GHz，在 11 kA/cm 2下为 3.73 GHz，在 200°C 下为 9 kA/cm 2下为 4.00 GHz。这些带宽是迄今为止报道的微型 LED 的最高带宽。微型 LED 在高达 400°C 的高温下工作，并且带宽会随着温度升高而提高。通过测量和分析阻抗、调制响应和辐射效率来确定微型 LED 有源层的寿命和复合率。该分析表明，由于占主导地位的非辐射寿命，带宽会随着电流密度和温度的增加而增加。

<https://ieeexplore.ieee.org/abstract/document/10613856>

<div STYLE="page-break-after: always;"></div>

# 6. 《廉价光源可使人工智能更节能》Nature

随着人工智能 (AI) 算法迅速成为日常生活中不可或缺的一部分，人们对训练和运行这些算法所需的大量能源产生了担忧1。实现更节能的 AI 的方法之一是用模拟元件替换传统数字计算机的某些部分。称为光子张量处理单元的设备依靠光来执行机器学习算法所需的矩阵乘法运算2，并且是这条道路上的关键一步。其中一些单元已经在使用3、4，但要在不大幅增加其尺寸的情况下增加它们所包含的组件数量 5 是一项挑战。Dong等人6在《自然》杂志上撰文提出了一种解决方案——一种利用廉价、高效的发光二极管 (LED) 产生的低质量光的计算机架构。

<https://www.nature.com/articles/d41586-024-02323-7>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Partial%20coherence%20enhances%20parallelized%20photonic%20computing.pdf>

光驱动人工智能的“改变游戏规则”的新发现

在《自然》杂志上发表的一篇题​​为“部分相干性增强并行光子计算”的论文中，牛津大学的研究人员与明斯特大学、海德堡大学和根特大学的合作者报告说，用不太复杂的光源代替激光器可以令人惊讶地提高某些光学应用的性能，例如光驱动的人工智能技术。

这一发现为更便宜、能耗更低的光源开辟了道路，这些光源可用于通常依赖昂贵、高规格激光器的应用。

光源的特性通常用物理学家称为相干性的量来描述：光波在时间和空间上的一致程度。低相干性光源（例如太阳和灯泡）发出各种颜色（或波长）的光。

另一方面，高质量工程光源（如激光器）具有非常窄的波长范围并且通常呈现单一颜色。

设计和使用高相干光（激光）的能力一直是光通信、光检测和测距 (LiDAR) 遥感技术以及医学成像技术等现代应用的基础。因此，人们自然而然地认为，使用更相干的光源可以增强系统性能和设备功能，例如，通过实现更高的分辨率和更精确的测量。

这一新发现挑战了这一传统观念，并揭示了低相干光源在特定情况下实际上可以发挥更好的作用，例如光子人工智能加速器——一种使用光子代替电子来执行人工智能计算的新兴技术。

该团队利用部分相干光源，利用电泵浦掺铒光纤放大器（一种用于光通信的装置，用于增强通过光纤传播的光信号的强度）产生的非相干光光谱的窄部分。

这种部分相干光被均匀地分割并分配到并行人工智能计算阵列的不同输入通道中。使用这样的光源，在具有 N 个输入通道的光子加速器中，人工智能计算的并行性惊人地提高了 N 倍。

作为测试案例，团队使用该系统通过分析患者的行走方式来识别帕金森病患者，分类准确率达到 92% 以上。

该团队还演示了如何使用一个具有 9 个输入通道的部分相干光源的简单系统来执行每秒约 1000 亿次操作的高速 AI 任务。通常，这样的速度（相当于在一秒钟内播放两个多小时的 4K 视频）只能在具有多个独立相干激光器的相干光子 AI 加速器中实现。

最终，消除添加额外光源的需要可能会对提高计算能力产生变革性的影响，正如第一作者、牛津大学材料系的董博伟博士所解释的那样，“使用‘较差’光源的好处具有扩展效应。如果光子加速器扩展到 100 个输入通道，那么与激光系统相比，你可以将 AI 模型的运行速度提高 100 倍。”

领导这项工作的牛津大学材料系兼 Salience Labs 联合创始人 Harish Bhaskaran 教授表示：“虽然这项工作展示了这种部分相干光在光子计算一些新兴领域的应用，但我们未来还将研究这种见解是否适用于光通信，特别是在新兴的光互连技术领域。

“这是一个快速发展的研究领域，有很多有趣的科学和工程值得探索。”

<https://phys.org/news/2024-08-game-discovery-driven-artificial-intelligence.html>

<div STYLE="page-break-after: always;"></div>
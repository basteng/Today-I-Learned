- [1.关于封装内光学 I/O 的三个常见误解](#1关于封装内光学-io-的三个常见误解)
- [2. Lizhenhao Paper](#2-lizhenhao-paper)
  - [2.1 《Bandwidth Analysis of High-Speed InGaN Micro-LEDs by an Equivalent Circuit Model》](#21-bandwidth-analysis-of-high-speed-ingan-micro-leds-by-an-equivalent-circuit-model)
  - [2.2 《High-Speed Micro-LEDs based on Nano-Engineered InGaN Active Region towards Chip-to-Chip Interconnections》](#22-high-speed-micro-leds-based-on-nano-engineered-ingan-active-region-towards-chip-to-chip-interconnections)
- [3. Wanglei Paper](#3-wanglei-paper)
- [4. Ayar Labs](#4-ayar-labs)
  - [4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)](#41-ayar-labs-暗示产品将在未来-2-3-年内出货-hpc-wire)
  - [4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)](#42-ayar-labs-旨在以光速消除人工智能的瓶颈-bloomberg-podcast)
  - [4.3 光学 I/O 如何助力生成式 AI 的未来：与 Vladimir Stojanovic 的访谈](#43-光学-io-如何助力生成式-ai-的未来与-vladimir-stojanovic-的访谈)
- [5. Avicena](#5-avicena)
  - [5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》](#51high-bandwidth-gan-based-micro-leds-at-temperatures-up-to-400c)
  - [5.2 硅光子学联合封装。 凉！ 但它实用吗？Bardia Pezeshki post at Linkedin](#52-硅光子学联合封装-凉-但它实用吗bardia-pezeshki-post-at-linkedin)
  - [5.3 Techopedia 专访 Bardia Pezeshki](#53-techopedia-专访-bardia-pezeshki)
    - [5.3.1 计算挑战：能源、处理能力和低延迟](#531-计算挑战能源处理能力和低延迟)
    - [5.3.2 “用光说话的芯片”](#532-用光说话的芯片)
    - [5.3.3 长距离光子学与短距离通信](#533-长距离光子学与短距离通信)
    - [5.3.4 用例和应用：现实生活中的光子学](#534-用例和应用现实生活中的光子学)
    - [5.3.5 底线](#535-底线)
- [6. 《廉价光源可使人工智能更节能》Nature](#6-廉价光源可使人工智能更节能nature)
- [7. 多孔硅](#7-多孔硅)
- [8. -3 dB带宽](#8--3-db带宽)
- [9. LED和LD光调制的区别](#9-led和ld光调制的区别)
- [10.模拟光纤通信相关知识](#10模拟光纤通信相关知识)
  - [10.1 LED光通信背景知识](#101-led光通信背景知识)
  - [10.2 LED调制带宽](#102-led调制带宽)
- [11. PCIe诞生20年来最大变革！引入光学传输](#11-pcie诞生20年来最大变革引入光学传输)
- [12.厦门大学与阳明交大研发红/黄光Micro LED光通信技术](#12厦门大学与阳明交大研发红黄光micro-led光通信技术)
- [13.蓝色GaN/InGaN量子阱发光晶体管的特性 2023IRDS\_BC 3.3.8 Transistor Laser](#13蓝色ganingan量子阱发光晶体管的特性-2023irds_bc-338-transistor-laser)
- [14.你也可以使用 LED 作为传感器](#14你也可以使用-led-作为传感器)
- [15.如何使用 LED 检测光](#15如何使用-led-检测光)
- [16. 光子学与人工智能：行业观点](#16-光子学与人工智能行业观点)
- [17. Bechtolsheim在Hotchips上关于Micro LED进展的讨论](#17-bechtolsheim在hotchips上关于micro-led进展的讨论)
- [18.光学](#18光学)
  - [18.1 新型微芯片装置可产生多种激光色调](#181-新型微芯片装置可产生多种激光色调)
  - [18.2 片上光源可产生多种波长范围](#182-片上光源可产生多种波长范围)
  - [18.3 微型新型激光器填补了可见光彩虹色的长期空白，开辟了新的应用](#183-微型新型激光器填补了可见光彩虹色的长期空白开辟了新的应用)
- [19. Recent progress on micro-LEDs - Nanowire](#19-recent-progress-on-micro-leds---nanowire)
- [20. Data communication using blue GaN-on-Si micro-LEDs reported on a 200-mm Silicon substrate 格勒诺布尔大学](#20-data-communication-using-blue-gan-on-si-micro-leds-reported-on-a-200-mm-silicon-substrate-格勒诺布尔大学)
- [21. 注入电流对量子点发光二极管调制带宽的影响](#21-注入电流对量子点发光二极管调制带宽的影响)
- [22.Nonpolar m -Plane InGaN/GaN Micro-Scale Light-Emitting Diode With 1.5 GHz Modulation Bandwidth - 非极性面 - 美国新墨西哥州阿尔伯克基新墨西哥大学高科技材料中心](#22nonpolar-m--plane-ingangan-micro-scale-light-emitting-diode-with-15-ghz-modulation-bandwidth---非极性面---美国新墨西哥州阿尔伯克基新墨西哥大学高科技材料中心)
- [23. Arista](#23-arista)
  - [23.1 Andy Bechtolshelm：](#231-andy-bechtolshelm)
- [24.数据中心交换芯片](#24数据中心交换芯片)
- [25. 初创公司](#25-初创公司)
  - [25.1 Lightwave](#251-lightwave)
  - [25.2 POET](#252-poet)
- [26. RC-LED](#26-rc-led)
  - [26.1 可见光共振腔发光二极管原理及发展概况 - 北工大](#261-可见光共振腔发光二极管原理及发展概况---北工大)

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

# 2. Lizhenhao Paper

## 2.1 《Bandwidth Analysis of High-Speed InGaN Micro-LEDs by an Equivalent Circuit Model》

- 实验装置：带宽测试系统主要由矢量网络分析仪（Keysight P5004A，9 kHz - 20 GHz）、直流电源、偏置T、射频探头（Cascade ACP40-GSG-150）、Si-PIN光电探测器（Alphalas UPD-50，7.0 GHz）和低噪声放大器（Pasternack PE15A3269，10至6000 MHz，34 dB增益）组成。图2（d）的插图显示了光学设置和透镜类型的测量图。微型LED晶圆紧密贴合在导热性良好的铜夹具上，其温度由TEC温控装置加热和稳定，以实现高温测试。
- Micro LED通信示，实验示意图
![system](/picture/2024-08-01%20124219.png)

- 偏置T，bias-T，示意图
  
![bias-T](/picture/BiasT_Banner_GIF_08-01-2023_OPTIMISED.webp)

<https://blog.minicircuits.com/rf-microwave-bias-tee-basics/>

**半导体二极管中的载流子复合通常用电路中的一对并联电阻和电容来表示[19]，[20]。在模型中，**
  
- 有源区内的复合用RRec-in和CRec-in表示
- 有源区外的复合用RRec-out和CRec-out表示，它来自于载流子泄漏、溢出或从有源区逃逸的复合
- Rs表示微型LED的串联电阻
- CP表示微型LED的寄生电容
- RL表示测试链路中的50°标准阻抗

![image](/picture/circuit%20model%20InGaN%20LEDs.png)



## 2.2 《High-Speed Micro-LEDs based on Nano-Engineered InGaN Active Region towards Chip-to-Chip Interconnections》

高速微尺度发光二极管（micro-LED）技术在短距离数据传输中的应用突破了传统电连接的限制，在大容量高速通信需求愈加迫切的今天，这一点尤为重要，而高速微LED光源是其中的关键部件。本工作采用交替生长中断法生长出尺寸更小、密度更高的三层InGaN纳米结构，该方法提高了局部载流子浓度，降低了差分载流子寿命。基于三层改进的InGaN纳米结构，设计并制作了蓝光微LED，实现输出光功率超过0.5mW，电-电（EE）-3dB带宽超过2.6GHz。利用该高速微型 LED 作为光源，演示了三种非归零开关键控 (NRZ-OOK) 实时通信系统：通过自由空间和石英光纤的单通道传输，以及通过塑料成像光纤的 4 通道传输，分别实现了 3.07、2.60 和 12.00 Gbps 的数据速率。此外，4 通道系统实现了 15.05 Gbps 的比特功率加载离散多音 (DMT) 传输。

<https://ieeexplore.ieee.org/document/10637686>

# 3. Wanglei Paper

《Green InGaN Quantum Dots Breaking through Efficiency and Bandwidth Bottlenecks of Micro-LEDs》

- 在制造高速 LED 后，进行了切割、引线键合和晶体管轮廓 (TO) 封装以测量调制带宽。图 5i 总结了不同电流密度下所有六个 LED 的 3 dB 调制带宽。所有六个样品的带宽都超过 650 MHz。较大的 LED 具有更高的输出功率但带宽较低。小于 125 µm 的 LED 的带宽超过 800 MHz。75 µm 高速微型 LED 的 3 dB 带宽在 226 A cm-2 的低电流密度下达到 1.12 GHz，50 µm 微型 LED 的带宽在相对较低的 509 A cm-2 电流密度下达到 1.3 GHz。图 5j 展示了 VW QD 绿色微型 LED 和其他报道的蓝色和绿色微型 LED 的调制带宽。可以看出，VW QD 的调制带宽比其他报道的绿色 LED 和蓝色极性 LED 更高，并且与非极性 LED 的最佳结果相当。

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

## 4.3 光学 I/O 如何助力生成式 AI 的未来：与 Vladimir Stojanovic 的访谈

2023 年 11 月 8 日

显然，2023 年是生成式人工智能的一年，人们对 ChatGPT 等新型大型语言模型 (LLM) 的兴趣激增。许多公司正在将人工智能融入其服务中（例如 Microsoft Bing、Google Bard、Adobe Creative Cloud 等），这无疑对NVIDIA今年的股价产生了重大影响。

当我们展望人工智能的未来及其面临的挑战时，谁能比 Ayar Labs 的首席架构师兼联合创始人 Vladimir Stojanovic 提供更好的见解呢？在这次问答采访中，我们向 Vladimir 提出了十几个问题，关于 Ayar Labs 的技术如何促进生成式人工智能的发展。

1. 从架构的角度来看，公司在持续发展和提高人工智能模型的性能方面面临哪些挑战，特别是在生成式人工智能的背景下？

生成式 AI 模型的关键在于它们非常庞大，需要跨多个 GPU 进行全局通信——而不仅仅是数据中心的单个机箱或机架。即使是推理（即推理和做出决策），要求也很高，微调和训练的要求就更高了。大致的规模是这样的：一个机架用于推理，数十个机架用于微调，数百个机架用于训练。无论如何，你必须将所有这些 GPU 互连起来。

2. 互连 GPU 的关键考虑因素是什么？

上述生成式 AI 架构中互连的作用是提供从每个 GPU 到其他每个 GPU 或子系统的全局通信，以完整的 GPU I/O 带宽和低延迟，最大限度地提高处理效率，同时功耗、面积和成本占用空间可忽略不计。基本上，它使分布式系统看起来像一个巨大的虚拟 GPU。因此，互连必须非常快速、密集且节能和经济高效。这就是 Ayar Labs 致力于商业化光学输入/输出 (I/O) 的原因：它使用硅光子学在芯片级集成光学连接，直接从 GPU (XPU) 封装中产生最快、最高效的互连。

3. 目前正在使用什么？为什么它不是最理想的？

目前，这些系统依赖于可插拔光纤连接，这本质上是一种光纤网络技术。可插拔光纤连接非常适合长途应用，如电信，但不适合板载输入/输出。

可插拔式 GPU I/O 在所有四个方面均不合格：带宽/延迟、功率、密度和成本。基于可插拔式 GPU 到 GPU 链路（或 GPU 到外部交换机链路）每比特消耗约 30 皮焦耳 (pJ/b)：初始电气 GPU 到光学可插拔链路消耗 5pJ/b，光学可插拔到光学可插拔链路消耗 20pJ/b，再从光学可插拔转换回电气 GPU 或交换机消耗 5pJ/b。将此 30pJ/b 与封装内光学 I/O 解决方案进行比较，后者直接连接两个封装，消耗不到 5pJ/b — 从而节省近 8 倍的功耗。

可插拔模块也是体积庞大的模块。与封装内光学 I/O 相比，它们的边缘带宽密度要低 10 倍以上，面积密度要低 100 倍以上。这限制了 GPU 卡或机箱可以传输到系统其余部分的带宽。基本上，今天我们或多或少已经达到极限，也许可以再挤一代，直到系统完全出现瓶颈。

最后但并非最不重要的是成本。由于可插拔模块是外部模块而不是板载芯片，因此其成本扩展性很差——多年来徘徊在 1-2 美元/Gbps 之间。为了实现未来生成式 AI 系统性能扩展所需的 GPU-GPU 带宽扩展，此成本需要降低大约 10 倍。封装内光学 I/O 可以通过光学芯片端和激光器端的集成来帮助实现这些成本节省。

4. 您能谈谈对训练和推理的影响吗？您认为光学 I/O 最大的优势是什么？

如上所述，有三个应用程序，每个应用程序的占用空间和容量都不同。首先，你要训练一个人工智能模型，然后对其进行微调（这可以是持续的），然后通过推理将其投入生产。考虑到模型扩展趋势——从当前最大的模型到下一代或两代，推理将需要 10-100 个 GPU，微调 100-1,000 个 GPU，并训练数千到数万个 GPU。考虑到一个机箱最多可容纳 8 个 GPU，而一个机架可容纳 32 个 GPU，即使是推理也将成为需要光学 I/O 的机架规模操作。

5. 您能否解释一下系统工程师在设计大规模 AI 工作负载时面临的主要挑战，以及光学 I/O 如何应对这些挑战？

首先，让我们明确一下我们在谈论谁。如果我们指的是机器学习 (ML) 程序员，那么具有光学 I/O 的平台将提供具有高吞吐量扩展、低延迟性能和低延迟分布的结构解决方案。这些因素结合起来，使整个分布式计算操作看起来尽可能像一个虚拟 GPU，从而提高程序员的生产力并实现可扩展的 ML 工作负载。

如果我们谈论的是需要构建支持高度可扩展分布式计算的平台的硬件设计师，那么光学 I/O 可以实现物理分解。这是使用更小的组件构建复杂、高度可扩展且成本扩展性更强的平台的关键。未来的设计可以围绕一堆物理分解的 GPU 计算或交换卡之类的东西构建，而不需要复杂且昂贵的多 GPU 机箱。

6. 您如何看待未来五到十年在人工智能模型增长和能源消耗的背景下光学 I/O 技术的作用将如何演变？

光学 I/O 的路线图实现了十多年的持续带宽和功率扩展，从而实现了强大的分布式计算平台扩展和相应的模型增长。

7. “全连接”与生成式 AI 场景中的统一延迟和总体效率有何关系？光学 I/O 在这方面有何帮助？

在生成式 AI 所需的极大规模（例如数千个计算插槽）上，必须通过交换结构实现全对全连接。这必须分布在所有计算插槽上（例如在基于 TPU 的系统中），或与计算插槽分开（例如在基于 GPU 的系统中）。无论哪种情况，光学 I/O 都能以低功耗和低成本提供充足的带宽和较低的每链路延迟。这允许在计算/交换机插槽和结构拓扑（即所谓的胖树（或折叠 Clos）设计）之外直接实现大量不受距离影响的光学连接，从而提供短而均匀的延迟，而不会影响注入带宽（节点将数据注入网络的速率）或二分带宽（真实整体网络带宽的计算）。目前，现有的结构设计通过使用更少的光学可插拔连接来在结构成本和性能之间进行折衷 - 例如，通过减少与胖树设计中的计算节点的注入容量相比的对分带宽，或者通过使用替代结构拓扑（例如TPU系统中的环面），这最大限度地减少了机架和行级光学连接的数量，但引入了不均匀的延迟配置文件，这再次限制了应用程序的性能。

8. 您能否详细说明光学 I/O 技术在可重构性中的作用，特别是在适应不断发展的 AI 模型要求方面，以及这种灵活性如何影响系统级效率？

封装内光学 I/O 可实现高带宽和计算/交换机封装外的大量端口（链路），从而为如何配置结构以满足不断发展的模型要求提供了灵活性。例如，系统设计可以强调更高的基数（更多链路），从而根据需要增加节点数量，以支持更大模型张量并行性和更低延迟。或者，它可以强调每个链路的更高吞吐量，以通过流水线并行性实现更低的传输延迟。

9. 考虑到人工智能应用的边缘计算趋势，光学 I/O 技术在资源受限的边缘设备中提供高速连接面临哪些独特的挑战和机遇？

由于边缘设备可用的资源有限，因此物理分解是一个关键考虑因素，也是光学 I/O 提供的主要优势之一。例如，航空航天公司正在寻求将下一代传感器与底层计算分解，以重新平衡关键约束（例如尺寸、重量和功率），同时还启用解决距离（超过一米）问题的新传感配置（例如多静态雷达、合成孔径、协作 MIMO 通信等）。

10. 光学 I/O 可以带来哪些潜在的 AI 性能提升？

我们一直在创建和评估平台开发，这些平台在机箱、机架和系统层面都有可能在下一代将结构吞吐量扩大 10 倍以上。这使得互连带宽能够跟上 GPU 改进和 AI 集群横向扩展趋势，确保连接性不会成为未来 AI 发展的制约因素。

11. 随着光学 I/O 的成熟，标准化、互操作性和生态系统开发的关键考虑因素是什么，以确保其广泛采用并与各种生成式 AI 硬件和软件框架兼容？

标准化对于整个生态系统的发展和繁荣至关重要，而标准化必须以光学 I/O 作为核心考虑因素。这里有两个要素：物理和软件。

在物理层，有连接本身和为光学器件供电的激光。UCIe（通用芯片互连快递）是业界在封装级通用互连方面正在整合的标准，结合了来自可互操作、多供应商生态系统的一流芯片间互连和协议连接。

对于激光器，CW-WDM MSA（连续波波分复用多源协议）是行业倡议和规范，旨在标准化 O 波段的 WDM CW 源，以用于新兴的先进集成光学应用，例如 AI、HPC 和高密度光学，这些应用预计将转向 8、16 和 32 个波长。

与其他物理层互连技术相比，这两项举措都实现了性能、效率、成本和带宽扩展的飞跃。

在软件层，未来取决于 CXL（Compute Express Link）等协议，这是用于处理器、内存和加速器缓存一致性互连的开放标准。这可以实现池化或交换内存等先进技术，为 GPU 利用物理层的高吞吐量和低延迟来共享分散内存提供基础。

12. 在技能和专业知识方面，进入人工智能光学 I/O 开发领域的专业人员需要具备哪些关键资格和知识领域，公司和教育机构如何相应地培养劳动力？

这是一个具有挑战性的多学科问题，涉及整个堆栈，从硅光子学和激光的物理学到电路设计和计算机/网络架构（加上制造和封装），更不用说分布式计算/共享内存系统的系统编程/通信堆栈。公司、个人和教育机构可以通过认识和强调这种跨堆栈设计方法来做好准备。

<https://ayarlabs.com/blog/how-optical-i-o-is-enabling-the-future-of-generative-ai-a-qa-with-vladimir-stojanovic/>


# 5. Avicena

## 5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》

Daniel J. Rogers; Haotian Xue; Fred A. Kish; Fu-Chen Hsiao;<font color=red> Bardia Pezeshki; Alexander Tselikov</font>; Jonathan J. Wierer

Gallium-nitride-based, blue micro-light-emitting diodes (micro-LEDs) with electro-optical -3 dB modulation bandwidths of <font color=red>3.73 GHz at 11 kA/cm 2 at room temperature</font> and <font color=red>4.00 GHz at 9 kA/cm 2 at 200°C </font>are reported. These bandwidths are the highest reported thus far for micro-LEDs. The micro-LEDs operate at high temperatures, up to 400°C, and bandwidths improve with increased temperatures. The lifetimes and recombination rates of the micro-LEDs active layer are determined by measuring and analyzing the impedance, modulation response, and radiative efficiency. This analysis shows increasing bandwidths with increasing current density and temperature resulting from dominant non-radiative lifetimes.

据报道，氮化镓基蓝色微型发光二极管 (micro-LED) 的电光 -3 dB 调制带宽 在室温下 为 3.73 GHz，在 11 kA/cm 2下为 3.73 GHz，在 200°C 下为 9 kA/cm 2下为 4.00 GHz。这些带宽是迄今为止报道的微型 LED 的最高带宽。微型 LED 在高达 400°C 的高温下工作，并且带宽会随着温度升高而提高。通过测量和分析阻抗、调制响应和辐射效率来确定微型 LED 有源层的寿命和复合率。该分析表明，由于占主导地位的非辐射寿命，带宽会随着电流密度和温度的增加而增加。

<https://ieeexplore.ieee.org/abstract/document/10613856>

这篇文章一共七个作者

1. Daniel J. Rogers
Department of Electrical and Computer Engineering, North Carolina State University, Raleigh, NC, USA

Daniel Rogers 于 2020 年获得 Seton Hall 物理学学士学位。他目前正在北卡罗来纳州立大学攻读博士学位。他目前正在研究 III-氮化物发光体。

2. Haotian Xue
Department of Electrical and Computer Engineering, North Carolina State University, Raleigh, NC, USA

薛浩天于 2020 年获得中国科学技术大学应用物理学学士学位和美国利哈伊大学电气工程硕士学位。他目前正在北卡罗来纳州立大学攻读博士学位，研究用于功率器件和发光器的 III 族氮化物半导体的生长。

3. Fred A. Kish
Department of Electrical and Computer Engineering, North Carolina State University, Raleigh, NC, USA

Fred A. Kish 分别于 1988 年、1989 年和 1992 年获得伊利诺伊大学香槟分校电气工程学士、硕士和博士学位。他的博士研究工作（在 Nick Holonyak, Jr. 的指导下）是核心含铝 III-V 原生氧化物技术的一部分，该技术推动了最高性能 VCSEL 的开发，并已授权给世界各地的 VCSEL 制造商。1992年至 1999 年，他在惠普公司共同发明并领导了当时生产的最高性能（效率）红橙黄色可见光 LED（晶圆粘合透明基板 AlGaInP LED）的商业化。这些设备的效率超过了白炽灯和卤素灯，基于该技术的产品迄今为止已带来超过 20 亿美元的收入。 1999 年至 2001 年，他担任安捷伦科技公司的 III-V 部门经理。2001年，他加入 Infinera 公司，在那里他共同发明并领导了第一款实用（商业部署）大规模 PIC 和第一款用于光通信的商用全集成片上系统的研究、开发和商业化工作。大规模 InP PIC 是 Infinera 光网络产品的核心，是 PIC 网络产品销售额超过 50 亿美元的推动技术。在加入北卡罗来纳州立大学担任北卡罗来纳州立大学纳米制造设施主任之前，他曾担任 Infinera 光学集成电路集团高级副总裁。Kish博士是美国国家发明家学会、Optica（前身为 OSA）和 IEEE 的院士，也是美国国家工程院院士。他获得的奖项包括 IEEE David Sarnoff 奖、IEEE 光子学会量子电子学奖、IEEE LEOS 工程成就奖、OSA Adolph Lomb 奖和国际复合半导体研讨会青年科学家奖。他合著了 135 多项美国专利、170 多篇同行评审期刊和会议出版物以及 5 篇关于光电器件和材料的书籍章节。

<https://ece.ncsu.edu/people/fakish/>

4. Fu-Chen Hsiao
Department of Electrical and Computer Engineering, North Carolina State University, Raleigh, NC, USA

Fu-Chen Hsiao 于 2010 年获得台湾台北国立台湾师范大学物理学学士学位，2012 年获得台湾台南国立成功大学光子学硕士学位，2021 年获得伊利诺伊大学厄巴纳-香槟分校电气工程博士学位。在加入北卡罗来纳州立大学教职员工之前，他是北卡罗来纳州立大学电气与计算机工程系的博士后研究员。Hsiao的研究重点是半导体材料和器件物理。他的研究包括半导体和纳米结构的电子、光学和传输特性建模、光子集成电路和半导体光电器件。目前，他的工作主要围绕研究 III-氮化物基异质结构中的非辐射复合过程以实现高速高效 LED，以及高温高效 III-As/P 激光二极管的设计。他还致力于基于宽带隙半导体的可见光范围内宽谱光子集成电路的开发。

<https://ece.ncsu.edu/people/fhsiao/>

5. Bardia Pezeshki
Avicena Tech Corporation, Sunnyvale, CA, USA

Bardia Pezeshki（IEEE 高级会员）于 1991 年获得美国加利福尼亚州斯坦福大学电气工程博士学位。此后，他曾在 IBM 和 SDL（现为 Lumentum）担任研究职位，并创立了三家初创公司，第一家制造用于长距离电信的可调激光器，第二家制造用于数据中心应用的 40 和 100 Gb/s 光收发器。他最新的初创公司 AvicenaTech Corporation 位于美国加利福尼亚州桑尼维尔，旨在开发用于芯片间数据互连的光通信。

<https://ieeexplore.ieee.org/author/37090014116>

6. Alexander Tselikov
Avicena Tech Corporation, Sunnyvale, CA, USA

7. Jonathan J. Wierer
Department of Electrical and Computer Engineering, North Carolina State University, Raleigh, NC, USA

Wierer 博士的研究兴趣包括半导体器件物理和半导体材料科学。具体来说，他对研究具有宽带隙半导体的电子和光电子器件感兴趣。他于 1999 年毕业于伊利诺伊大学香槟分校，获得电气工程博士学位，师从 Nick Holonyak, Jr。在加入北卡罗来纳州立大学之前，Wierer 博士曾在 Philips-Lumileds、桑迪亚国家实验室和利哈伊大学工作。在 Lumileds 高级实验室，他的研究重点是新型 III 族氮化物发光二极管 (LED)。这包括开发第一款高功率（1 瓦）倒装芯片 III 族氮化物 LED 和 III 族氮化物光子晶体 LED 的开创性工作。在桑迪亚国家实验室，他的兴趣扩展到其他 III 族氮化物研究领域，包括太阳能电池、子带间器件、层混合、电力电子器件、紫外 LED 和纳米线 LED。他最引人注目的工作是提出将激光二极管作为固态照明的超高效光源。Wierer 博士撰写或与他人合作撰写了 200 多篇期刊出版物和会议报告，并拥有 42 项专利，主要与 III 族氮化物器件有关。他是 IEEE Photonics Technology Letters 期刊的高级编辑和 IEEE Journal of Quantum Electronics 的副主编。他是光学学会院士和电气电子工程师学会的高级会员。

<https://ece.ncsu.edu/people/jjwierer/>

## 5.2 硅光子学联合封装。 凉！ 但它实用吗？Bardia Pezeshki post at Linkedin
Silicon Photonics Co-packaging. Cool! but is it practical?

Back in 2017, my old company Kaiam arguably started this, with a demo at OFC with Corning of a 1.6Tb/s module. We called it CoPPhI back then and Rob Kalman and I gave a number of talks and seminars proselytizing the approach.. But boy was it hard! I think it still is.

But there is a much better way now. Turns out you don't need lasers if you don't want to go far. And the bottleneck for AI/memory/processors is really only a few meters. GaN LEDs can do speeds greater than 10Gb/s, and the display world knows how to put millions on them on any silicon (with transistors!). 

Compared to laser based CPO: LED based links don't go far, but
* no tight single mode coupling - (50um diameter fibers)
* runs at high temp - recent paper went to 400C!
* super reliable - unlike VCSELs - and no need for an external lightsource
* no modal noise issues, isolators needed, polarization problems, bit-error-rate floors due ultimately to speckle
* silicon detectors are amazing in the blue - can even do APDs and piggy back on CIS processors for cameras
* much lower power and massive density (pJ/bit and Tb/s per mm)
* fundamentally wide bus (Hey, clock speeds of chips haven't improved in decades - this is fundamentally what chip guys want) 
* And super low cost!

As we have played with this technology over the last few years at Avicena, we've become more and more convinced this will find its way into cables, board mounted optics, chiplets, and ultimately on the chips themselves - in your AI HPC, servers, laptops, even cell phones.

Definitely not as sexy as lasers - but way more practical.

硅光子学联合封装。 凉！ 但它实用吗？

早在 2017 年，我的老公司 Kaiam 就可以说开始了这项工作，在 OFC 上与康宁一起演示了 1.6Tb/s 模块。 我们当时称之为CoPPhI，Rob Kalman和我做了一些演讲和研讨会，宣传这种方法。但是男孩，这很难吗！ 我认为它仍然是。

但现在有更好的方法。 事实证明，如果你不想走得太远，你就不需要激光。 而AI/内存/处理器的瓶颈其实只有几米。 氮化镓 LED 的速度可以超过 10Gb/s，显示世界知道如何在任何硅片（使用晶体管）上放置数百万美元。 

与基于激光的 CPO 相比：基于 LED 的链接走不远，但
* 无紧密单模耦合 - （50um 直径光纤）
* 在高温下运行 - 最近的纸张达到了 400C！
* 超级可靠 - 与 VCSEL 不同 - 无需外部光源
* 无模态噪声问题，无需隔离器，出现极化问题，最终由散斑导致的误码率基底
* 硅探测器在蓝色中令人惊叹 - 甚至可以执行 APD 并搭载在相机的 CIS 处理器上
* 更低的功率和大密度（pJ/bit 和 Tb/s/mm）
* 从根本上说是宽总线（嘿，芯片的时钟速度几十年来没有提高 - 这基本上是芯片专家想要的）
* 而且成本超低！

在过去的几年里，当我们在Avicena使用这项技术时，我们越来越相信这将进入电缆、板载光学器件、小芯片，并最终出现在芯片本身——你的人工智能高性能计算、服务器、笔记本电脑，甚至手机中。

绝对不像激光那样性感 - 但更实用。

**回帖汇总**

Tom Collins ：Surely the problem with only 10Gb/s per fiber is how to get enough fibers attached to the silicon? 
当然，每根光纤只有 10Gb/s 的问题是如何让足够的光纤连接到硅上？ 

Bardia Pezeshki:very large arrays of fibers are available for applications such as imaging and illumination. Currently we use bundles of 50um fibers which at 10Gbs gives you a density of 4Tb/s per mm^2. We have samples of 3mm×5mm fiber arrays of 10um diameter that would give total BW of 1000 Tb/s. See some of our papers/videos.
超大的光纤阵列可用于成像和照明等应用。目前，我们使用 50um 光纤束，在 10Gbs 时，密度为每 mm^2 4Tb/s。我们有直径为 10um 的 3mm×5mm 光纤阵列样本，总带宽为 1000 Tb/s。请观看我们的一些论文/视频。

Martijn Heck:As a scientist, I think every credible alternative that challenges the existing paradigms is very interesting. I think we need to keep in mind that all these approaches, whether PIC, VCSEL or LED based, are still in their infancy, and, as a result, need to target requirements of 2034 rather than 2024... that means typically 30X nowadays' bandwidth, bandwidth density and energy efficiency (so <100 fJ/b). 
作为一名科学家，我认为每一个挑战现有范式的可靠替代方案都非常有趣。我认为我们需要记住，所有这些方法，无论是基于PIC、VCSEL还是LED，都仍处于起步阶段，因此，需要针对2034年而不是2024年的需求......这意味着现在的带宽、带宽密度和能源效率通常为 30 倍（因此 <100 fJ/b).

Paul Brooks:one important metric is bandwidth density - off the front panel and off the silicon. Today we already have a huge mismatch - the author notes that the 'internal speed' in an IC is under 10Gb/s it is very very wide - hence we use SERDES and today we see 112G parts established and 224G will emerge later this year. A large ASIC may have 6000 bumps and this already a throttle factor with 112G. So how to get the BW off - copackage optics - this would use chunks of 32 at 112G a lane (3Tb engines) - this field is getting a lot of investment and many public displaces (OFC24) show this as viable but can it manufactured and deployed at scale? We already have switch silicon at 51Tb and so we will need to have very broad interfaces to utilize what silicon can deliver. Copper remains the medium of choice and it certainly is viable (as DAC or perhaps ACC/AEC) for links at 224G SERDES/1.6Tb. This is a match for inside the rack - not perfect but robust - new equalizers will go to 40dB now... Will people accept a link x10 broader based on lower cost LED? optical interconnects are more challenging than copper....an interesting path lies ahead
一个重要的指标是带宽密度 - 远离前面板和硅片。今天，我们已经出现了巨大的不匹配 - 作者指出，IC中的“内部速度”低于10Gb / s，它非常非常宽 - 因此我们使用SERDES，今天我们看到112G部件建立，224G将在今年晚些时候出现。一个大型 ASIC 可能有 6000 个凸起，这已经是 112G 的节流因素。那么如何摆脱 BW - copackage optics - 这将在每车道 112G（3Tb 引擎）上使用 32 个块 - 这个领域正在获得大量投资，许多公共流离失所 （OFC24） 表明这是可行的，但它可以大规模制造和部署吗？我们已经有了 51Tb 的交换机芯片，因此我们需要有非常广泛的接口来利用硅可以提供的功能。 铜缆仍然是首选介质，对于224G SERDES/1.6Tb的链路，铜缆肯定是可行的（如DAC或ACC/AEC）。 这是机架内部的匹配 - 不完美但坚固 - 新的均衡器现在将达到 40dB......人们会接受基于低成本 LED 的 10 倍更宽的链接吗？光互连比铜缆更具挑战性。一条有趣的道路在前方

Bardia Pezeshki:See answer to Tom's question. We can get very high bandwidth density using bundles of illumination fiber. Large arrays are available. So ultimately no need for serdes and the accompanying complications. Most of us think single mode fibers, which is tough to align, brittle, and usually 1D arrays (eg psm in MTP). But illumination fibers, developed for lighting, can be in very large and ordered arrays, giving you tens of thousands of lanes or even more. We've done a first demo with 300 lanes.
请看汤姆问题的答案。 我们可以使用照明光纤束获得非常高的带宽密度。可以使用大型阵列。 因此，最终不需要 serdes 和随之而来的并发症。我们大多数人都认为单模光纤，它难以对齐、易碎，通常是一维阵列（例如 MTP 中的 psm）。但是，为照明而开发的照明光纤可以采用非常大且有序的阵列，为您提供数以万计的通道甚至更多。我们已经完成了第一个有 300 条车道的演示。

Dan Kuchta:I'm quite interested in the peer reviewed published reliability model for these LEDs. Can you provide the reference(s)?
我对这些 LED 的同行评议发表的可靠性模型非常感兴趣。 您能提供参考资料吗？

Bardia Pezeshki:Thanks Dan! Most LED manufacturers share their reliability reports with their customers. Closest to our application or use case, is LEDs for car headlights that are currently deployed on Audi/BMW/ and other high end vehicles. I think we shared with you our early data. We have some updates to share on our next call. I may do a paper soon and make our data public. 
谢谢丹！ 大多数 LED 制造商与客户分享他们的可靠性报告。 最接近我们的应用或用例的是目前部署在奥迪/宝马/和其他高端车辆上的汽车前照灯的 LED。 我想我们与您分享了我们的早期数据。 我们有一些更新要在下次电话会议上分享。 我可能很快就会写一篇论文，把我们的数据公之于众。

<https://www.linkedin.com/posts/bardia-pezeshki-b75b2b6_silicon-photonics-co-packaging-cool-but-activity-7196899863488307202-ZHR2/>

## 5.3 Techopedia 专访 Bardia Pezeshki

从电子技术到光子技术的转变有望成为未来的下一个数字前沿和规范。从网络到6G和芯片到芯片通信，光子技术有望成为更强大、更节能、更高速的数据传输的解决方案。

英特尔、索尼、NTT 以及无数其他公司和初创公司正在开发新的光子技术，重新构想我们使用芯片和网络的方式。

当今的计算仍然面临着一些瓶颈，其中之一就是电子来回发送数据的最大速度。

但如果线索不在名称中，光子学就利用光——没有什么能胜过光。

Techopedia 采访了Avicena公司的首席执行官兼董事会成员Bardia Pezeshki 博士，Avicena 是一家总部位于加利福尼亚州桑尼维尔的高带宽半导体公司，也是探索利用超高速 µLED或微型 LED 进行芯片到芯片通信和连接的公司之一。

**关键要点**

- 通过利用光的力量，光子学在速度、效率和数据传输容量方面比传统电子学具有显著优势。
- 光子学对于克服当前计算架构的局限性至关重要，特别是在人工智能和高性能计算等领域。
- 为了充分发挥光子学的潜力，科技巨头、初创企业和研究机构之间的合作对于制定标准和克服技术障碍至关重要。
- 光子学的广泛应用将彻底改变从数据中心到医疗保健的各个行业，因为它推动了技术和性能的前所未有的进步。

### 5.3.1 计算挑战：能源、处理能力和低延迟

随着人工智能(AI) 和机器学习(ML) 的发展速度和势头不断加快，NVIDIA等公司推出了更强大的芯片，而英特尔和华为等公司也全力参与竞争，但仍有一个大问题尚未解决：

人工智能和机器学习处理的数据比以往任何时候都多，可能导致高延迟，并使数据中心的能耗达到历史最高水平。

不同的研究预测人工智能将导致能源消耗大幅增加。例如，高盛发现该技术预计将使数据中心的电力需求增加 160%。

Avicena 的 Pezeshki 解释说，几十年来人们一直想将集成电路与光子学连接起来，他说：

<font color=red>“原因是光子比电子更善于传递信息。它们彼此之间不会发生相互作用，而且不存在电阻和电容。”</font>

### 5.3.2 “用光说话的芯片”

光子学的潜力已经吸引了大多数大型科技公司的注意，如上所述，英特尔在过去几十年中已在硅光子学和光学技术方面投资了数十亿美元，其中包括洛克希德马丁、IAG Capital Partners、惠普企业和 NVIDIA。

然而，光子技术仍在发展中，面临诸多障碍。Pezeshki 为我们解析了其中的奥秘。

<font color=red>“芯片上和芯片外的数据移动问题是电子产品的最大瓶颈。几乎所有先进芯片都受到（输入/输出） I/O 的限制，这种限制在 AI 类型的配置中最为严重，因为 GPU 必须通过交换机网络并行工作。”</font>

Pezeshki 解释说，光子芯片的关键问题在于硅从根本上来说不是一种好的光学材料，并且与光子标准激光器不兼容。

<font color=red>“使用标准光纤技术将相距仅一米左右的芯片连接起来确实太昂贵且复杂。”</font>

Avicena 的解决方案是利用 LED 和显示技术，让“芯片通过光说话”。

<font color=red>“我们基本上是将一个小型 microLED 显示屏和一个摄像头放在芯片上，让芯片互相‘看着’，通过类似成像光纤的东西交换数据。”</font>

为了与芯片配合使用，Avicena 的 microLED 显示器比普通显示器更简单——

1000 个像素为单一颜色，而RGB像素为数百万。但 Avicena 凭借简单性获得了高速性能 — 与普通显示器的帧速率相比，速度高达数 Gb/s。

“我们使用的显示和摄像头技术与几乎所有（互补金属氧化物半导体）CMOS（大多数现代电子设备的基础）兼容”

### 5.3.3 长距离光子学与短距离通信

NTT 已经证明光子网络和高速、低延迟和海量数据传输是可能的。

NTT 的研究与开发部门认为光子学是一种自然的进化，其应用范围将无穷无尽，从远程先进的机器人实时医疗程序和手术到数字孪生、智能汽车和智能城市以及网络上的人工智能数据。

但是，使用光子学在长距离架构下传输数据是一回事，而让芯片在硬件内非常短的距离内“对话”又是另一回事。Pezeshki 不仅相信这是可能的，而且坚定地宣称他的公司正在努力实现这一里程碑。

<font color=red>“我们的目标是实现芯片间光子互连的十年梦想。”</font>

Avicena 的技术与其他走上这条路、尝试过但失败的人有何不同？与传统方法相比，他们基于 LED 的方法比铜或激光更节能。它也更加并行——想想超宽数据总线，它直接与芯片上的信息原生移动方式进行交互。

Pezeshki 表示：<font color=red>“没有必要将数据序列化为每条通道非常高的速度，因为这需要更多的电力并延迟数据的移动。”</font>

Pezeshki 表示，随着 AI 集群面临数据挑战且需求越来越大，内存芯片和GPU内的光学接口允许每个处理器访问更多内存，并且许多处理器可以共享一个大内存池。

### 5.3.4 用例和应用：现实生活中的光子学

光子芯片到芯片的通信可能代表着计算架构的巨大转变。

通过利用光的速度和效率，该技术克服了传统电气互连的根本限制。光子芯片不再依赖铜线，而是利用光在处理器、内存单元和其他组件之间传输数据。

Pezeshki 谈到了为什么连接与处理器一样重要。

<font color=red>“从总体来看，计算能力不仅来自快速的处理器和内存，还来自处理器之间的连接密度。”</font>

“当人们转向光子学时，特别是具有多通道的并行配置，并且信息在芯片上垂直流动，你就可以正面解决问题。”

改造全球硬件以支持光子学是一项艰巨的任务。Pezeshki 解释了 Avicena 如何努力使这一转变更加无缝。

Pezeshki 表示：“对于 Nvidia 或英特尔来说，推出一款配备紧密光学接口的新处理器意义重大。为这一转变提供分步路线图非常重要。”

<font color=red>“我们正在制造符合标准的光缆，可以替代电缆和板载光学器件，而不需要重新设计 GPU。”</font>

随着这些光学解决方案在广泛的现场应用中得到证实，芯片设计人员将更愿意将光学器件靠近 IC。当然，最终我们的技术可以集成到处理器和内存芯片中，从而消除接口封装和 IC。

### 5.3.5 底线
从电子技术到光子技术的转变有望彻底改变计算架构，一些人可能会认为这是一次意想不到的转变。以软件和代码形式出现的创新与硬件层面的创新大不相同。

从电子和铜线到芯片间直接光缆的转变极具挑战性。整个行业的标准化、供应链和物流问题以及行业的全面接受都是光子学实现所需的因素。

然而，像 Avicena 这样创造合规创新解决方案的公司并非孤军奋战。从英特尔到 NTT 以及所有大型科技公司，光子学都已列入他们的议程。原因很简单。

为了进一步迈向技术的未来，世界需要更快、更高效的处理和传输，以及更密集的连接以实现同步通信。光子学和光能提供所有这些，甚至更多。

<https://www.techopedia.com/what-is-photonics-next-chapter-of-computing>

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

# 7. 多孔硅

Microscopy studies of InGaN MQWs overgrown on porosified InGaN superlattice pseudo-substrates

我们研究了在无孔和多孔 SL 模板上生长的 MQW 中出现的小 V 形坑的起源。我们之前的研究表明，多孔 SL 模板会导致应变松弛，因此，与无孔模板上的 QW 相比，在这种结构上生长的 QW 中出现的额外 V 形坑的密度更高，这令人惊讶。在无孔模板上，我们已经证明小 V 形坑可能来自 TD 或 SMB 与样品表面的交叉点。当 MD 从顶面滑入样品以减轻应变时，会出现额外的 TD。这些 MD 通常会滑入 SL 本身。相比之下，当 SF 在生长过程中在异质结构的界面上形成时，就会出现 SMB。

在部分松弛的多孔模板上过度生长期间，MQW 的铟含量会随着孔隙度的增加而增加，这要么是因为成分牵引效应降低，要么是因为多孔层中的热导率降低。因此，尽管模板松弛，但 In 含量较高的 MQW 中松弛的驱动力可能仍然很大。此外，多孔结构会阻止 MD 滑入 SL，并可能由于应变和成分不均匀性而抑制 MD 的延伸。总之，这些影响解释了在多孔模板上过度生长的 MQW 中观察到的额外小 V 坑。最后，我们注意到，V 坑密度可以通过 SL 模板中的多孔化程度来管理，这可能为 V 坑工程提供有用的控制参数，以优化长波长 LED 中的电流注入。

<https://iopscience.iop.org/article/10.1088/1361-6641/ad575b>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Microscopy%20studies%20of%20InGaN%20MQWs%20overgrown%20on%20porosified%20InGaN%20superlattice%20pseudo-substrates.pdf>

# 8. -3 dB带宽

-3 dB带宽是一个在信号处理、电子工程和通信系统中常用的概念，具体含义如下：

**定义**

-3 dB带宽指的是信号功率衰减到最大功率的二分之根号二倍（即功率下降到最大值的0.707倍）时，对应的频率范围。在对数坐标中，这个点被称为-3分贝点或半功率点，其定义是功率减半前的频率宽度。

**解释**
- 功率与幅值的关系：幅值的平方即为功率，当幅值变为最大值的二分之根号二倍时，功率就变为最大功率的一半。
- 对数坐标中的位置：在对数坐标中，功率减半对应于-3dB的位置，因此称为-3dB带宽。
能量集中度：这个带宽表示信号能量在该频率范围内集中度达到一半，是描述信号能量集中程度的一个重要参数。

**应用**
-3 dB带宽在多个领域有广泛应用，包括：

- 滤波器设计：用于衡量滤波器的通带平坦度和阻带衰减，是滤波器性能的一个重要指标。
- 信号分析：在信号分析中，了解信号的-3 dB带宽有助于理解信号的频谱特性和能量分布情况。
- 通信系统：在通信系统设计中，-3 dB带宽可用于评估系统的传输能力和信号完整性。

**示例**

假设有一个信号，其最大功率对应的频率为f0，当信号功率衰减到最大功率的一半时，对应的频率范围为f1到f2。那么，这个信号的-3 dB带宽就是从f1到f2的频率范围。

**综上所述**，-3 dB带宽是一个重要的技术参数，用于描述信号的能量集中程度和频率特性，在信号处理、电子工程和通信系统中具有广泛的应用。

来自 文心一言

# 9. LED和LD光调制的区别

高调制速率下的信号光源常用激光器来做信号源，而不采用LED。

半导体发光二极管由于不是阈值器件，它的输出光功率不像半导体激光器那样会随注入电流的变化而发生突变，因此LED的PIV特性曲线的线性比较好。图示出了LED与LD的PIV特性曲线的比较。由图可见，其中LED1和LED2是正面发光型发光二极管的Pq特性曲线。LED3和LED4是端面发光型发光二极管的PIV特性曲线，可见，发光二极管的PIV特性曲线明显优于半导体激光器，所以在模拟光纤通信系统中得到广泛应用。但在数字光纤通信系统中，因为它不能获得很高的调制速率（最高只能达到100 Mb/s）而受到限制。

![image](/picture/wx_article__36431b42f12d194a5c401d71647ce267.jpg)

至于为什么不能获得高的调制速率，从光子的产生上来分析是：

LED是只能等上能级的电子自发地下降到低能态（也就是电子和空穴复合），产生自发辐射或者热效应。所以LED的响应速度主要是由上能级的寿命决定。而LD因为有光腔产生的光反馈，这个光可以把处于上能级的高能态的电子，通过受激辐射，下降到低能态。所以LD比LED更快。<font color=red>也可以说LD的光很大程度上是受限于皮秒ps的光子寿命，而LED受限于纳秒ns的载流子寿命</font>。从LD的光子寿命可以分析如下：

“估算无腔面镀膜，折射率为3.5的300um长激光器器件中，光子寿命是多少？”

解：

激光器腔体中包含吸收损失α产生的增益循环表达式：

![image](/picture/wx_article__84bc17601c4aec520b173e5cb4c14b65.jpg)

L=300um,R1=R2=0.3 先不看吸收损耗α=0，计算gCav=40cm-1

同时，cm-1为单位的增益可以转换为s-1为单位的增益。

g[cm-1]=g[s-1]c/n

gcav除以c/n，就是g[s-1]值为3.3X105s-1

换成时间常数τp=3ps.

这个ps量级的光子寿命，就是半导体激光器可以快速调整的基本原因了。而LED的载流子寿命是ns级别。因此激光器可以调制到Gb/s,远比二极管的速度快。

不过也听说国外有人用microLED做光调制到1~5 Gb/s。微LED波长430 nm，带宽20 nm， 几厘米的传输距离可以实现高速调制。

![image](/picture/wx_article__591b96a2fceebfaa5a12d756205feb98.jpg)
![image](/picture/wx_article__277677c2e01c42a4c57753a08b31dcc7.jpg)

<https://lights.ofweek.com/2023-10/ART-220008-11000-30613227.html>

# 10.模拟光纤通信相关知识

## 10.1 LED光通信背景知识

光通信是要实现超高速的光开关速率，而并不是常见电路中的高速开关，这里强调的是光的开关速率，并非电子或空穴的开关速率；光通信用以补充WIFI等无线通信应用的不足，在某些领域替代WIFI成为一种全新的通信方式。LED光通信技术是近年来逐步发展起来的一种全新的通信技术，很多相关的技术研究还处在起步阶段，尤其在高速LED器件、高速开关电路的技术更是几乎空白。LED串联一个开关进行简单调制，缺点是开关速度严重受限，载流子复合速率不高且剩余载流子泯灭时间过长，使得光通信效果很差。

<https://patents.google.com/patent/CN105050245A/zh>

## 10.2 LED调制带宽

LED的调制带宽决定了通信系统的信道容量和传输速率,其定义是在保证调制度不变的情况下,当 LED输出的交流光功率下降到某一低频参考频率值的一半时(-3dB)的频率就是 LED的调制带宽,如图3-5所示。图中的光带宽指光电探测器输出的信号电流变为原来一半时对应的带宽。

LED的调制带宽受响应速率限制,而响应速率又受半导体内少子寿命τc 影响:

![image](/picture/3db%20f.png)

对于III-V 族(如 GaAs)材料制成的发光二极管而言,τc 的典型值为100ps,故 LED的理论带宽总是限制在2GHz以下。当然,目前所有发光二极管的τc 带宽都远远低于这个值,照明用的大功率白光二极管由于受其微观结构及光谱特性所限,带宽更低。较低的调制带宽限制了 LED在高速通信领域(包括可见光通信系统)的应用,因此,设法提高LED的调制带宽是解决问题的关键。

**综上，LED调制带宽基本取决于载流子寿命**
- 如果载流子寿命100皮秒ps，则3dB理论带宽约为2.7Ghz
- 如果载流子寿命100纳秒ns，则3dB理论带宽约为2.7Mhz

<https://github.com/basteng/Today-I-Learned/blob/main/paper/%E5%8F%AF%E8%A7%81%E5%85%89%E4%BF%A1%E9%81%93%E5%BB%BA%E6%A8%A1.pdf>

摘自 p29~p30

# 11. PCIe诞生20年来最大变革！引入光学传输

PCI-SIG组织官方宣布，已经成立新的光学工作组(Optical Workgroup)，研究为PCIe规范引入光学传输接口的可能性。

PCIe标准是Intel 2001年提出的，2003年发布1.0版本，数据传输率为2.5GT/s，2022年初发布的PCIe 6.0版本已经达到64GT/s。

正在开发中的7.0继续翻番为128GT/s，x16双向理论带宽高达512GB/s。

20年来，PCIe接口的外观形态虽然没有任何变化，而内部技术已经翻天覆地，并始终保持前后兼容。

只是受到传统铜线传输机制的制约，PCIe技术的继续提升越来越难，不得不加入越来越多、越来越复杂的辅助机制，控制信号和数据完整性。

正因为如此，PCI-SIG决定更换赛道，借助光学传输的力量，寻求继续提升速度、降低功耗和延迟。

当然，一切都还在起步阶段，说不定要到PCIe 9.0才能真正拥抱光学传输呢。

![pcie1](/picture/PCIE1.jpg)
![pcie2](/picture/PCIE2.png)
![pcie3](/picture/PCIE3.png)

<https://news.mydrivers.com/1/926/926700.htm>

PCIE相关报告

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/DriveWorld%20PCI-SIG%20-%20Accelerating%20Automotive%20Connectivity%2C%20from%20Infotainment%20to%20ADAS.pdf>

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/HOTI_PCIe6.0.pdf>

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/SNIA-SDC23-DasSharma-PCIe-7.0-Specification-Bandwidth.pdf>


# 12.厦门大学与阳明交大研发红/黄光Micro LED光通信技术

厦门大学和中国台湾阳明交通大学的研究人员通过将氮化铟镓(InGaN)黄光、红光 Micro LED应用于光通信 (VLC)系统当中，实现了更高的光通信效率。

研究人员表示，与光通信系统中常用的硅基光电二极管相比，氮化铟镓光电二极管具有低噪和高灵敏度的优势。

该研究表明，与之前使用的较短波长Micro LED光电二极管相比，此次研究的红/黄光Micro LED对蓝光拥有更高的响应程度。

据悉，长波长的氮化铟镓Micro LED具有在新型显示和可见光通信领域的应用潜力。在本次研究中，研究团队为光通信应用制造了红光和黄光Micro LED，作为光通信发射器和光电二极管 (PD)，并采用应力调制工程和原子层沉积（ALD）技术来提高传输和检测性能。

实验结果表明，在用作光通信发射器时，红光和黄光Micro LED在2000 A/cm²电流密度下表现出439.7和532.5 MHz的高调制带宽，分别实现1.9和2.4 Gbps的数据速率。当用作光通信光电二极管时，具有高铟成分量子阱的长波长Micro LED表现出更长波长吸收边缘，这有望在滤除荧光成分的同时实现对蓝光更高的响应度。

另外，红光和黄光Micro LED光电二极管的响应光谱与大部分蓝色信号重叠，因此对于450 nm的波长光，红光和黄光Micro LED的响应度分别高达0.208和0.135 A/W，高于现有的氮化铟镓LED光电探测器。

此外，研究团队还表示，基于波长选择性，长波长的Micro LED电二极管可滤除缓慢的荧光发射，从而实现高于硅基探测器数倍的白光调制带宽。（来源：LEDinside）

<https://mp.weixin.qq.com/s/rVoYMnpO0djGfXxH_3z2AA>

# 13.蓝色GaN/InGaN量子阱发光晶体管的特性 2023IRDS_BC 3.3.8 Transistor Laser

Other noteworthy results include demonstration of blue-emitting light-emitting transistors in the GaN/InGaN system.573

Characteristics of Blue GaN/InGaN Quantum-Well Light-Emitting Transistor

**摘要：**
我们展示了第一个 GaN/InGaN 量子阱发光晶体管 (QW-LET) 的同时电调制和光调制，该晶体管在重掺杂 p 的 In0.05 Ga0.95N 基极中包含一个 In0.15 Ga0.85N QW。与 GaAs/InGaAs 同类产品不同，GaN/InGaN QW-LET 具有电流增益（高达 5）和光功率，它们随基极电流线性增加。其发射光谱以 420 nm 波长为中心，几乎不随电流注入而移动，这与典型的氮化物基 LED 的行为相反。该器件的不寻常特征可能与 QW 中的极化场引起的倾斜能带分布和 p 型掺杂问题有关。

<https://ieeexplore.ieee.org/document/8911438>

# 14.你也可以使用 LED 作为传感器
LED 是一项很棒的技术。你只需要投入一点电力，就能发出大量的光。它们高效、便宜、数量充足。我们用它们做很多事情！

您可能不知道的是，这些不起眼的组件有一个秘密功能，数据表中基本没有记录。当然，您可以使用 LED 作为光源，但您知道您可以将其用作传感器吗？


两用设备
使用 LED 作为传感器的概念很像使用扬声器作为麦克风。翻转一下，LED 不会发光，而是感应光线。使用万用表可以很容易地看到效果。将万用表的引线连接到 LED，并将其设置为测量电流。将 LED 指向太阳，您可能会得到读数。虽然 LED 对光敏感，但与传统光电二极管不同，它通常对光的波长范围非常小。

但如何使用这种效果呢？其实，你可以采用多种方法。如果你是模拟爱好者，你可以将 LED 连接到运算放大器的输入端，并根据需要使用该设备放大输出。几乎任何普通运算放大器都可以这样使用：LED 上的光越多，产生的输出电压就越高。

但是，您可以走得更远，正如三菱电机研究实验室 (MERL) 的聪明才智早在 2003 年就确定的那样。效仿他们的例子，您可能希望将 LED 连接到微控制器。将其设置为“反向偏置”模式，当连接到 IO 引脚时，它可以充当传感器，而不是光发射器。要做到这一点，只需将 LED 的阳极接地，同时将阴极连接到高状态的 I/O 引脚。这实现了“反向偏置”，并对 LED 的固有电容进行充电。电容很小，所以这只需要几分之一秒。然后，可以将 IO 引脚切换到输入，LED 的电容将放电到微控制器引脚中。光越多，LED 中感应的电流越大，LED 的电容放电越快。测量电压降至 IO 引脚数字逻辑电平以下所需的时间，您就可以使用简单的 IO 引脚感应光照水平。

<font color=red>两个三态引脚可让您使用 LED 发光并感应光线。</font>
![LED](/picture/Screenshot-2024-07-18-175501.webp)
来源：MERL，研究论文 <https://www.merl.com/publications/docs/TR2003-35.pdf>

事实上，MERL 团队意识到，你甚至可以走得更远。不起眼的 LED 可以成为“最后一厘米”通信设备，既用作光发射器，又用作光接收器。要实现这一点，只需将 LED 插入微控制器上的两个三态 IO 引脚之间。当阳极驱动为高电平、阴极驱动为低电平时，LED 就会亮起。反过来，LED 就会反向偏置。然后，可以将其中一个三态引脚设置为输入模式，以将 LED 读取为传感器。

MERS 团队建议，LED 可用作各种创新应用中的传感器。您可以使用电视的电源 LED 来检测光照水平，从而适当调整屏幕亮度。您甚至可以进行简单的接近感应，使用 LED 阵列依次充当发射器和传感器。如果您愿意，您甚至可以在小型设备上使用状态 LED 进行双向通信。

<font color=red>研究人员仅使用普通 LED 便可在几厘米的距离内实现微控制器之间的通信。数据速率达到 250 比特/秒</font>。

来源：MERL，研究论文 <https://www.merl.com/publications/docs/TR2003-35.pdf>

然而！我们几乎从未将 LED 用于上述任何用途。实际上，虽然 LED 是传感器，但它们并不是 出色的传感器。如今，我们有更好的光电晶体管、光电二极管和其他传感器。如果您尝试设计一个零件数量最少或尽可能便宜的设备，这种技术可能 对您有用。或者，如果您想在仅有 一个 LED 的设备中添加惊喜功能。但在现实世界中，这种技术并没有得到广泛的使用。毕竟，摆弄巧妙的 LED 技巧比仅仅指定合适的传感器需要更多的工程时间。

尽管如此，该技术还是找到了一些实际应用。以这种方式使用的 LED 确实具有波长选择性强的优点，并且可以随着时间的推移保持相当稳定。传奇人物Forrest Mims利用了这一点，将 LED 传感器用于各种科学仪器中。事实上，他的臭氧测量装置依赖于这种技术，并且非常可靠，证明了NASA 自己的 Nimbus-7 卫星存在漂移误差。

<font color=red>Forrest Mims 喜欢使用运算放大器来增强用作传感器的 LED 的输出。</font>
来源：Forrest Mims 的 Make 文章 <https://makezine.com/projects/make-36-boards/how-to-use-leds-to-detect-light/>

快速发展的钙钛矿技术领域也充满希望。钙钛矿 LED（PerLED）可以使用先进的半导体材料来制造既可作为良好光源又可作为光电探测器的设备。人们希望它们能够制造出无需额外触摸传感器的可触摸显示器。相反，PerLED 阵列可以同时充当显示器和传感器。然而，目前这项研究还处于早期阶段，钙钛矿的不稳定性意味着任何实际应用都还遥遥无期。

还值得注意的是，这种技术不适用于许多现代 LED。即可寻址 LED、自闪烁 LED 以及任何此类 LED。这是因为这种技术依赖于将微控制器直接连接到 LED 芯片本身。许多现代“智能”LED 本身不分出引脚，只为内部控制器芯片提供引脚。因此，不要指望将此技术用于您的 NeoPixel、WS2812B 或类似产品。

归根结底，使用 LED 作为传感器是一种有趣的技术。如果您使用特定波长的光做特定的事情，它也非常有用。不过，除此之外，这是一个很棒的派对技巧，值得放在您的工具箱中，因为您永远不知道它什么时候会派上用场。

<https://hackaday.com/2024/07/23/you-can-use-leds-as-sensors-too/>

# 15.如何使用 LED 检测光

![LED2](/picture/led-1.webp)
既然电磁电话听筒可以兼作麦克风，那么半导体光探测器是否可以兼作光发射器呢？

1962 年，当我还是一名高中生时，这个问题就浮现在我的脑海里。那时我还不知道半导体中的量子效应与电话听筒的电磁操作无关。如果我知道这一点，我绝不会将火花线圈连接到硫化镉光敏电阻的引线上，看看它是否会发光。它确实发光了——一种柔和的绿光，中间点缀着明亮的绿光。

大学期间，我发现连接到晶体管脉冲发生器的硅太阳能电池会发出不可见的红外线闪光，而第二个太阳能电池可以检测到这种闪光。1972 年，我使用近红外 LED 和激光二极管通过空气和光纤发送和接收语音信号。后来，我尝试使用双向光耦合器，通过将一对 LED 粘在一起，使它们彼此面对而制成。

1988 年，我尝试使用 LED 作为阳光探测器。它们的效果非常好，以至于我于 1990 年 2 月 5 日开始使用的第一个自制 LED 太阳光度计至今仍在使用。

 

为什么使用 LED 作为传感器？
硅光电二极管随处可见且价格低廉。那么为什么要使用 LED 作为光传感器呢？

LED 检测的波长范围很窄，这就是我称其为光谱选择性光电二极管的原因。硅光电二极管的光谱响应范围非常广，约为 400nm（紫色）至 1,000nm（不可见的近红外），并且需要昂贵的滤光片才能检测特定波长。
大多数 LED 的灵敏度随着时间的推移都非常稳定。硅光电二极管也是如此——但滤光片的寿命有限。
LED 既能发光，又能检测光线。这意味着只需两端各一个 LED 即可建立光学数据链路，因为无需单独的发送和接收 LED。
LED 比光电二极管更便宜且更普及。
 

LED 作为光传感器的缺点
没有完美的传感器。

LED 对光的敏感度不如大多数硅光电二极管。
LED 对温度敏感。这可能会给室外传感器带来问题。一种解决方案是将温度传感器安装在 LED 附近，以便可以实时或在处理数据时应用校正信号。
我测试过的一些 LED 确实会逐渐失去灵敏度。
 

LED 检测特定颜色的光
典型的人眼对波长范围从 400nm（紫色）到 700nm（红色）的光有反应。LED 检测的光波段要窄得多，峰值灵敏度在波长略短于其发射的峰值波长处。例如，峰值发射为红色（660nm）的 LED 对 610nm 的橙色光反应最佳。

典型的蓝色、绿色和红色 LED 发出的光的光谱宽度约为 10nm—25nm。近红外 LED 的光谱宽度为 100nm 或更大。我测试过的大多数 LED 的灵敏度都提供了足够的重叠，可以检测到来自相同 LED 的光。

![LED3](/picture/led-2.webp)

图 A显示了 7 个蓝色、绿色、红色和近红外 LED 的光谱响应，它们取代了我改进的多滤光片旋转阴影带辐射计中用于太阳光谱的常用硅光电二极管和滤光片。

蓝色和大多数绿色 LED 都是由氮化镓 (GaN) 制成的。最亮的红色 LED 是由铝砷化镓 (AlGaAs) 制成的。近红外遥控器中使用的 LED 也是 AlGaAs 设备；它们的峰值发射约为 880nm，峰值检测约为 820nm。

旧式遥控器使用硅补偿的砷化镓 (GaAs:Si)。这些 LED 发出的波长约为 940nm，非常适合检测水蒸气，但它们已经变得非常难以找到。

根据我的经验，红色“超亮” LED 和 AlGaAs LED 以及类似的近红外 LED 的灵敏度在多年使用后都非常稳定。由磷化镓 (GaP) 制成的绿色 LED 也非常稳定。然而，由 GaN 制成的蓝色 LED 的灵敏度下降幅度比我使用过的任何 LED 都要大。

笔记：

这不适用于白色 LED，白色 LED 是一种蓝光 LED，涂有荧光粉，当受到 LED 发出的蓝光刺激时，会发出黄光和红光。蓝色、黄色和红色的融合会产生白光。虽然白色 LED 可以检测蓝光，但蓝色 LED 是更好的选择。

基本 LED 传感器电路

![LED4](/picture/led-3.webp)
![LED5](/picture/led-4.webp)

在大多数电路中，你可以用 LED 代替标准硅光电二极管。只需注意极性即可。另外，请记住，LED 不像大多数标准光电二极管那样敏感，并且对更窄的光波长带有反应。

为了获得最佳效果，请使用封装在透明环氧树脂中的 LED，并先进行一些实验。这些实验将帮助您了解用作传感器的 LED 的检测角度与用作光源时的发射角度如何匹配：

- 使用标准耦合器将 LED 连接到塑料光纤，或使用此方法直接连接（图 B）：用锉刀将 LED 顶部弄平，将其牢固夹紧，然后小心地在发光芯片正上方钻一个小孔。插入光纤并将其固定到位。
- 将透明封装的红色或近红外 LED 的引线连接到设置为指示电流的万用表。将 LED 指向太阳或明亮的白炽灯，仪表将指示电流（图 C）。
- 使用一个 LED 为第二个 LED 供电。连接 2 个透明封装的超亮红色 LED 的阳极和阴极引线。当用明亮的手电筒照亮一个 LED 时，第二个 LED 会发光。将热缩管放在发光的 LED 上以阻挡来自手电筒的光线。您可以在文章顶部的照片中看到它的工作原理。

![LED5](/picture/led-5-alt%20(1).webp)

LED 的光敏表面比大多数硅光电二极管小得多，因此它们更有可能需要放大。廉价的运算放大器是理想的选择。图 D显示了一个简单的电路，我经常用它来将 LED 的光电流转换为成比例的电压。Linear Technology LT1006 单电源运算放大器 (IC1) 提供的电压输出几乎与入射光的强度完全成线性关系。增益或放大倍数等于反馈电阻 (R1) 的电阻。因此，当 R1 为 1,000,000 欧姆时，电路的增益为 1,000,000。电容器 C1 可防止振荡。

许多其他运算放大器可以替代 LT1006，但大多数运算放大器都需要双极性电源。如果使用其中一种，请将引脚 4 直接连接到负电源。将引脚 3 和 LED 的阴极连接到地（正电源的负极 F 和负极 w 之间的连接点）。

 

进一步
为用作光电二极管的 LED 开发新应用的最佳方式是试验我在此处描述的应用。当我在 60 年代进行这项工作时，我并不知道这些简单的实验会通过单根光纤实现双向通信，以及使用几种仪器测量大气，而这些仪器我已经使用了 23 年多。

本文最初发表于MAKE 第 36 卷，第 136 页。

有关“LED 作为光电二极管”的更多 Forrest M. Mims III 文章和书籍，请访问forrestmims.org/publications.html。

<https://makezine.com/projects/make-36-boards/how-to-use-leds-to-detect-light/>

# 16. 光子学与人工智能：行业观点

OPN 与六家公司讨论了人工智能可能为光学和光子学行业（在硅光子学及其他领域）带来的一些机遇。

2022 年 11 月，Open AI 发布了生成式人工智能聊天机器人 ChatGPT，这是全球范围内轰动一时的技术新闻，似乎为整个商业领域打开了新的生产力和潜力前景。尽管最初的公众炒作大部分已经平息，但数据中心支持人工智能的基础设施以及产品实验室支持人工智能的思维的持续快速增长，为光学和光子学行业创造了令人着迷的机会。

为了了解这一切是如何展开的，OPN 最近采访了六家关注这个市场的公司的代表。虽然由此得出的结论只是故事的一小部分，但它们确实暗示了生成式人工智能的数据需求如何催化了硅光子学活动的发酵，以及人工智能对光学公司如何看待其其他产品产生更广泛的影响。

**芯片时间**

对于硅光子学而言，服务这些市场的大部分行动在于解决人工智能的“数据瓶颈”。这是指随着支持人工智能的 CPU、GPU 和专用集成电路 (ASIC) 通过铜互连以越来越快的速度从封装外计算资源（例如内存模块或其他 ASIC）中吸收数据，延迟和能耗增加。

许多公司都在为解决这一难题而努力：硅光子“小芯片”将电域和光域之间的转换尽可能地靠近 GPU，从而使分布式计算资源之间的连接保持以光纤中快速、节能的光编码形式存在。硅谷的Ayar Labs是一家在该领域耕耘了九年的公司。Ayar 于 2015 年 5 月成立，其前身是加州大学伯克利分校、科罗拉多大学和美国麻省理工学院 (MIT) 实验室的工作（后来在《自然》杂志上报道），展示了 Ayar 现在所说的“世界上第一个使用光进行通信的处理器”。

特里·索恩（Terry Thorn）三年前加入该公司担任商业运营副总裁，此前他在半导体巨头英特尔公司担任了 24 年的各种职务。他告诉 OPN，阿亚尔的工作重点是计算系统内部“扩展”领域的问题。该领域涉及在计算芯片之间分流数据，无论是 CPU 和 GPU、两个 GPU 还是 GPU 和分布式内存主机。（它与涉及将数据从服务器机架传输到其他服务器的“横向扩展”领域形成对比，这通常是传统可插拔收发器的最佳选择。）

在扩展领域，当大量传统铜互连被光纤中的光链路取代时，“显然，延迟和能耗的降低会让您受益匪浅”，Thorn 表示。“我们的连接越接近计算芯片，我们就越能充分利用这种效率优势。”他表示，在扩展领域，Ayar 认为“最大的直接利益，也是客户最迫切需要和最感兴趣的领域。”

Ayar 为满足这一需求而设计的芯片组名为 TeraPHY（发音为“terrify”）。该芯片组旨在与电子 GPU 或 CPU 集成在一起，允许将电子数据立即编码（通过微环谐振器系统）为光学数据，并通过光纤带发送到其他配备类似设备的计算资源。

Thorn 表示，在 OFC 2023 上，Ayar 展示了其芯片在“实时硅片中”运行的“非常稳定的演示”，该芯片在 4 Tbps 双向连接（即每个方向 2 Tbps）中运行，能耗仅为 5 皮焦耳 (pJ)。高数据吞吐量是通过在芯片上进行波分复用来实现的，八个光纤连接中每个光纤承载八个波长的光，每个波长以 32 Gbps 的速度传输数据。八个月后，即 2023 年 11 月，Ayar 展示了一个类似的系统，该系统采用英特尔现场可编程门阵列 (FPGA) 封装，“连续数天实时运行”，Thorn 表示。

这些演示以及 Ayar 产品中的另一个关键组件是其片外光源，商品名为 SuperNova，可插入芯片中。虽然 OFC 2023 演示中使用的版本支持八种波长，但一年后的 OFC 2024 上，Ayar 推出了升级版的 16 波长 SuperNova，该公司表示它可以“驱动 256 个光载波，实现 16 Tbps 的双向带宽”——Thorn 认为该公司将在未来几年公开展示这一级别的带宽。Thorn 表示，除了改变波长数量外，Ayar 还可以使用“许多其他杠杆”来提高吞吐量，包括在芯片上添加光纤端口，并将每波长的数据调制从目前的 32 Gbps 提高。

Thorn 认为，Ayar 公开展示的“实时硅片”功能稳步提升，是该公司在竞争日益激烈的互连市场中的优势。他说，另一个优势是该公司采用了新兴的通用芯片互连快递 (UCIe) 框架等标准，用于其芯片的电气接口。此外，他指出，Ayar 已与各种公司建立了合作伙伴关系，以推动用例的发展，这些公司包括 GPU 制造商 NVIDIA、瑞典电信公司爱立信、洛克希德、Lumentum、美国国防部，甚至英特尔公司等正在为人工智能开发自己的硅光子解决方案的公司。

然而，在考虑这个市场的竞争时，索恩的态度很哲学。虽然他认识到其他参与者也在寻求利用硅光子学来解决人工智能的带宽挑战，但他相信，让客户摆脱传统电气互连的总体努力将使该领域的所有竞争对手受益。“我们面临的最大挑战之一是围绕电气和铜建立的势头，”索恩说。“如果有人改变这种心态，我们就可以围绕光学和硅光子学启动一个不同的飞轮，这有助于提升所有船只。”

```
Ayar Labs 的 Terry Thorn 表示：“我们面临的最大挑战之一是围绕电气和铜的发展势头。”
```

**互连和 AI 加速器**

另一家年轻公司Lightmatter总部位于美国加利福尼亚州山景城，正在推进人工智能光子学的更广阔愿景，既包括用于处理人工智能数据的光互连，也包括用于加速计算神经网络实际计算的加速器芯片。如果融资进展可以作为参考，那么这一愿景似乎引起了投资者的共鸣：Lightmatter 的最新一轮 C 轮融资于 2023 年 12 月完成，将公司的总估值推高至 12 亿美元，使其稳居“独角兽”行列。

对于 Lightmatter 来说，这是一段令人兴奋的旅程。该公司由 Nicholas Harris、Darius Bunandar 和 Thomas Graham 于 2017 年底创立，当时他们刚刚完成麻省理工学院的研究生学业。Harris 和 Bunandar 当时正在研究用于量子计算的硅光子处理器，而人们对机器学习的兴趣突然爆发，这促使他们将这些可编程平台用于人工智能应用。MBA 学生 Graham 加入了财务部门。

Lightmatter 表示，它“模糊了扩展网络和扩展网络之间的界限”，并特别强调减少人工智能对环境的影响。现任 Lightmatter 首席科学家的 Bunandar 告诉 OPN：“最大的问题是，我们如何为 [人工智能] 提供动力？我们如何为今天将要部署和训练这些模型的超大规模企业提供更快、更高效的计算？……我认为每个人都会同意，托管和训练这些算法所需的能量是相当巨大的。”

```
Lightmatter 表示，它“模糊了扩大规模和扩展规模网络之间的界限”，并且特别致力于减少人工智能对环境的影响。
```

Lightmatter 声称，当前的芯片技术已经达到了其随着人工智能日益增长的需求而扩展的能力的极限。该公司的解决方案是一套由三项技术组成的全栈套件：Passage，一种晶圆级可编程光子互连；Envise，一种光子人工智能加速器芯片；以及 Idiom，一个软件层。

Passage 集成了晶体管和光子学，据 Lightmatter 称，这种组合允许 40 个波导装入一根光纤的空间中。该公司认为，这降低了封装复杂性和成本，同时提高了性能。由于光子互连是内置的，因此无需在芯片和光收发器之间驱动长线迹。Lightmatter 坚持认为，其“显著的互连密度改进”提供了比现有芯片间互连多 10 倍以上的 I/O 带宽，并且可以在五年内实现超过 100 倍的带宽。

Bunandar 表示：“当我们考虑训练和部署这些生成式人工智能算法时，实际上 80% 以上的电力都花在了数据和内存移动上。我们相信 Passage 可以在市场上发挥重要作用，因为它可以节省用于内存到计算以及计算到计算通信的电力。”

Lightmatter 称 Envise 是“世界上第一个光子计算平台”，Bunandar 称 Envise 拥有多个试点客户。作为通用机器学习加速器，它将光子学、电子学和新算法结合到一个模块中，为人工智能量身定制计算平台。Passage 旨在改进芯片的通信方式，而 Envise 则着眼于芯片的计算方式。在 2021 年接受 OPN 采访时 ( optica-opn.org/news/0621-lightmatter )，哈里斯将当时最先进的 NVIDIA 芯片（功耗为 450 W）与 Lightmatter 芯片（功耗仅为 80 W）进行了比较，以突出效率的提高，这符合该公司减少人工智能对环境影响的使命。（不过，目前尚不清楚这两款产品是否具有相同的功能。）

Lightmatter 表示，其一系列产品将满足蓬勃发展的人工智能行业所引发的不断增长的计算需求。“我们认为，需要一种新的计算模式来支持当前的人工智能和下一次人工智能革命，”Bunandar 说。“因此，我们通过推出光子技术来响应这一号召……我们正在彻底改变芯片的计算和通信方式。”

**芯片制造商的尝试**

尽管初创公司和早期公司纷纷抢占人工智能领域的先机，但半导体和网络行业中的老牌公司也并未停滞不前。

例如，在 2024 年 3 月的 OFC 上，半导体巨头英特尔公司推出了自己的光学计算互连 (OCI) 芯片组，并在 6 月的一次大型新闻发布会上扩展了该芯片组的功能（参见 optica-opn.org/news/0624-intel）。该芯片组结合了两个同封装系统——嵌入波导、放大器和密集波分复用激光器的光子集成电路 (PIC)，以及带有控制电路和驱动器的电子集成电路。英特尔集成光子解决方案事业部产品管理和战略高级总监 Thomas Liljeberg 表示，其结果是“紧凑、完全独立的 I/O 系统”，它“连接到 CPU 或 GPU 上的 I/O 端口，将 [电信号] 转换为可通过光纤传输的光信号，并在另一端转换回来。”

在 OFC 2024 演示中，英特尔通过八对光纤（每根光纤八个波长）展示了 CPU 之间的 4 Tbps 双向连接，总功率效率为 5 pJ/bit。“你可以把它想象成 10 W 封装中的 4 Tbps 连接，所以它非常非常高效，”Liljeberg 说。他还补充说，该公司认为“至少五六代带宽将在同一核心技术下翻倍”，通过增加每根光纤的波长数量、每波长的线路速率以及物理连接到芯片的光纤数量等权宜之计。Liljeberg 坚持认为，这些多个扩展旋钮让该公司“有信心，我们正在走上一条健康的道路”，可以支持未来的人工智能数据传输需求。

英特尔过去曾与 Ayar Labs 等公司合作进行演示，它很清楚自己并不是 AI I/O 市场的唯一参与者。但该公司认为它在小芯片领域拥有许多优势。其中之一是它能够将可靠的磷化铟激光器直接大规模集成到其硅片上——该公司指出，它向可插拔收发器市场交付的“超过 3200 万个片上激光器”已经证明了这一点。Liljeberg 向 OPN 指出，集成激光器之所以有意义，很大程度上是因为它们大大降低了外部激光器的耦合损耗，这是一个很大的优势，“在以绝对最佳功率效率为目标的用例中”。

更广泛地说，英特尔认为，在多个层面上集成的专业知识将成为赢得人工智能驱动市场的关键。在这里，该公司强调了其 OCI 芯片的 PIC 层上集成了“超过 2,000 个组件”；该公司在封装和构建“复杂芯片堆栈”方面的专业知识，将 PIC 与 EIC 整合成一个子系统；以及其将该子系统集成到计算平台的能力。“你需要在价值链中发挥所有这些学科和所有这些能力，”Liljeberg 说。

```
活跃的游乐场
以下是众多试图在人工智能数据领域开拓市场的公司的随机样本。

Celestial AI。该公司的产品基于“光子结构”构建，该结构将数据以光的形式编码，不仅传输到 GPU 边缘，还一直传输到“计算点”——计算机芯片上进行数字运算的精确点。该概念的新颖性吸引了大量资金，并与 Celestial 所称的“一些领先的超大规模计算公司”建立了探索性合作伙伴关系，致力于构建“光子结构生态系统”。[optica-opn.org/news/0524-fabric]

POET Technologies。这家总部位于多伦多的集成光子学公司正在强调其“光学中介层”，POET 称其为“有史以来首次将电子和光子集成到单个设备中的晶圆级技术”，这是一种与 CMOS 兼容的平台技术，可用作针对收发器和板载级 AI 应用的共封装光学器件的构建模块。

Ranovus。另一家总部位于加拿大的公司 Ranovus 通过其 Odin 单芯片光学引擎专门针对数据中心的光学互连，该引擎将硅光子 PIC 与片外量子点激光器相结合，用于 AI/ML 工作负载。在 OFC 2024 上，该公司宣布正在与台湾无晶圆厂半导体公司联发科合作开发“6.4 Tbps 共封装光学解决方案”，其“包括激光器在内的能效为 4 pJ/bit”。

Quintessent。总部位于加州的初创公司 Quintessent 将激光源视为 AI 可扩展性的“最薄弱环节”，并希望通过自己的硅光子技术（结合量子点和多波长梳状激光器）来加强这一环节。该公司今年早些时候宣布了 1150 万美元的种子轮融资。[ optica-opn.org/news/0624-quint ]
```

**代工厂方面**

半导体代工厂也参与其中。例如，GlobalFoundries (GF) 是 2009 年从 AMD 制造业务分拆而来的公司，该公司专注于其硅光子平台 GF Fotonix，作为构建 AI 友好型光子互连的解决方案。

GF 硅光子产品管理副总裁 Anthony Yu 于 9 年前加入该公司，自 2017 年以来一直在建立其硅光子业务。GF 早期的努力集中在波导集成和多个电子和光学元件的单片集成上，主要面向可插拔收发器市场。GF Fotonix 最初于 2022 年推出，实际上是第三代产品——Yu 告诉 OPN，“这是我们在 AI 领域的最佳选择。”

GF Fotonix 是一个 300 毫米单片硅技术平台，支持共封装光学元件，并支持 C、L 和 O 波段每波长 200 Gbps。因此，它允许在单个芯片上集成各种光学元件（如调制器、耦合器和多路复用器）和基于 CMOS 的电气元件。GF 声称其集成方法实现了“业界最高的每光纤数据速率”。Yu 强调，GF 目前拥有硅光子学领域“唯一投入生产的 300 毫米单片技术”。

作为一家代工厂，GF 是一家“平台公司”，事实上，它既与光子 AI 处理领域的知名初创公司合作，包括 Lightmatter 和 Ayar Labs，也与在数据中心和 AI 领域拥有股份的规模更大的公司合作，例如 NVIDIA 和 Cisco Systems。“我们谨慎选择合作伙伴，”Yu 说道。特别是，GF 会从战略上寻找“可以合作的初创公司”，这可以推动 GF 在 AI 领域的学习，并且随着时间的推移，随着初创公司的崛起，其代工业务量也会增加。

在代工厂中，GF 很早就开始推进硅光子学。但它并不是唯一一家。例如，2024 年 4 月，全球最大的独立代工厂台湾台积电公布了自己的硅光子学路线图。Yu 认为这种竞争对行业有利——“它提供了选择，”他告诉 OPN，“并让我们变得更加敏锐。”GF 也继续在硅光子学方面投入巨资，并将很快发布第四代单片平台，该平台应能实现每波长 400 Gbps。Yu 认为，GF 的领先优势使其在提供客户现在要求的低成本和大规模可制造性方面具有优势。

作为多年来致力于打造 GF 硅光子学业务的人，Yu 强烈地感觉到，生成式人工智能的出现以及数据瓶颈和能源效率的挑战可能最终推动这项技术向前发展。“现在对光子学的需求就在这里，”他说。“我认为时机已经到来。这就是我们全身心投入其中的原因。”

**网络角度**

在传统的光网络业务中，诺基亚 6 月下旬宣布将以 23 亿美元收购加州的光网络和 PIC 公司Infinera ，这充分表明了集成光子学的潜力。行业观察人士指出，此次收购将使诺基亚进入 Infinera 在数据中心互连 (DCI) 市场和可插拔相干光学领域的产品线。但早在收购宣布之前，Infinera 营销副总裁 Tim Doiron 在一次无关的采访中告诉 OPN，部分由人工智能工作负载刺激的流量大幅增长，以及人工智能提供的改善客户服务和体验的机会，促使该公司对其产品和内部流程进行了不同的思考。

```
诺基亚 6 月底宣布将以 23 亿美元收购光网络和 PIC 公司 Infinera，这充分表明了集成光子学的潜力。
```

一个切实的成果是，Infinera 将目光转向了数据中心本身——打破了过去专注于数据中心之间流量的模式。该公司援引 Cignal AI 分析师的预测，未来四年，数据中心内部互连技术的市场需求将增长近十倍，这在很大程度上是由人工智能工作负载推动的。该公司的一篇博客文章还指出，用于生成人工智能的 GPU 集群每三年就会扩大 10 倍。

为了满足这一惊人的需求，Infinera 于 2024 年 3 月推出了 ICE-D，这是一条基于单片磷化铟 PIC 技术的新型高速数据中心内光学产品线。Infinera 吹捧其光学半导体工厂的“独特功能”，以及磷化铟在数据中心内互连方面的优势，包括低损耗和低功耗要求。该公司表示，ICE-D 组件已证明可将每比特功耗降低多达 75%（这是耗电 AI 应用的一个重要考虑因素），同时提高连接速度，这也是 AI 领域的一个关键因素。

在宣布收购的新闻稿中，诺基亚特别指出 ICE-D 产品线具有战略优势，因为它“特别适合 AI 工作负载，这可能成为非常有吸引力的长期增长机会”。在宣布收购诺基亚时，Infinera 首席执行官 David Heard 也对这种新产品的多样性表示认可。“我们相信诺基亚是一家优秀的合作伙伴，”他说，“我们将共同拥有更大的规模和更深厚的资源，以设定创新步伐，并在光学比以往任何时候都更重要的时代满足快速变化的客户需求——在电信网络、数据中心间应用以及现在的数据中心内部。”

正如 Heard 所说，数据中心之间也感受到了人工智能和机器学习工作负载带来的流量激增，这进一步推动了 Infinera 的核心 DCI 业务。随着容量需求不断上升，Infinera 正在寻求扩大可用频谱，以帮助网络运营商管理带宽需求。据 Doiron 称，该公司认为现在是将 C 波段从目前的 4.8 THz 扩展到 6.1 THz 传输空间，进入所谓的 Super-C 波段的正确时机。“经济性和性能都足以实现这一点，”Doiron 说，“让您在现有光纤上额外增加 27% 的容量，而无需铺设更多光纤。”

AI 提供的功能也启发了该公司反思自己的流程。“当我们审视 AI 时，我们会看到两个方面。一方面是网络带宽需求的额外驱动因素，”Doiron 解释道。“但同时，这也是我们审视自身业务、审视我们如何为客户提供解决方案以及如何帮助客户的机会。”网络健康预测就是这样一种应用，它可以利用 AI 预测网络问题并提前做出响应。此外，AI 还可用于客户服务以及规划和执行营销活动。

“虽然现在还处于早期阶段，但我们将继续增强和完善人工智能。我们将解决日益复杂的问题，”Doiron 说道。“我真的认为人工智能有能力改变我们网络的可靠性、弹性和可预测性，并真正在许多方面提高我们工作的效率和速度。现在是从事重要创新的好时机。”

**人工智能作为业务优化器**

Infinera 不仅将 AI 作为新业务领域，还将其用于改进现有运营，这并不是孤例，而是整个光子学行业的趋势。为了了解 AI 在这方面的影响，我们采访了德国 Jenoptik，了解该公司如何将 AI 融入现有产品和流程。这家全球集成光子学公司的历史可以追溯到 19 世纪末卡尔蔡司、恩斯特阿贝和奥托肖特的研究伙伴关系，在利用技术发展方面拥有丰富的经验——而 AI 的发展也不例外。

“AI 对我们来说真的不是一个新话题……它已经在我们的光学领域和客户中应用了很多年，”Jenoptik 数字化转型和创新总监 Adrian König 解释道。“从战略上讲，AI 和机器学习使我们能够增强现有产品套件并为客户创新新产品。将 AI 驱动的分析融入我们的光子产品中，使我们能够为客户提供更精确、更可靠的解决方案。或者在图像处理领域——就 AI 而言，这对我们来说确实是一件大事——我们改变了客户获取所需信息的方式。”

Jenoptik 企业创新项目经理 Subhasis Pradhan 表示，该公司早在 2017 年就开始采用人工智能来改进其产品，这远早于 2022 年 11 月推出的 ChatGPT 引发的关注爆发。2017 年的项目面向汽车行业，涉及将神经网络应用于图像处理以检查螺钉头是否有缺陷。高分辨率摄像系统与在大量无错误组件数据集上训练的神经网络相结合。然后，它们可以自主准确地识别生产部件是否符合规定的质量要求。

这一计量应用为 Jenoptik 随后在其他领域使用人工智能奠定了基调。该公司强调，要找到一个用例来为客户创造价值，而不是为了自身利益而进行创新。正如 Pradhan 所说：“我们看到了人工智能或机器学习的价值，但更重要的是将商业机会与技术机会结合起来。” König 进一步阐述了这一观察：“归根结底，问题本身并不是我们关注的重点。我们关注的重点是如何为客户解决问题。”

```
Jenoptik 的 Adrian König 解释道：“从战略上讲，人工智能和机器学习使我们能够增强现有的产品套件并为我们的客户创新新产品。”
```

该公司的三个部门之一 Smart Mobility 从 AI 的整合中获得了特别显著的好处。该部门为民用安全和执法部门部署了支持 AI 的自动车牌识别 (ALPR)，以及支持 AI 的收费系统。这些系统将 Jenoptik 的 VECTOR 2 ALPR 摄像头（可自动捕获车辆牌照）与深度学习软件配对，后者可访问现有的图像组合，以提高捕获率，即使在具有挑战性的环境中也能更成功地读取完整的车牌。

另一家采用整体 AI 方法的公司是全球激光和机床巨头通快公司 (Trumpf)。该公司一直直言不讳地表示，计划将 AI 融入其运营的各个方面。在今年 4 月的新闻发布会上，通快首席技术官 Berthold Schmidt 表示：“五年后，我们希望成为行业内领先的 AI 解决方案用户和领先提供商。到那时，通快的所有工作都应该与 AI 息息相关。”该公司目前提供 AI 解决方案，用于对切割部件进行分类或改进机床中的装配设计，以及激光技术中的工艺控制。7 月中旬，通快宣布与机器学习初创公司 SiMa.ai 合作，为激光系统配备 SiMa 的 AI 芯片，旨在改进焊接、切割和打标工艺。通快还希望提高其内部职能的效率，例如其正在试行类似 ChatGPT 的模型，为服务工程师提供故障的可能解决方案。

总结 Jenoptik 的 AI 理念，König 说道：“我们希望通过光子学创造更美好的未来。牢记这一目标，我们将 AI 视为我们市场的推动者。我们非常乐观地认为，AI 将继续保持这种状态，我们将继续为客户创造更多价值。”

<https://www.optica-opn.org/home/articles/volume_35/september_2024/features/photonics_and_ai_industry_perspectives/?utm_content=305005905&utm_medium=social&utm_source=linkedin&hss_channel=lcp-6627049>

# 17. Bechtolsheim在Hotchips上关于Micro LED进展的讨论

Bechtolsheim 预计到 2028 年 XPU 性能将提升 100 倍

说到提高计算引擎性能，效果是乘法的，而不是加法的。如果有一个人不担心我们如何在未来六年内将这些引擎的性能提高两个数量级，那就是 Andy Bechtolsheim。

好吧，至少 Bechtolsheim 似乎并不太担心。这是我们从他最近在硅谷举行的 Hot Interconnects 2024 会议上的主题演讲中得到的印象，在演讲中，系统和网络业务的一位杰出人物大声质疑到本世纪末，I/O 能否跟上用于 AI 加速的 XPU 设计的计算速度。然后 Bechtolsheim 抓住了我们所有人的耳朵，在 21 分钟内讲完了 38 张幻灯片，证明我们半导体行业已经做到了这一点。

鉴于贝希托尔斯海姆在科技行业长期的观察和创新，当贝希托尔斯海姆讲话时，人们会认真倾听。贝希托尔斯海姆是著名的 Sun Microsystems 创始人之一，1995 年他与 David Cheriton 共同创立了千兆以太网交换机制造商 Granite Systems，思科系统一年后收购了该公司，以便在互联网泡沫开始之际从路由业务扩展到交换机业务时获得更好的立足点。（贝希托尔斯海姆和 Cheriton 是谷歌的首批两位投资者，他们因出售 Granite Systems 而致富。）2001 年，在互联网泡沫破灭后，贝希托尔斯海姆创立了 InfiniBand 系统制造商 Kealia，2004 年 Sun Microsystems 收购 Kealia 后，该公司被 Sun Microsystems 以 Constellation 系统的形式商业化。一年后，贝希托尔斯海姆、Cheriton 和 Ken Duda 共同创立了 Arista Networks，从那时起他们就一直在那里工作。

我们将为您提供 Bechtolsheim 的主要观点，即如何从现在到 2028 年将 XPU 性能提高至少 50 倍，并可能通过液体冷却技术的进步提高 100 倍。

![image](/picture/andy-hoti-process-technology-improvements-600x292.jpg)

通过将台湾半导体制造公司的 5 纳米工艺缩小到 2 纳米，晶体管密度可提高 50%，性能可提高 33%，同时功耗保持不变。如果将这些乘以 1，则在相同的散热条件下，性能可提高 2 倍。

如果你比 Bechtolsheim 更进一步，看看英特尔 14A 和台积电 A14 工艺预计在 2026 年推出，第二年进行调整，这些工艺将在 2028 年成熟。与台积电目前的 5 纳米工艺相比，这将使芯片性能提升约 2.5 倍。考虑到这种适度的性能提升，你就可以明白为什么 Bechtolsheim 不费心了。2 倍很重要。再增加 0.5 倍，就没那么重要了。

但当机会来临的时候，我们将会接受它。

无论是 2 倍还是 2.5 倍，关键在于，在六年内，它都不会有太大的进步，而且它还不到 20 世纪 90 年代和 21 世纪摩尔定律密度和性能改进的正常速度的一半，而且我们预计到那时它的发热量会更高。因此，为了提高每个 XPU 的性能，XPU 必须变得更大。这也是 XPU 系统板将缩减为 XPU 插槽的原因之一。

台积电对其晶圆系统 (System on Wafer) 的情况是这样看待的，Bechtolsheim 引用道：

![image](/picture/andy-hoti-system-on-wafer.jpg)

这些封装越来越大，其各个组件也变得越来越热，因此这些 XPU 的热密度基本上每两年就会翻一番。Bechtolsheim 使用的基准是 2022 年 XPU 的平均功耗为 600 瓦，今年每 XPU 的功耗为 1,000 瓦，到 2026 年将跃升至 2,000 瓦，到 2028 年将达到惊人的 4,000 瓦。

无论如何，将所有这些加起来，你会发现在 2022 年至 2028 年期间，XPU 性能将提高 55.4 倍，而发热量将增加 6.7 倍。据我们所知，这并不假设任何计算芯片的 3D 堆叠，但如果在此基础上添加 3D 元素，密度可能会增加一个与计算堆栈数量相关的倍数。重要的是，通过巧妙的冷却——Bechtolsheim 没有具体说明，因为这不是他演讲的目的——与 2022 年的 XPU 相比，你可以将这一数字再翻一番，使计算性能提高 100 倍以上。

![image](/picture/andy-hoti-future-gpu-performance-600x314.jpg)

假设性能类型（矢量和张量）和数值精度（从 FP64 到 FP8）的平衡与当前的“Hopper”H100 GPU 大致相同，那么根据我们的计算，未来在英特尔 14A-E 或台积电 A14 中实现的 Nvidia GPU 的性能可能比 H100 高 65.4 倍。Bechtolsheim 提到的液体冷却提升将差距缩小到 100 倍，我们推测这意味着对所有东西进行超频，并用液体冷却系统中的每个元素。这样的 Z100 GPU（是的，我们编造的）将具有 345 万亿次浮点运算的 FP64 矢量性能和 670 万亿次浮点运算的 FP64 张量性能，以及 9.8 千万亿次浮点运算的 FP16 张量性能，用于 AI 工作和低精度 HPC 工作。

只有天知道这种装置要花多少钱……这也不是贝克托尔斯海姆的部门。

您可能会认为，该 XPU 复合体（芯片大小超过 40 个光罩，HBM 超过 60 个存储体 - 60 个存储体！）的 I/O 功率绝对巨大。但事实证明，I/O 功率（基本上是连接到每个 XPU 的以太网 NIC）似乎将保持在 XPU 本身消耗功率的 2.5% 左右。Bechtolsheim 的计算方法如下：

![image](/picture/andy-hoti-future-io-bandwidth-600x340.jpg)

有趣的是，Bechtolsheim 认为，800 Gb/秒以太网端口将添加到 XPU 中，随着 XPU 路线图的推进，功耗将稳定在每比特 4 皮焦耳，功耗也将保持相对稳定，占总功耗的 2.5%。同样有趣的是，每个 XPU 的 I/O 带宽似乎将增加 8 倍，即使采用 2 纳米工艺实现的 XPU 的性能可能会提高 55.4 倍，如果采用 1.4 纳米工艺，性能可能会提高 65.4 倍，如果采用更先进的冷却技术，性能可能会提高 100 倍，但 I/O 带宽只会增加 8 倍。

我们强烈怀疑这些 XPU 的以太网端口数量将超过上述数字，如果可能的话，端口运行速度可能达到 1.6 Tb/秒，甚至达到 3.2 Tb/秒。但正如您所想象的，很难与 Bechtolsheim 争论这一点。我们没有机会要求解释 XPU 性能与 I/O 之间的差距，但我们发现这种差异很有趣。

Bechtolsheim 所看到的用于从 XPU 芯片获取数据的芯片到芯片接口和高速 SerDes 是这样的：

![image](/picture/andy-hoti-chip-level-interconnects-600x331.jpg)

“在扩展社交基板的 IO 带宽时，随着基板的增加，我们将获得更多的前沿，从而提供比以往更多的 IO，”Bechtolsheim 解释道。“因此，假设当今高速 SerDes 的前沿为每毫米 1 兆位，在 25 x 25 毫米的单个芯片上，那就是 100 兆位。对于更大的基板芯片，即 50 毫米 x 50 毫米，那就是 200 兆位。对于更大的基板芯片，即 100 毫米 x 100 毫米的多芯片基板，将有 400 兆位 - 这是使用 200 Gb/秒 SerDes 技术。如果使用 400 Gb/秒 SerDes，可能会翻倍到 800 兆位，所以这些都不是限制。”

“归根结底，这取决于这些元件之间的距离，使芯片死亡时功耗大大降低。功耗可能是每比特 0.2、0.3 或 0.4 皮焦耳。而且由于你可以堆叠行，因此你可以获得每毫米 5 兆兆位到 10 兆兆位的芯片外数据。这更难，因为你要驱动更远的距离，你需要更多的功率和更多的驱动器才能做到这一点。但似乎仍然可以将每比特的数据从 1 兆兆位提高到甚至 2 兆兆位。

现在，这些都不再是限制，我想在此强调高 SerDes 作为通用接口的作用。我将其称为通用电气接口，用于支持铜缆、AOC 电缆或任何类型的光学模块的任意组合。这里有一个明确的路线图，从今天出货的 112G，到即将推出的 224G，以及未来的 448G。还有一个匹配的光学模块，路线图从今天的 800G 千兆模块到八通道光学的 1,600G 和 3,200G。”

正如许多人所说和所做的那样，以及 Nvidia 最近对120 千瓦 GB200 NVL72 机架级系统所做的那样，您坚持使用 XPU 之间的铜缆，并尽可能将铜缆直接从交换机 ASIC 上移除，以降低成本。光学器件非常非常昂贵，也更容易出现故障。而且，您可以提高机架的计算密度（从而提高机架的热密度），以减少 XPU 之间的距离，因为它们的 AI 工作负载（以及附带的 HPC 工作负载）对延迟非常敏感。据 Bechtolsheim 称，人们目前正在为此目的设计可承载 400 千瓦甚至 500 千瓦功率的机架。

挑战在于你必须超越机架并将一排机架或整个数据中心的机架连接在一起。

好消息是，运行速度为 1.6 Tb/秒的以太网光收发器与传输速度为 800 Gb/秒的收发器具有相同数量的驱动器、激光器、检测器、光纤和连接器。通道以 200 Gb/秒（扣除开销后）而不是 100 Gb/秒的速度移动。最大的问题是功率。使用 DSP 的收发器的运行功率为 30 瓦，使用线性接收光学 (LRO) 方法的收发器的运行功率为 20 瓦，但线性驱动可插拔光学（由于某种原因缩写为 LPO）仅为 10 瓦。对于 102.4 Tb/秒的交换机，使用 LPO 的运行功率为 800 瓦，使用 LRO 的运行功率为 1,600 瓦，使用 DSP 的运行功率为 2,400 瓦。

![image](/picture/andy-hoti-1600g-dr8-power.jpg)

您可以看到为什么 Bechtolsheim 一直是 LPO 方法的拥护者，该方法使用与近封装光学器件或共封装光学器件相同的方法，但将所有电路保留在可插拔模块中，而不是试图塞进开关盒中。

根据 Bechtolsheim 的说法，微型 LED 光学器件的进给和速度如下：

![image](/picture/andy-hoti-1600g-osfp-4g-microled.jpg)

以下是基于 32 Gb/秒 NRZ 微环的 1.6 Tb/秒 OSFP 模块的堆叠方式：

![image](/picture/andy-hoti-1600g-osfp-32g-nrz.jpg)

后者的功率比微型 LED 方法略高一点，与 LPO 可插拔模块的功率大致相同。

后两种技术方法非常令人兴奋（我们将分别深入探讨），但 Bechtolsheim 担心大批量生产会降低成本。如今，你需要获得超大规模企业或云构建商的设计许可才能开始，而这些很难获得。

Bechtolsheim 介绍了一些历史，提醒大家 IBM 为 Power 775 超级计算机服务器节点进行了联合封装的光学器件，该节点应该是最初的“Blue Waters”超级计算机的核心，该超级计算机是为伊利诺伊大学的国家超级计算应用中心设计的，其开发资金来自十五年前的美国国防高级研究计划局。

![iamge](/picture/andy-hoti-cpo-power-775.jpg)

IBM 于 2010 年推出了 Power 775 服务器及其光纤互连，并于 2011 年 8 月停止实施 Blue Waters 机器。我们猜测，IBM 必须提供一台具有 2 petaflops 的机器来支持 NCSA 在 Blue Waters 合同中要求的高性能 LINPACK 测试中的 1 petaflops 性能。我们猜测，这台机器的制造成本可能为 3 亿美元，而且它不一定能为蓝色巨人带来利润。（顺便说一下，这台机器上的所有东西都是液体冷却的，节点确实是一项工程壮举。）当 IBM 停止实施时，Cray 与 NCSA 达成了一项价值 1.88 亿美元的交易，以构建一个以 Blue Waters 命名的混合 CPU-GPU 系统。从那时起，NCSA 停止在其机器上运行 HPL，并停止参与 Top500 超级计算机排名。

Blue Waters 的重点是可制造性。CPO 已经存在很长时间了，制造起来很困难，当用于驱动信号的激光器嵌入到使用它们的设备中时，很难避免激光器出现故障。

Bechtolsheim 通过对 100,000 个 XPU 集群的 DSP 光学器件和 LPO 光学器件之间的功率进行比较，强调了另一个重要观点——关于网络的热量。请看：

![image](/picture/andy-hoti-power-savings-100k-cluster-600x308.jpg)

Bechtolsheim 的思想实验中的 XPU 具有 25.6 Tb/秒的总网络 I/O 带宽，顺便说一句，这相当于当今常见的中端以太网交换机 ASIC。这被分解为 16 个以 1.6 Tb/秒运行的端口，以计算光收发器的数量。要互连 100,000 个 XPU，需要令人难以置信的 640 万个光学器件。

如果你算一下，LPO 光学器件将消耗 64 兆瓦的电力，略低于橡树岭国家实验室的整个“Frontier”超级计算机消耗的 22.7 兆瓦的三倍。使用 DSP 光学器件，消耗的功率为 192 兆瓦，是 LPO 光学器件的三倍。这几乎是这 100,000 个 XPU 预计消耗的 400 兆瓦的一半。

“毋庸置疑，没有人会为这种应用部署基于 DSP 的光学器件，因为买不起，”Bechtolsheim 说。“所以我们需要线性光学器件。”

即使我们对微型 LED 方法的可能性感到兴奋，但这一点很难争论。我们将让那些致力于此的人很快在The Next Platform上提出这些论点。

<https://www.nextplatform.com/2024/08/26/bechtolsheim-outlines-scaling-xpu-performance-by-100x-by-2028/>

# 18.光学

## 18.1 新型微芯片装置可产生多种激光色调

美国国家标准与技术研究所 (NIST) 和马里兰大学的研究人员开发出一种微芯片技术，可以将不可见的近红外激光转换成各种可见激光颜色，包括红色、橙色、黄色和绿色。他们的工作为在集成微芯片上产生激光提供了一种新方法。

该技术可应用于精密计时和量子信息科学，这些领域通常依赖于原子或固态系统，这些系统必须由波长精确指定的可见激光驱动。该方法表明，使用单个小型平台即可获得各种波长，而无需笨重的台式激光器或一系列不同的半导体材料。在微芯片上构建此类激光器还提供了一种低成本方法，可将激光器与光学时钟和量子通信系统所需的微型光学电路集成在一起。

该项研究发表于 10 月 20 日的《Optica》杂志，为“NIST on a Chip”计划做出了贡献，“NIST on a Chip”计划旨在将 NIST 最先进的测量科学技术小型化，使其能够直接分发给工业、医学、国防和学术界的用户。

作为最精确、最准确的实验时钟和量子信息科学新工具的核心的原子系统通常依靠高频可见（光学）激光来运行，而不是用来设定世界各地官方时间的低频微波。

科学家们目前正在开发紧凑且低功率的原子光学系统技术，以便它们可以在实验室外使用。虽然实现这一愿景需要许多不同的要素，但一个关键要素是获得体积小、重量轻且低功率的可见光激光系统。

尽管研究人员在制造用于电信的近红外波长的紧凑型高性能激光器方面取得了巨大进展，但要在可见光波长下实现同等性能却是一项挑战。一些科学家通过使用半导体材料来产生紧凑型可见光激光器取得了进展。相比之下，NIST 和马里兰大学帕克分校的 Xiyuan Lu、Kartik Srinivasan 及其同事采用了不同的方法，专注于一种名为氮化硅的材料，这种材料对光具有明显的非线性响应。

**<font color=red>氮化硅等材料具有一种特殊性质：如果入射光的强度足够高，则出射光的颜色不一定与入射光的颜色相匹配。这是因为当非线性光学材料中的束缚电子与高强度入射光相互作用时，电子会以不同于入射光的频率或颜色重新辐射该光。</font>**

（这种效果与我们每天看到的光从镜子反射或通过镜头折射的体验形成对比。在这些情况下，光的颜色始终保持不变。）

卢和他的同事采用了一种称为三阶光学参量振荡 (OPO) 的过程，其中非线性材料将近红外的入射光转换为两个不同的频率。其中一个频率高于入射光，将其置于可见光范围内，另一个频率较低，延伸到红外深处。尽管研究人员多年来一直使用 OPO 在大型桌面光学仪器中创造不同颜色的光，但这项由 NIST 领导的新研究是首次将这种效应应用于具有大规模生产潜力的微芯片上产生特定的可见光波长。

为了使 OPO 方法小型化，研究人员将近红外激光引入微谐振器，这是一种面积不到百万分之一平方米的环形装置，制造在硅片上。这个微谐振器内的光在消散前循环约 5,000 次，强度足够高，可以进入非线性状态，然后转换为两个不同的输出频率。

为了创造多种可见光和红外光，该团队在每个微芯片上制作了数十个微谐振器，每个微谐振器的尺寸略有不同。研究人员精心选择了这些尺寸，以便不同的微谐振器能够产生不同颜色的输出光。该团队表明，这种策略使波长变化相对较小的单个近红外激光器能够产生各种特定的可见光和红外光。

具体来说，尽管输入激光在近红外波长（780 纳米至 790 纳米）的窄范围内工作，但微芯片系统产生的可见光颜色范围从绿色到红色（560 纳米至 760 纳米），红外波长范围从 800 纳米至 1,200 纳米。

斯里尼瓦桑说：“我们方法的好处是，只要调整微谐振器的尺寸，就可以获得其中任何一个波长。”

卢教授表示：“尽管这是首次演示，但我们很高兴能够将这种非线性光学技术与成熟的近红外激光技术结合起来，创造出可用于各种应用的新型片上光源。”

<https://opg.optica.org/optica/fulltext.cfm?uri=optica-7-10-1417&id=441023>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/On-chip%20optical%20parametric%20oscillation%20into%20the%20visible%20generating%20red%2C%20orange%2C%20yellow%2C%20and%20green%20from%20a%20near-infrared%20pump.pdf>

## 18.2 片上光源可产生多种波长范围

研究人员设计了一种新型芯片集成光源，可以将红外波长转换为可见波长，而这在基于硅芯片的技术中很难实现。这种灵活的芯片上光生成方法有望实现高度微型的光子仪器，这种仪器易于制造，坚固耐用，可在实验室外使用。

在光学学会 (OSA) 的影响力研究期刊《Optica 》中，来自美国国家标准与技术研究所 (NIST)、马里兰大学和科罗拉多大学的研究人员介绍了他们的新型光参量振荡器 (OPO)光源，并表明它可以产生与输入光颜色或波长截然不同的输出光。除了产生可见波长的光外，OPO 还同时产生可用于电信应用的近红外波长。

研究团队负责人 Kartik Srinivasan 表示：“我们的方法节能灵活，能够产生波长范围比直接芯片集成激光器更宽的相干激光。可见光的芯片生成可用作功能强大的紧凑型设备的一部分，例如基于芯片的原子钟或便携式生化分析设备。在硅光子学平台上开发 OPO 为在商业制造工厂中可扩展制造这些设备创造了潜力，从而使这种方法非常具有成本效益。”

**利用非线性过程**

尽管材料对光的响应通常呈线性变化，但材料特性在高功率光下会以更快的速度发生变化，从而产生各种非线性效应。OPO 是一种利用非线性光学效应产生非常宽范围输出波长的激光器。

研究人员希望弄清楚如何利用紧凑型芯片激光器发射波长范围内的激光，并将其与非线性纳米光子学相结合，以产生硅光子平台难以达到的波长范围内的激光。

“非线性光学技术已被用作世界上最好的原子钟和许多实验室光谱系统中激光器的组成部分，”该论文的第一作者、NIST-马里兰大学博士后学者 Xiyuan Lu 说道。“能够在集成光子学中访问不同类型的非线性光学功能（包括 OPO），对于将目前基于实验室的技术转变为便携式且可在现场部署的平台非常重要。”

**在这项新研究中，研究人员设计了一种基于氮化硅微环的 OPO。该光学元件由大约 1 毫瓦的红外激光功率供电，大约与激光笔中的功率相同。当光在微环周围传播时，其光强度会增加，直到强度足以在氮化硅中产生非线性光学响应。这可以实现频率转换，这是一种非线性过程，可用于产生与进入系统的光不同的输出波长或频率。**

“纳米光子工程的最新进展使得这种频率转换方法非常高效，”卢说。“我们工作中的一个关键进展是弄清楚如何促进感兴趣的特定非线性相互作用，同时抑制可能在此系统中出现的潜在的竞争非线性过程。”

**测试光源**

研究人员利用详细的电磁模拟设计了新的片上光源。然后，他们制作了该设备，并用它将 900 纳米的输入光转换为 700 纳米波长（可见光）和 1300 纳米波长（电信）波段。OPO 实现这一目标所需的泵浦激光功率不到之前报道的微谐振器 OPO 所需功率的 2%，而微谐振器 OPO 是为产生相差很大的输出颜色而开发的。在之前的案例中，产生的两种颜色都是红外光。通过对微环尺寸进行一些简单的更改，OPO 还可以产生 780 纳米可见光和 1500 纳米电信波段的光。

研究人员表示，通过将廉价的商用近红外二极管激光器与集成了滤光片、探测器和光谱部分等组件的 OPO 芯片相结合，新的 OPO 可用于构成一个完整的系统。他们正在继续寻找增加 OPO 输出功率的方法。

“这项研究表明非线性纳米光子学已达到成熟水平，我们可以创建一种连接相隔很远的波长的设计，然后实现足够的制造控制，在实践中实现该设计和预期的性能，”Srinivasan 说道。“展望未来，应该能够使用少量紧凑型芯片激光器结合灵活多变的非线性纳米光子学来生成各种所需波长。”

更多信息： X. Lu、G. Moille、A. Singh、Q. Li、DA Westly、A. Rao、S.-P. Yu、T​​C Briles、SB Papp 和 K. Srinivasan，“利用硅纳米光子学实现毫瓦阈值可见光-电信光学参量振荡”，Optica，6，12，1535-1541 (2019)。DOI：doi.org/10.1364/OPTICA.6.001535

论文链接
<https://opg.optica.org/optica/fulltext.cfm?uri=optica-6-12-1535&id=424681>

<https://phys.org/news/2019-12-on-chip-source-versatile-range-wavelengths.html>

## 18.3 微型新型激光器填补了可见光彩虹色的长期空白，开辟了新的应用

![image](/picture/tiny-new-lasers-fill-a.jpg)
微环谐振器产生的一系列可见光颜色。来源：S. Kelley/NIST

制造绿光并不容易。多年来，科学家们已经制造出能发出红光和蓝光的小型高质量激光器。然而，他们通常采用的方法——将电流注入半导体——在制造发射黄光和绿光波长的微型激光器时效果并不好。

研究人员将可见光光谱这一区域内缺乏稳定、微型激光器这一现象称为“绿色空白”。填补这一空白将为水下通信、医疗等带来新的机遇。

绿色激光笔已经存在了25年，但它们只能发出窄光谱的绿光，而且没有集成在芯片中，无法与其他设备协同执行有用的任务。

![image](/picture/tiny-new-lasers-fill-a-1.jpg)

紧凑型激光二极管可以发射红外、红光和蓝光波长，但在产生绿光和黄光波长方面效率极低，这一区域被称为“绿隙”。图片来源：S. Kelley/NIST

现在，美国国家标准与技术研究院 (NIST) 的科学家通过修改一个微小的光学元件缩小了绿色差距：一个环形微谐振器，小到可以装在芯片上。这项研究发表在《光：科学与应用》杂志上。

微型绿色激光光源可以改善水下通信，因为在大多数水生环境中，水对蓝绿波长几乎是透明的。其他潜在应用包括全彩激光投影显示器和医疗状况的激光治疗，包括糖尿病视网膜病变，即眼部血管增生。

这一波长范围内的紧凑型激光器对于量子计算和通信应用也很重要，因为它们有可能将数据存储在量子比特中，量子比特是量子信息的基本单位。目前，这些量子应用依赖于体积、重量和功率较大的激光器，这限制了它们在实验室外部署的能力。

多年来，由 NIST 和联合量子研究所 (JQI，NIST 与马里兰大学的研究合作伙伴) 的 Kartik Srinivasan 领导的团队一直使用由氮化硅组成的微谐振器将红外激光转换为其他颜色。当红外光被泵入环形谐振器时，光会旋转数千次，直到达到足以与氮化硅强烈相互作用的强度。这种相互作用称为光学参量振荡 (OPO)，会产生两种新波长的光，称为闲置光和信号光。


![image](/picture/tiny-new-lasers-fill-a-2.jpg)
红外激光（称为泵浦光）被发射到环形微谐振器中，并通过光学参量振荡转换成两种新波长的光，称为信号光和闲置光（顶部）。信号光的波长位于可见光范围内，而闲置光的红外波长比泵浦激光的波长更长。由于能量守恒，两个泵浦光子携带的能量必须等于两个输出波长中单个光子携带的能量之和（右下）。图片来源：S. Kelley/NIST

在之前的研究中，研究人员生成了几种不同颜色的可见激光。根据微谐振器的尺寸（决定了生成的光的颜色），科学家生成了红色、橙色和黄色波长，以及波长为 560 纳米的光，波长正好位于黄色和绿色光之间的边缘。然而，该团队无法生成填补绿色空白所需的全部黄色和绿色。

“我们不想只擅长探测几种波长，”新研究的合作者、美国国家标准与技术研究院的科学家孙毅 (Yi Sun) 表示。“我们希望探测到间隙中的整个波长范围。”

为了填补这一空白，研究小组以两种方式修改了微谐振器。首先，科学家们稍微加厚了它。通过改变其尺寸，研究人员更容易产生能够深入绿色间隙的光，波长短至 532 纳米（十亿分之一米）。通过扩大范围，研究人员覆盖了整个间隙。

此外，该团队还通过蚀刻掉下方的部分二氧化硅层，将微谐振器暴露在更多空气中。这使得输出颜色对微环尺寸和红外泵浦波长的敏感度降低。较低的灵敏度使研究人员能够更好地控制从他们的设备产生略有不同的绿色、黄色、橙色和红色波长。

![image](/picture/tiny-new-lasers-fill-a-3.jpg)
传统的微谐振器（顶部）通过 OPO 产生的波长有限。通过部分蚀刻掉微谐振器下方的二氧化硅薄膜以形成“底切”并使用更厚的氮化硅层（底部），NIST 研究人员能够覆盖整个“绿色间隙”光谱范围，同时还可以提高所产生波长的密度。图片来源：S. Kelley/NIST

结果，研究人员发现他们可以在绿色间隙中创建 150 多种不同的波长并对其进行微调。“以前，我们可以对使用 OPO 产生的激光颜色进行大幅度的改变——从红色到橙色到黄色再到绿色——但很难在每个色带内进行细微的调整，”Srinivasan 指出。

通过改变红外泵的波长，NIST 研究人员可以在整个绿色间隙中产生可见光波长。底部的视频由研究人员拍摄，描述了这一过程。图片来源：S. Kelley/NIST
科学家们目前正在努力提高产生绿隙激光颜色的能量效率。目前，输出功率仅为输入激光功率的百分之几。输入激光和将光引导到微谐振器的波导之间更好的耦合，以及更好的提取产生的光的方法，可以显著提高效率。

作者包括 JQI 的 Jordan Stone 和 Xiyuan Lu，以及华盛顿州雷德蒙德 Meta 现实实验室研究公司的 Zhimin Shi。

更多信息： Yi Sun 等人，推进片上克尔光学参量振荡向覆盖绿隙的相干应用发展，光：科学与应用(2024)。DOI：<10.1038/s41377-024-01534-x>

论文链接
<https://www.nature.com/articles/s41377-024-01534-x>

<https://phys.org/news/2024-08-tiny-lasers-gap-rainbow-visible.html>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Advancing%20on-chip%20Kerr%20optical%20parametric%20oscillation%20towards%20coherent%20applications%20covering%20the%20green%20gap.pdf>

# 19. Recent progress on micro-LEDs - Nanowire

随着增强现实/虚拟现实 (AR/VR) 等技术的发展，它们正朝着高效、小尺寸和超高分辨率的显示器方向发展，开发尺寸在几微米甚至更小的光电器件引起了人们的极大兴趣。在这篇评论文章中，我们概述了可见微米级发光二极管 (LED) 的一些最新发展。我们讨论了较小尺寸器件的更高表面复合、实现更长发射波长的难度以及将单个全彩色器件集成到显示器中的复杂性等主要挑战，以及为解决这些问题而开发的技术。然后，我们介绍了自下而上基于纳米结构的亚微米 LED 的最新研究，重点介绍了它们的独特优势、最新发展和广阔的潜力。最后，我们提出了未来发展微型 LED 的前景，以实现更高的效率、更好的色彩输出和更高效的集成。

<https://www.light-am.com/article/doi/10.37188/lam.2023.031>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Recent%20progress%20on%20micro-LEDs.pdf>

# 20. Data communication using blue GaN-on-Si micro-LEDs reported on a 200-mm Silicon substrate 格勒诺布尔大学

报告称，在 200 毫米硅基板上使用蓝色 GaN-on-Si 微型 LED 进行数据通信

本文报道了在 200 毫米硅基板上制造的氮化镓 (GaN) 蓝色微发光二极管 (μLED) 用于多 Gb/s 数据传输。制造工艺与 CMOS 集成电路设计兼容，为基于 μLED 的可见光通信 (VLC) 或芯片间互连的全集成发射器铺平了道路。使用直流光正交频分复用 (DCO-OFDM) 调制实现了光纤引导传输，并且报道了使用单个 50×50 μm 2 蓝色 μLED 的 数据速率为 5.9 Gb/s，误码率 (BER) 为 3.8×10 -3 。在 μLED 仅受其非线性失真而非系统噪声限制的情况下，该数据速率进一步提高到 15.5 Gb/s，突显了 GaN μLED 的高线性度。

通信作者 Yannis Le Guennec

Yannis Le Guennec 于 2000 年获得法国格勒诺布尔国立物理学院工程师学位，并于 2003 年获得格勒诺布尔理工学院光学光电子学和微波博士学位。他目前是微电子、电磁学和光子学研究所 (IMEP-LAHC) 的助理教授。他感兴趣的领域是微波光子学、全光信号处理、超宽带 (UWB) 通信和光纤无线电技术。

<https://ieeexplore.ieee.org/document/10654359>

# 21. 注入电流对量子点发光二极管调制带宽的影响

本文介绍了量子点 (QD) 发光二极管 (QLED) 的调制带宽研究。我们研究中使用的 QLED 是红光发射 CdSe/ZnS QLED，其结构为氧化铟锡 (ITO)/聚（3.4-乙烯二氧噻吩）聚苯乙烯磺酸盐 (PEDOT:PSS)/TFB/QD/ZnO/Al，发射面积为 2 或 4 mm 2 。我们发现，在较小的注入电流（低于 ~10 mA）下，电阻电容 (RC) 时间常数和载流子寿命对 QLED 带宽的影响相当，而在较大的注入电流下，带宽主要由载流子寿命决定。QD 的响应时间不是限制因素。QLED 的带宽随注入电流的增加而增加，最终受器件损伤阈值电流的限制。在相同的注入电流下，发光面积较小的QLED具有较大的电流密度，因而具有较大的带宽。在注入电流为28 mA时，2 mm 2 QLED提供11.4 MHz的带宽和156 000 cd/m 2的亮度值 ，而4 mm 2 QLED提供8.2 MHz的带宽和97 000 cd/m 2的亮度值 。我们的研究为QLED带宽优化提供了指导方针，并为QLED在照明、显示和通信应用方面的进一步开发提供了有用信息。

The relationship between the response time τ and the modulation bandwidth f is given by f=1 /(2πτ ). If the bandwidth of the QLED was limited by the fluorescent lifetime of the QD film, with τ=10 ns, the theoretical and measured bandwidth are 15.9 and 15.5 MHz, respectively. The RC time constant should also affect the bandwidth of a QLED [35]. To obtain the R and C values of the QLED, we measured the current–voltage and capacitance–voltage relationships of the QLED with a semiconductor parameter analyzer (Keithley 4200A-SCS, 50 kHz). The variations in the R and C values with the injection current for the 2- and 4-mm2 QLEDs are shown in Fig. 7(a) and (b), respectively. At the same current, the R and C values of the 2-mm2 QLED are smaller than those of the 4-mm2 QLED. The resistivity coefficient ρ can be expressed as [36]
响应时间 τ 与调制带宽 f 之间的关系为 f=1/(2πτ)。如果 QLED 的带宽受 QD 薄膜的荧光寿命限制，τ=10 ns，则理论带宽和测量带宽分别为 15.9 和 15.5 MHz。<font color=red>RC 时间常数也会影响 QLED 的带宽 [35]</font>。为了获得 QLED 的 R 和 C 值，我们使用半导体参数分析仪（Keithley 4200A-SCS，50 kHz）测量了 QLED 的电流-电压和电容-电压关系。图 7(a) 和 (b) 分别显示了 2 和 4 mm2 QLED 的 R 和 C 值随注入电流的变化。在相同电流下，2 mm2 QLED 的 R 和 C 值小于 4 mm2 QLED。电阻率系数 ρ 可表示为 [36]

![image](/picture/evaluation1.png)

with

![image](/picture/evaluation2.png)

where ρ0 is the bulk resistivity, κ is a thickness-dependent parameter, n is the electron concentration, νF is the Fermi velocity, e is the electron charge, m is the effective mass of electron, and lbulk is the bulk mean free path. As the bulk resistivity is inversely proportional to the electron concentration, which is proportional to the current density, the resistance of the device decreases with an increase in the current. The total capacitance of a QLED is given by C=CD+CR , where CD is the diffusion capacitance and CR is the radiative-recombination-based capacitance [37]. An increase in the current causes a decrease in the radiative-recombination-based capacitance, which thus leads to a reduction in the total capacitance. Knowing the R and C values of the QLED, we can estimate the RC-limited bandwidth by f=1 /(2πRC ).

其中，ρ0 是体电阻率，κ 是厚度相关参数，n 是电子浓度，νF 是费米速度，e 是电子电荷，m 是电子的有效质量，lbulk 是体平均自由程。由于体电阻率与电子浓度成反比，而电子浓度与电流密度成正比，所以器件的电阻会随着电流的增加而减小。QLED 的总电容由 C=CD+CR 给出，其中 CD 是扩散电容，CR 是基于辐射复合的电容 [37]。电流的增加会导致基于辐射复合的电容减小，从而导致总电容减小。了解 QLED 的 R 和 C 值后，我们可以通过 f=1/(2πRC ) 估算 RC 限制带宽。

<https://ieeexplore.ieee.org/document/8852748>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/%E6%B3%A8%E5%85%A5%E7%94%B5%E6%B5%81%E5%AF%B9%E9%87%8F%E5%AD%90%E7%82%B9%E5%8F%91%E5%85%89%E4%BA%8C%E6%9E%81%E7%AE%A1%E8%B0%83%E5%88%B6%E5%B8%A6%E5%AE%BD%E7%9A%84%E5%BD%B1%E5%93%8D.pdf>

参考文献：
RC 时间常数也会影响 QLED 的带宽 [35]

**High-Speed Visible Light Communications Using Individual Pixels in a Micro Light-Emitting Diode Array**

**利用微型发光二极管阵列中的单个像素实现高速可见光通信**

报道了基于 III 族氮化物的微像素发光二极管阵列中单个像素的高频调制，其中每个阵列由 16 × 16 个可单独寻址的 72 微米直径像素组成。所研究的器件的峰值发射波长分别为 370、405 和 450 nm。发现 450 nm 发射器件的典型像素的光学 -3 dB 调制带宽约为 245 MHz。使用开关键控非归零调制，从 450 nm 发射的单个像素实现了高达 1 Gb/s 的数据传输速率，比特误码率小于 1 × 10 -10 。此类器件具有用于自由空间或光纤耦合可见光通信的潜力。

<https://ieeexplore.ieee.org/document/5504118>

# 22.Nonpolar m -Plane InGaN/GaN Micro-Scale Light-Emitting Diode With 1.5 GHz Modulation Bandwidth - 非极性面 - 美国新墨西哥州阿尔伯克基新墨西哥大学高科技材料中心

我们展示了一种高速非极性 m 平面 InGaN/GaN 微尺度发光二极管 (LED)，其在电流密度为 1 kA/cm 2时具有创纪录的 1.5 GHz 电 -3 dB 调制带宽。使用速率方程模型提取了 1 kA/cm 2 时 200 ps 的差分载流子寿命 (DLT) 。较短的 DLT 归因于无极化非极性 InGaN/GaN 量子阱中较高的电子-空穴波函数重叠，与极性 c 平面量子阱相比，这导致低电流密度下的自发辐射率更高。在低电流密度下具有改进的高速性能的 LED 将有助于降低功耗并提高 Gb/s 可见光通信系统的效率。

<https://ieeexplore.ieee.org/document/8283504>

# 23. Arista

## 23.1 Andy Bechtolshelm：

这是他在2024年8月底Hotchips听说的使用MicroLED的OSPF，而并不是实际应用中使用了MicroLED

![image](/picture/OSFP-MicroLED.png)

# 24.数据中心交换芯片

数据中心交换芯片的演进趋势是：每两年翻一番的快速增长，25.6T交换芯片采用7nm工艺，51.2T必须选择5nm工艺节点，预计2025年3nm工艺节点将问世，为交换芯片带来102.4T的容量。

![image](/picture/Commercial-Switching-Chip-Capacity-1024x576.webp)

光口方面，25.6T光模块搭配64个400G光模块，2021年已经实现，预计明年将搭配64个800G模块，8x100G方案支持交换机升级到51.2T

对于102.T的交换容量，需要1.6T的光模块，光口需达到200G每波长速率，预计2025年进入产业节点。

![image](/picture/Switch-density-doubles-every-two-years-1024x576.webp)

单通道100G是大节点，可以支持400G、800G光模块的落地，有机会做16x100G 1.6T的方案，但是FiberMall认为8x200G 1.6T才是产业价值。

![image](/picture/Switching-capacity-of-different-serdes-rates-1024x525.webp)

当前，800G即将进入产业化的关键阶段。

1、2020年已完成800G光模块的规范 

2、800G光模块已具备部署条件

这是第一个在系统技术成熟前就能部署的光模块。

3、下一代交换芯片全部支持800G光模块接入

采用8*100G解决方案

![image](/picture/51.webp)

800G光模块主要为2x400G解决方案。

![image](/picture/800G-optical-module-1024x576.webp)

![image](/picture/LC-1-1024x576.webp)

![image](/picture/dual-MPO.webp)

![image](/picture/dual-MPO.webp)

![image](/picture/duplex-LC.webp)

OSFP-XD的MSA在2022年9月有一个草案，MSA的第13页引用了Lightcounting的一张图表，Top5云供应商的以太网光模块市场趋势，其中800G光模块将成为以太网光模块的下一个主导产品。

![image](/picture/sales-of-ethernet-transceivers-to-the-top5-cloud-companies-1024x576.webp)

1.6T光模块

基于200G波长的1.6T光模块
SerDes 接口为 100G 或 200G
降低单位功耗和单位成本的前景

![image](/picture/1.6T-transceiver-1024x576.png)

基于16x100G OSFP-XD1600方案的1.6T光模块预计在2024年带动产业链技术成熟节点，基于8x200G的OSFP1600预计在2026年成熟。

![image](/picture/evolutionary-route-of-OSFP-and-OSFPXD-1024x520.webp)

![image](/picture/rates-of-optical-and-electrical-port-1024x576.webp)

800G、1.6T、以及3.2T采用热插拔模块封装，功耗是需要解决的巨大问题。

![image](/picture/consumption-of-optical-module-1024x575.webp)

下图蓝色部分为以太网模块，橙色部分为相干模块，模块功耗曲线如下。

![image](/picture/Hot-pluggable-module-power-consumption-1024x556.webp)

转换后，基本具有单位位转换函数递减的趋势。

![image](/picture/power-consumption-of-Hot-pluggable-module-1024x576.webp)

根据功耗，以下光模块尺寸可用于不同的解决方案。

![image](/picture/power-consumption-of-Hot-pluggable-optical-module-1024x576.webp)

对于相干的1.6T ZR来说，功耗太大，不能选择QSFP-DD这样的小封装，下图是这几种模块外形尺寸的对比。

![image](/picture/module-form-factor-1024x509.webp)

![image](/picture/optical-module-form-factor-1024x476.webp)

![image](/picture/power-consumption-1024x576.webp)

FiberMall预计2025年将具备单波200G的产业部署能力，基于此，1.6T将具有单位功耗和成本的优势。有可能出现热插拔和CPO竞争，1.6T仍然可以选择热插拔并支持交换机升级到102.T，避免使用产业链不熟悉的CPO封装。

![image](/picture/The-per-channel-rate-will-transition-to-200G-in-2025-1024x575.webp)

**概括**

1. 产业将快速过渡到800G、1.6T光模块端口。
单位成本更低，单位电耗更低。

2. 800G光模块大部分采用2x400G解决方案。
采用2×4×100G解决方案。

3. 1.6T光模块大多采用2x800G方案。
采用2x4x200G解决方案。

4. 1.6T光模块只能使用OSFP/OSFP-XD。
QSFP-DD封装的散热能力不足以满足1.6T ZR的需求。

5. 51.2T/102.4T主流模块封装，无需CPO即可热插拔。

<https://www.fibermall.com/blog/fibermall-1600g-optical-module-roadmap.htm?srsltid=AfmBOopYi2Dm84lSw2dTLUAdCclZd6mtLZ7g3PSqbnyEWrXY4DKmFoHf>

# 25. 初创公司

## 25.1 Lightwave

微腔 MicroLED

要使 MicroLED 发挥应有的作用，就需要坚实的发展平台。当发光体的尺寸变小后，LED 照明行业以前的性能技巧（如表面粗糙化）就不再有效。如今，需要光学微腔。微腔由 LPI 的外延镜模板实现，这些模板具有反射性、导电性，并且与氮化铟镓晶格匹配。

经济实惠的 MicroLED 新时代

MicroCavity MicroLED 可实现光束整形和高效的电光转换。Lightwave Photonics, Inc. 技术实现的低温外延生长进一步实现了与 CMOS 技术的集成。

- 微腔: 微腔是指长度小于一微米的光学腔。在这种光学范围内，由于波共振，发射光的行为与光线追踪模型不同。

- 光束整形:  微腔的优点之一是其固有的光束整形特性。这有助于满足显示器和增强现实的功效需求。

- 电到光子的转换: 微腔的另一个优点是外部量子效率。电能可以更有效地转化为光输出。

- 低温生长: III 族氮化物材料的低温外延生长是发光器件与温度敏感的 CMOS 结构集成的关键。

- 一体化: 展望未来的应用，第二大常用半导体材料系统（III-氮化物）将需要与硅 CMOS 集成。在推出我们的 MicroLED 解决方案时，对集成的需求显而易见。

**导电、晶格匹配和反射**

LPI 使用金属陶瓷和故意掺杂 n 型的 GaN 制作镜子，这两种材料都具有导电性。 镜子材料需要与氮化铟镓晶格匹配，以便在镜子上生长的后续材料具有高质量和低缺陷数量。  并非所有反射材料都相同。金属陶瓷材料的反射特性使镜子可以放置在更靠近 MicroLED 的有源区域的位置。这对于 MicroLED 的整体性能非常重要。

**产品**

蓝宝石、硅、SiC、GaN 上的镜像模板……
镜面模板上的 LED 外延片
低温 III-N 外延膜（掺杂、未掺杂）

<https://lightwavephotonics.com/>

## 25.2 POET

作为一家公司，POET Technologies 一直专注于其技术的颠覆性潜力。我们利用对有源光子器件和光波导的设计和制造知识，并深入了解半导体制造技术，创造了有史以来第一个将电子和光子集成到单个器件中的晶圆级产品 - POET 光学中介层。

由于所有制造、组装、对准、测试、老化和封装均在晶圆级完成，POET 光学中介层实现了集成电子和光子的最低成本， 并具有无与伦比的可扩展性。

 POET 光学中介层是一种 平台技术 ，可提供最大的灵活性和可扩展性。电子和光子器件均在晶圆级制造到光学中介层的各层中，从而消除了主动对准并允许所有器件之间进行高速通信。替换器件或更改外形尺寸只需对平台进行最小的设计更改即可完成，从而使基于光学中介层的解决方案能够跨越多代产品和各种应用。

POET 光学中介层采用与标准 CMOS 半导体工艺完全兼容的晶圆级 工艺制造， 使其成为长期寻求的共同封装光学器件的解决方案——将光子通信能力直接构建到芯片中——用于高速计算和网络应用。

<https://poet-technologies.com/index.html>

**光学中介层**

POET 光学插入器™
电子和光子学的晶圆级集成

POET 光学中介层™ 采用一种新颖的波导技术，可将电子和光子器件集成到单个多芯片模块中。通过应用先进的晶圆级半导体制造技术和新颖的封装方法，POET 的光学中介层消除了传统光子解决方案中采用的昂贵组件、组装、对准和测试方法。除了与传统设备相比降低成本外，POET 的光学中介层还为从数据中心到消费产品的各种光子应用提供了灵活且可扩展的平台。

<https://poet-technologies.com/poet-platform.html>

# 26. RC-LED

## 26.1 可见光共振腔发光二极管原理及发展概况 - 北工大

可见光共振腔发光二极管，是把有源层置于多层F-P光学共振腔中，使自发发射的光在腔中发生干涉，抑制非共振波长，从而达到可选择性出光的目的。

<https://github.com/basteng/Today-I-Learned/blob/main/paper/%E5%8F%AF%E8%A7%81%E5%85%89%E5%85%B1%E6%8C%AF%E8%85%94%E5%8F%91%E5%85%89%E4%BA%8C%E6%9E%81%E7%AE%A1%E5%8E%9F%E7%90%86%E5%8F%8A%E5%8F%91%E5%B1%95%E6%A6%82%E5%86%B5.pdf>















- [1.关于封装内光学 I/O 的三个常见误解](#1关于封装内光学-io-的三个常见误解)
- [2. Lizhenhao Paper](#2-lizhenhao-paper)
  - [2.1 《Bandwidth Analysis of High-Speed InGaN Micro-LEDs by an Equivalent Circuit Model》](#21-bandwidth-analysis-of-high-speed-ingan-micro-leds-by-an-equivalent-circuit-model)
  - [2.2 《High-Speed Micro-LEDs based on Nano-Engineered InGaN Active Region towards Chip-to-Chip Interconnections》](#22-high-speed-micro-leds-based-on-nano-engineered-ingan-active-region-towards-chip-to-chip-interconnections)
- [3. Wanglei Paper](#3-wanglei-paper)
- [4. Ayar Labs](#4-ayar-labs)
  - [4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)](#41-ayar-labs-暗示产品将在未来-2-3-年内出货-hpc-wire)
  - [4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)](#42-ayar-labs-旨在以光速消除人工智能的瓶颈-bloomberg-podcast)
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
- [1.关于封装内光学 I/O 的三个常见误解](#1关于封装内光学-io-的三个常见误解)
- [2. Lizhenhao Paper](#2-lizhenhao-paper)
- [3. Wanglei Paper](#3-wanglei-paper)
- [4. Ayar Labs](#4-ayar-labs)
  - [4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)](#41-ayar-labs-暗示产品将在未来-2-3-年内出货-hpc-wire)
  - [4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)](#42-ayar-labs-旨在以光速消除人工智能的瓶颈-bloomberg-podcast)
- [5. Avicena](#5-avicena)
  - [5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》](#51high-bandwidth-gan-based-micro-leds-at-temperatures-up-to-400c)
  - [5.2 硅光子学联合封装。 凉！ 但它实用吗？Bardia Pezeshki post at Linkedin](#52-硅光子学联合封装-凉-但它实用吗bardia-pezeshki-post-at-linkedin)
- [6. 《廉价光源可使人工智能更节能》Nature](#6-廉价光源可使人工智能更节能nature)
- [7. 多孔硅](#7-多孔硅)
- [8. -3 dB带宽](#8--3-db带宽)
- [9. LED和LD光调制的区别](#9-led和ld光调制的区别)
- [10.模拟光纤通信相关知识](#10模拟光纤通信相关知识)
- [10.1 LED光通信背景知识](#101-led光通信背景知识)
- [10.2 LED调制带宽](#102-led调制带宽)

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

# 10.1 LED光通信背景知识

光通信是要实现超高速的光开关速率，而并不是常见电路中的高速开关，这里强调的是光的开关速率，并非电子或空穴的开关速率；光通信用以补充WIFI等无线通信应用的不足，在某些领域替代WIFI成为一种全新的通信方式。LED光通信技术是近年来逐步发展起来的一种全新的通信技术，很多相关的技术研究还处在起步阶段，尤其在高速LED器件、高速开关电路的技术更是几乎空白。LED串联一个开关进行简单调制，缺点是开关速度严重受限，载流子复合速率不高且剩余载流子泯灭时间过长，使得光通信效果很差。

<https://patents.google.com/patent/CN105050245A/zh>

# 10.2 LED调制带宽

LED的调制带宽决定了通信系统的信道容量和传输速率,其定义是在保证调制度不变的情况下,当 LED输出的交流光功率下降到某一低频参考频率值的一半时(-3dB)的频率就是 LED的调制带宽,如图3-5所示。图中的光带宽指光电探测器输出的信号电流变为原来一半时对应的带宽。

LED的调制带宽受响应速率限制,而响应速率又受半导体内少子寿命τc 影响:

![image](/picture/3db%20f.png)

对于III-V 族(如 GaAs)材料制成的发光二极管而言,τc 的典型值为100ps,故 LED的理论带宽总是限制在2GHz以下。当然,目前所有发光二极管的τc 带宽都远远低于这个值,照明用的大功率白光二极管由于受其微观结构及光谱特性所限,带宽更低。较低的调制带宽限制了 LED在高速通信领域(包括可见光通信系统)的应用,因此,设法提高LED的调制带宽是解决问题的关键。

**综上，LED调制带宽基本取决于载流子寿命**
- 如果载流子寿命100皮秒ps，则3dB理论带宽约为2.7Ghz
- 如果载流子寿命100纳秒ns，则3dB理论带宽约为2.7Mhz

<https://github.com/basteng/Today-I-Learned/blob/main/paper/%E5%8F%AF%E8%A7%81%E5%85%89%E4%BF%A1%E9%81%93%E5%BB%BA%E6%A8%A1.pdf>

摘自 p29~p30

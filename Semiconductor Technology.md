- [1.CMOS 图片 来自领英 Hyeongwon Seo](#1cmos-图片-来自领英-hyeongwon-seo)
- [2.14nm FinFET 晶体管TEM](#214nm-finfet-晶体管tem)
- [3. SK Hynix HBM](#3-sk-hynix-hbm)
- [4. 长鑫存储技术有限公司 通过使用堆叠层而不是 4F2 的 3D DRAM 路线](#4-长鑫存储技术有限公司-通过使用堆叠层而不是-4f2-的-3d-dram-路线)
- [5. 实现高密度半导体结构的考虑因素：现代 DRAM 中的 4F2 和 6F2](#5-实现高密度半导体结构的考虑因素现代-dram-中的-4f2-和-6f2)
- [6. 刻蚀](#6-刻蚀)
- [7. 新型存储](#7-新型存储)
- [8. 半导体技术节点的线宽](#8-半导体技术节点的线宽)
- [9. 内存墙：DRAM 的过去、现在和未来The Memory Wall: Past, Present, and Future of DRAM](#9-内存墙dram-的过去现在和未来the-memory-wall-past-present-and-future-of-dram)
- [10. Microprocessor 和 Microcontoller 有什么区别？](#10-microprocessor-和-microcontoller-有什么区别)
- [11. CFET](#11-cfet)
  - [11.1 台积电、IBM 和三星将于 12 月在一场活动中展示其下一代 CFET 晶体管创新](#111-台积电ibm-和三星将于-12-月在一场活动中展示其下一代-cfet-晶体管创新)
- [12.Memory Hierarchy: Basics](#12memory-hierarchy-basics)
- [13. Potential of EUV for high volume manufacturing of DRAM](#13-potential-of-euv-for-high-volume-manufacturing-of-dram)
- [14. 台积电 高带宽 die-to-die IEDM2024](#14-台积电-高带宽-die-to-die-iedm2024)

<div STYLE="page-break-after: always;"></div>

# 1.CMOS 图片 来自领英 Hyeongwon Seo

20年来，先进半导体芯片的制造方法及其垂直堆叠结构和配置方法基本保持不变。

对于半导体行业的新手和已经成为各自领域专家的人来说，一目了然地看到硅表面下方和上方的堆栈和互连结构的整个形状和实际尺寸，可能是获得新灵感的第一道门。

尽管这些照片是 10 或 20 年前的照片，但它们在探索这条道路和想象未来方面仍然具有价值。

硅表面一直被狭窄和填充，而它上面的结构随着它们的升高而变得更大和更松散，即使想象将堆栈延伸到芯片外部，这一点也保持不变。

硅表面创新的难度，带动着硅之上、芯片外的创新。

*事实上，第一张附图在组件和整体比例方面并不现实。


![image1](/picture//1721363312331.jpg)
![image2](/picture//1721363315102.jpg)
![image3](/picture/1721363315538.jpg)
![image4](/picture//1721363311020.jpg)

<div STYLE="page-break-after: always;"></div>

# 2.14nm FinFET 晶体管TEM

随着最近等离子聚焦离子束 （Helios-5 PFIB/SEM） 的安装，我们想展示我们的 TEM 提升和 STEM/EDX 成像能力。附图显示了带有 14nm FinFET 晶体管的 12 层铜芯片的原位 TEM 提升结果。STEM成像在30kV下进行。薄片被减薄到FinFET结构的栅极。
With the recent installation of our Plasma Focus Ion Beam (Helios-5 PFIB/SEM), we would like to present our TEM lift out and STEM/EDX imaging capabilities. Attached image showed the result of an in-situ TEM liftout of a 12 layer copper die with 14nm FinFET transistors. STEM imaging was done at 30kV. The lamella was thinned to the gate of the FinFET structure.

![image5](/picture/1720812293598.gif)
<div STYLE="page-break-after: always;"></div>

# 3. SK Hynix HBM

Competitive Edge of #HBM ( High Bandwidth Memory )

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Competitive%20Edge%20of%20%23HBM%20(%20High%20Bandwidth%20Memory%20).pdf>
<div STYLE="page-break-after: always;"></div>

# 4. 长鑫存储技术有限公司 通过使用堆叠层而不是 4F2 的 3D DRAM 路线

设计规则预计为 3X nm （比 14nm 节点更松散），层数低于 100 层。

3D 可堆叠 1T1C DRAM：架构、工艺集成和电路仿真

动态随机存取存储器不断缩小⟨随着10纳米以下尺寸的不断缩小，可堆叠DRAM特征尺寸必然会遭遇诸多难以逾越的障碍，如亚10纳米图形化问题、超高纵横比（HAR）电容和窄感测边距等。一种有希望的解决方案是采用三维（3D）水平堆叠晶体管和电容的架构创新，类似于3D NAND的架构。然而，3D可堆叠DRAM架构的工艺集成方案和电路仿真却鲜有报道。本文首次系统地介绍了一种3D DRAM架构和集成方案，并进一步对3D DRAM进行了电路仿真研究，证实了所提架构的可行性，并在DRAM内核时序优化方面展现出巨大的前景。

<https://ieeexplore.ieee.org/abstract/document/10145931>

# 5. 实现高密度半导体结构的考虑因素：现代 DRAM 中的 4F2 和 6F2

2024 年 9 月 11 日 作者Hyeongwon

![image](/picture/4F2_DRAM_STRU624.webp)

在高密度半导体制造中，为了提高电路密度，有时会使用基于最小线宽的概念来表示可以创建重复使用的单元器件的最小单位面积。像 SRAM 这样的器件非常大，但 DRAM 或 NAND 等存储器件则以 8F2、6F2、4F2 或更小的尺寸来表示。最近，经常有报道提到 4F2 DRAM 形式的下一代 DRAM 开发，一些供应商正在研究 2030 年以后推出的产品。

“xx F2” 的概念传统上被理解为二维平面中尺寸的表示。因此，人们普遍认为两个组件不能同时在同一平面的同一位置创建。但是，考虑到现代尝试以堆叠形式配置单元设备，xx F2 的概念可能存在一些令人困惑的方面。器件的通道区域和栅极结构在同一平面上占据 1F2 面积的说法假设两个组件是垂直排列的，并且不同时占据同一平面。但是，当检查许多图表时，似乎这些基本假设早已变得模糊。

![image](/picture/4F2-DRAM-Sample.webp)

如果开发出一种结构，其中两个基本组件占据相同的 F2 区域，这实际上意味着基数更接近 6F2 而不是 4F2。理解这一点对于制定和理解基本产品策略仍然至关重要。通过减小最小线宽将两个组件集成到 F2 区域的概念实际上几乎是荒谬的。

但如果产品实际制作精良，这种表现方式更多是为了展示，实际操作中，有可能推出看似4F2结构，但由于最小线宽大幅缩小，而更接近~6F2级别的产品。

![image](/picture/8f2-6f2-4f2-dram-and-3d-cell-1024x276-1.webp)

<https://semihpc.com/considerations-in-achieving-high-density-semiconductor-structures-the-4f26f2-in-modern-dram/>

# 6. 刻蚀

Dry etch gas chemistry review

 刻蚀化学是刻蚀特定材料的起点，也是工艺优化的关键控制旋钮之一。高电负性元素，卤素，如 F、Cl 和 Br，是用添加剂气体和前驱体蚀刻原料气的常见元素。
 
在本文中，介绍了 Si 刻蚀的各向异性，介绍了 Si、SiO 和 SiN 之间的选择性研究，以了解原料气和反应性添加剂如何影响刻蚀行为。还包含与掺杂、晶体学和离子诱导织构相关的蚀刻依赖性，以通过薄膜特性掌握蚀刻效应。

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/Dry%20etch%20gas%20chemistry%20review.pptx>

# 7. 新型存储

在 VLSI 2023 上，三星显然展示了其 MRAM 路线图，显示其 14nm MRAM 的单元为 0.0242 um2，预计其 8nm MRAM 的单元为 0.016 um2。这对于小于任何 NOR Flash 或 SRAM 信元大小非常重要。该 cell 大小的 current drive 也可能足以用于 ReRAM。

<https://ieeexplore.ieee.org/abstract/document/10185248>

# 8. 半导体技术节点的线宽

在先进的半导体行业，人们常说“我们已经接近技术的极限，以当前的结构和方案进一步缩小晶体管或提高性能已不再可行”。

此时，企业必须在扩展核心结构和技术与快速开发和采用替代技术之间做出选择。在市场上，这两种选择的结果会随着时间的推移而显现出来，并以各种形式呈现，例如收入、盈利能力或客户偏好。

然而，通常很难确定这些结果是否归因于快速采用某些技术或新材料、引进昂贵设备等决策，或者它们是否源于更详细的选择，例如栅极电介质的物理或电气特性和厚度、晶体管的结构或触点与栅极之间的距离，这些选择共同产生多米诺骨牌效应。这些微妙的选择可能会影响看似关键和战略性的决策，但它们往往被忽视。就我个人而言，

我更感兴趣的是硅片上的细微选择及其影响，而不是各个供应商的表面策略。例如，纳米片是一种具有许多优势的结构，我听说台积电从 2nm 节点开始采用该技术。不过，我相信他们也值得考虑以 2.Xnm 解决方案扩展 FinFET 选项。

*所附图片和图表与主要半导体供应商或特定技术分析提供商的观点无关。它们包括一些公开可用的数字以及作者得出的估计值和预测值，可能与特定产品的实际测量值不符。它们仅用于支持作者的观点。

![](/picture/TSMC-TR-SIZE-TREND-XX-20241008-512-1.webp)

<https://semihpc.com/navigating-the-fine-line-choices-in-advanced-semiconductor-tech-and-the-hidden-details/>

# 9. 内存墙：DRAM 的过去、现在和未来The Memory Wall: Past, Present, and Future of DRAM

全世界越来越多地质疑摩尔定律的消亡，但悲剧的是，它早在十多年前就已经消亡，没有引起任何轰动或引起任何关注。人们通常关注的是逻辑，但摩尔定律也一直适用于 DRAM。

![](/picture/4ed35062-121f-412e-aea9-0439fcc5a83f_1132x1318.webp)

![](/picture/c1afb454-26ac-44a2-ba24-754d80012365_1122x1024.webp)
原始缩放定律 - 来源：1965 年《集成电子学的未来》 - 戈登·摩尔

DRAM 不再可扩展。在辉煌时期，内存位密度每 18 个月翻一番 - 甚至超过逻辑。这意味着每十年密度增加 100 多倍。但在过去的十年里，扩展速度已经大大放缓，密度仅增加了 2 倍。

![](/picture/cab4be20-9507-47a5-95b2-13544883eb66_1872x922.webp)
来源：SemiAnalysis

如今，随着人工智能的爆发式发展，行业平衡被进一步打破。虽然随着时间的推移，逻辑芯片的密度和每晶体管功能成本都有了显著改善，但 DRAM 速度的提升却十分缓慢。尽管存在大量 FUD，但台积电 3nm 和 2nm 节点的每晶体管成本仍在下降。而对于内存而言，带宽的增加是由英勇而昂贵的封装推动的。

![](/picture/966cd4b6-272c-45e2-93c0-2a1c6f2872a8_1522x1022.png)
资料来源：Nvidia、SemiAnalysis

高带宽内存 (HBM) 是加速器内存的支柱，其每 GB 成本是标准 DDR5 的 3 倍或更多。客户被迫接受这一点，因为如果他们想制造具有竞争力的加速器套件，几乎没有其他选择。这种平衡是不稳定的——未来的 HBM 世代将继续变得更加复杂，层数也更高。随着模型权重本身接近多 TB 级，AI 内存需求正在激增。对于 H100，制造成本的约 50% 以上归因于 HBM，而对于 Blackwell，这一比例增长到约 60% 以上。

换句话说，DRAM 行业已经陷入困境。计算改进虽然正在放缓，但远远超过了内存。DRAM 的创新步伐如何才能重新加快？未来可以利用哪些创新来改善带宽、容量、成本和功耗？

有很多可能的解决方案。由于人工智能的资本支出高达数千亿美元，因此业界有强大的动力推动这些解决方案的发展。

首先介绍 DRAM 的背景和历史，然后介绍构成现代“内存墙”的每个问题以及可能的解决方案。我们将讨论相对简单的短期想法，例如扩展 HBM 路线图，以及更复杂的长期选择，例如内存计算 (CIM)、铁电 RAM (FeRAM) 或磁性 RAM (MRAM) 等新内存类型，以及即将问世的 4F 2 DRAM 和 3D DRAM。

**DRAM 入门：工作内存**

计算机中使用多种类型的内存。最快的是 SRAM（静态随机存取存储器），它与逻辑处理技术兼容，位于 CPU 或 GPU 上。由于它位于逻辑芯片上，SRAM 也是最昂贵的内存类型 - 每字节比动态随机存取存储器 (DRAM) 贵 100 倍以上 - 因此仅少量使用。相反的类型包括非易失性 NAND 固态驱动器、硬盘驱动器和磁带。这些内存很便宜，但对于许多任务来说太慢了。DRAM 位于 SRAM 和闪存之间的“金发姑娘”区域 - 速度足够快，价格足够便宜。

![](/picture/01f7a2ef-7664-4fc4-87e5-4a43bbcfcff0_1624x632.webp)
记忆层次结构。来源：Enfabrica

DRAM 可占非 AI 服务器系统成本的一半。然而，在过去 10 年中，它是所有主要逻辑和内存中扩展速度最慢的。16Gb DRAM 芯片于 8 年前首次大量上市，但如今仍然是最常见的；它们推出时每 GB 的成本约为 3 美元，最高达到近 5 美元，然后在过去 12 个月内回落到 3 美元左右。速度稍慢一些。功率得到了最大的改善，这主要归功于 LPDDR 的兴起，这是一种使用更短、更高效线路的封装变化，但这里的门槛很低。DRAM 扩展缺乏进展是阻碍计算性能和经济瓶颈。

**DRAM 入门：基本架构**

从原理上讲，DRAM 很简单。它由以网格形式排列的存储单元阵列组成，每个存储单元存储一位信息。所有现代 DRAM 都使用 1T1C 单元，即 1 个晶体管和 1 个电容器。晶体管控制对单元的访问，电容器以小电荷的形式存储信息。

![](/picture/b1154591-77ce-42f4-8752-12020330b35e_521x475.webp)
基本 DRAM 电路：存储单元阵列，每行通过一条字线连接，每列通过一条位线连接。激活 1 条字线和 1 条位线可读取或写入它们相交处的单元

字线 (WL) 连接一行中的所有单元；它们控制每个单元的访问晶体管。位线 (BL) 连接一列中的所有单元；它们连接到访问晶体管的源极。当一条字线通电时，该行中所有单元的访问晶体管都会打开，并允许电流从位线流入单元（写入单元时）或从单元流向 BL（读取单元时）。一次只有 1 条字线和 1 条位线处于活动状态，这意味着只有活动字线和位线相交的 1 个单元会被写入或读取。

<https://www.youtube.com/watch?v=7J7X7aZvMXQ>
当字线打开访问晶体管时，电荷可以从位线流向电容器，反之亦然。资料来源：Branch Education

DRAM 是一种易失性存储器技术：存储电容器会泄漏电荷，因此需要频繁刷新（频率约为每 32 毫秒一次）以维护存储的数据。每次刷新都会读取单元的内容，将位线上的电压提升到理想水平，并让刷新后的值流回电容器。刷新完全在 DRAM 芯片内部进行，没有数据流入或流出芯片。这最大限度地减少了浪费的电量，但刷新仍会占 DRAM 总功耗的 10% 以上。

电容器与晶体管非常相似，已缩小到纳米级宽度，但其纵横比也非常大，大约 1,000nm 高，但直径只有数十纳米——纵横比接近 100:1，电容约为 6-7 fF（飞法拉）。每个电容器存储的电荷非常小，新写入时约有 40,000 个电子。

单元必须通过位线将电子输入和输出，但施加到位线上的电压会被连接到同一位线上的所有其他单元稀释。总位线电容可能总计超过 30fF——稀释度为 5 倍。位线也非常细，这会减慢电子的速度。最后，如果单元最近没有刷新，则可能已大量耗电，因此只能输送一小部分电荷。

所有这些因素都意味着，放电单元以读取其值会产生非常微弱的信号，必须将其放大。为此，感测放大器 (SA) 连接到每个位线的末端，以检测从存储单元读取的极小电荷并将信号放大到有用的强度。然后可以在系统的其他地方将这些较强的信号读取为二进制 1 或 0。

感测放大器具有巧妙的电路设计：它将活动位线与未使用的匹配邻居进行比较，首先将两条线的电压设置为相似。活动位线上的电压将与非活动邻居进行比较，使感测放大器失去平衡，并使其将差值放大回活动位线，既放大信号，又将新的全值（高或低）驱动回仍与位线保持开放的单元。这是一石二鸟的情况：单元同时被读取和刷新。

读取/刷新活动单元后，该值可以从芯片中复制出来，也可以通过写入操作进行覆盖。写入操作会忽略刷新后的值，并使用更强的信号强制位线匹配新值。读取或写入完成后，字线将被禁用，从而关闭访问晶体管，从而捕获存储电容器中的任何驻留电荷。

**DRAM 入门：历史（DRAM 仍在扩展时）**

现代 DRAM 由两项独立而互补的发明实现：1T1C 存储单元和感测放大器。

1T1C 单元由 IBM 的 Robert Dennard 博士于 1967 年发明，他也因同名的 MOS 晶体管缩放定律而闻名。DRAM 和缩放都基于 MOS 晶体管（金属氧化物硅，晶体管栅极中的层）。

![](/picture/272b2edb-c7b6-43dd-af7e-6f729d764d1d_1072x999.webp)
Dennard 的 1T1C 存储单元架构原始专利。来源：美国专利 3,387,286

尽管发明了 1T1C 存储单元结构，但英特尔于 1973 年推出的早期 DRAM 每个单元使用 3 个晶体​​管，中间晶体管的栅极充当存储电容器。这是一个“增益单元”，其中中间和最后一个晶体管提供增益以放大中间栅极上的非常小的电荷，使单元能够轻松读取而不会干扰存储的值。

1T1C 电池在理论上更佳：器件更少、连接更简单、体积更小。为什么没有立即采用呢？因为读取电池还不实用。

在发明时，1T1C 单元的电容很小，无法运行。因此需要第二个关键发明：感测放大器。

第一个现代感测放大器由西门子的卡尔·斯坦于 1971 年开发，并在加州的一次会议上进行了展示，但完全被忽视了。1T1C 架构当时尚未被广泛采用，西门子也不知道该如何利用这项发明。斯坦被调往另一个职位，在那里他拥有与 DRAM 无关的成功职业生涯。

![](/picture/52c42f7e-3f11-4cbf-8c58-2b965654bff7_1033x566.webp)
Stein 的原始感测放大器专利。来源：美国专利 3,774,176

这种设计与位线间距完美匹配，并且能够缩小尺寸以跟上单元尺寸。感测放大器在不使用时完全断电，这样就可以在芯片上安装数百万个感测放大器而不会耗电。这真是一个小奇迹。

感测放大器的时代花了 5 年多的时间才到来。Mostek 的 Robert Proebsting 独立（重新）发现了这一概念，到 1977 年，他们采用 1T1C + SA 架构的 16kb DRAM 成为市场领导者。这一成功模式一直延续——近 50 年后，DRAM 架构基本保持不变。

**DRAM 入门：当 DRAM 停止扩展时**

20世纪，摩尔定律和登纳德缩放定律统治了半导体行业。在巅峰时期，DRAM 密度的增长速度超过了逻辑。每 18 个月，DRAM 芯片的容量就会翻一番，推动了日本晶圆厂的崛起（1981 年，其市场份额首次超过美国，1987 年达到 80% 左右的峰值），以及后来的韩国公司（其市场份额在 1998 年超过日本）。相对简单的工艺使晶圆厂快速更替，为拥有资金建设下一代晶圆厂的新进入者创造了机会。

![](/picture/5db28368-bf61-4508-944b-d5f421a0267c_908x565.webp)
在 DRAM 规模不断缩小的“黄金时代”，每比特价格在 20 年内下降了 3 个数量级。资料来源：Lee, KH，《2000 年后 DRAM 行业战略分析》

这种速度无法长期维持，到 20 世纪末到21世纪，逻辑的发展速度已大大超过内存扩展。最近的逻辑扩展速度已放缓至每 2 年密度提高 30-40%。但与 DRAM 相比，这仍然不错，DRAM 的速度比其峰值慢了大约一个数量级，现在需要 10 年才能将密度提高 2 倍。

![](/picture/06fa2151-f906-4e4e-b69f-31806e707c50_803x452.webp)
“这次不一样”：不，内存周期已经成为行业的一部分 50 年了。资料来源：Lee, KH，《2000 年后 DRAM 行业的战略分析》

这种规模扩张放缓对 DRAM 定价动态产生了连锁反应。虽然内存传统上是一个周期性行业，但密度扩张缓慢意味着在供应有限的情况下，成本降低幅度要小得多，无法缓解价格上涨。增加 DRAM 供应的唯一方法是建造新的晶圆厂。价格大幅波动和高资本支出意味着只有最大的公司才能生存：20 世纪 90 年代中期，有 20 多家制造商生产 DRAM，前 10 名制造商占据了 80% 的市场份额。现在，前 3 家供应商占据了 95% 以上的市场份额。

由于 DRAM 已商品化，供应商本质上更容易受到价格波动的影响（与逻辑或模拟相反），并且必须在市场低迷时主要依靠其产品的原始价格进行竞争。逻辑只有在成本增加的情况下才能维持摩尔定律，而 DRAM 则没有这种奢侈。DRAM 的成本很容易衡量，单位为美元/Gb。相对于早期，过去 10 年的价格下降缓慢——十年内仅下降 1 个数量级，而过去需要一半的时间。DRAM 特有的峰值和谷值行为也很明显。

![](/picture/07104303-6471-4d17-9b57-1d8f7cc89e86_1276x758.webp)
DRAM 密度扩展速度每十年减慢 2 倍，而价格则受周期性影响。资料来源：DRAMExchange、SemiAnalysis

自进入 10 纳米节点以来，DRAM 位密度一直停滞不前。即使在三星的 1z 和 SK 海力士的 1a 节点中添加 EUV，密度也没有显著提高。两个显著的​​挑战是电容器和感测放大器。

电容器的制作难度很大。首先，图案化要求很高，因为孔必须紧密排列，具有非常好的临界尺寸 (CD) 和覆盖控制，以便接触下方的访问晶体管并避免桥接或其他缺陷。电容器的纵横比非常高，蚀刻出又直又窄的孔轮廓非常困难，此外，还需要更厚的硬掩模来实现更深的蚀刻，因为更厚的掩模需要更厚的光刻胶，而光刻胶更难图案化。

接下来，必须在整个孔轮廓的壁上沉积几纳米厚的多个无缺陷层，以形成电容器。几乎每一步都考验着现代加工技术的极限。

![](/picture/6d683331-b14b-44e2-9be5-7fa053d79caa_245x326.webp)
DRAM 存储电容器需要在 100:1 纵横比的孔中形成许多精致的层（不按比例 - 实际电容器可能比图中高 10 倍）。来源：应用材料

感测放大器与逻辑互连类似。它们曾经是事后才想到的，但现在其难度与“主要”功能（逻辑晶体管和存储单元）相当甚至更大。它们受到多方面挤压。必须进行面积缩放以匹配位线缩小，感测放大器变得更不敏感，并且随着尺寸变小而更容易出现变化和泄漏。同时，较小的电容器存储的电荷较少，因此读取它们的感测要求变得更加困难。

还有其他挑战，结果是使用传统方法以经济的方式扩展 DRAM 变得越来越困难。新想法的大门已经打开——让我们来探索其中的一些……

**短期缩放：4F2和垂直通道晶体管**

短期内，DRAM 规模将继续沿着其传统路线图发展。更大、更根本的架构变革将需要数年时间才能开发和实施。与此同时，该行业必须满足对更高性能的需求，即使只是进行微小的改进。

短期路线图有两项创新：4F 2单元布局和垂直通道晶体管 (VCT)。

![](/picture/1adc3c45-a0a5-40a5-ad1b-129ce564c69b_896x455.webp)
三星 DRAM 路线图。资料来源： SemiEngineering最初发布的 Samsung Memcon 2024

请注意，包括三星在内的一些公司在其路线图中将 VCT 置于“3D”旗帜之下。虽然从技术上讲这是正确的，但这有点误导，因为 VCT 与通常所说的“3D DRAM”不同。

![](/picture/9beb7021-7d67-4c41-994a-55c72a87fc22_1024x514.webp)
标准 6F 2布局与采用垂直通道晶体管的 4F 2布局。来源：CXMT IEDM 2023

4F 2以最小特征尺寸 F 来描述存储单元面积，类似于标准逻辑单元高度（例如“6T 单元”）的轨道度量。最小特征尺寸通常是线宽或空间宽度，在 DRAM 中，这将是字线或位线宽度。这是表示单元布局密度的简单方法，并且易于比较 - 4F 2单元的大小仅为 6F 2单元的 2/3 ，理论上密度增加 30%，而无需缩小最小特征尺寸。请注意，纯单元布局并不是密度缩放的唯一限制，因此实际收益可能低于理想的 30% 情况。

4F 2是单个位单元的理论极限。回想一下，特征尺寸是线或空间宽度（即半间距），因此线 + 空间图案的间距为 2F，而不是 F，因此最小可能单元尺寸是 4F 2而不仅仅是 F 2 。因此，一旦实现这种架构，水平扩展的唯一途径就是扩展 F 本身——这很快就会变得不切实际，甚至完全不可能。

自 2007 年以来， DRAM 一直使用 6F2布局，之前使用 8F2 （有趣的是：现代 NAND 已经使用4F2单元，但特征尺寸 F 明显更大。SRAM 的数量级为 120 F2 ，密度降低了 20 倍！）

一个值得注意的例外是 CXMT，这家中国供应商在 2023 年底展示的突破制裁的 18 纳米 DRAM中使用了 VCT 和4F2布局。由于三星、SK 海力士和美光能够缩小单元，因此他们没有像 CXMT 那样被迫采用这些架构。CXMT 早期采用的影响也很重要——他们很可能在缩小 F 方面遇到了困难，因为他们选择了单元和晶体管架构的更彻底的改变。

4F 2单元的关键推动因素是垂直通道晶体管。这是必要的，因为晶体管必须缩小以适合单元，并且两个触点（位线和电容器）也必须适合该占位面积，因此，一条垂直线。在这些规模下，有必要垂直而不是水平构建晶体管，将其占位面积缩小到大约 1F，大致匹配其上方的电容器，同时保持足够的通道长度以使晶体管有效运行。当前的 DRAM 使用水平通道和具有水平分离的源极/漏极。这些是成熟且易于理解的架构。VCT 依次堆叠源极（连接到其下方的 BL）、通道（被栅极和控制栅极的字线包围）和漏极（连接到上方的电容器）。在制造过程中存在权衡，有些步骤变得更容易，而其他步骤则更难，但总体而言，VCT 更难制造。

三星的工艺因使用晶圆键合而引人注目。在类似于逻辑背面供电的工艺中，单元访问晶体管是在翻转晶圆并将其键合到支撑晶圆之前在顶部形成位线的情况下制造的，因此位线现在被埋了起来。有趣的是，键合后的基座似乎不需要与 VCT 精确对准，尽管披露并未解释外围 CMOS 是位于翻转的芯片上还是位于新键合的基座中。顶部变薄以露出晶体管的另一端，因此可以在其顶部构建存储电容器。EVG 和 TEL 将从这种对晶圆键合工具的新需求中获益。

**DRAM 入门：当前变体**

DRAM 有很多种，每种都针对不同的目标进行了优化。相关的最新一代类型是 DDR5、LPDDR5X、GDDR6X 和 HBM3/E。它们之间的差异几乎完全在于外围电路。不同类型内存单元本身相似，所有类型的制造方法也大致相似。让我们简单介绍一下各种 DRAM 类型及其作用。

DDR5（第五代双倍数据速率）采用双列直插式内存模块 (DIMM) 封装，可提供最高内存容量。LPDDR5X（低功耗 DDR5，X 表示增强型）可提供低功耗操作，但需要与 CPU 的较短距离和低电容连接，从而限制了容量，因此它用于需要低功耗且布局限制可容忍的手机和笔记本电脑。

最近，我们看到一些 AI 加速器、Apple 的专业工作站和 Grace 等 AI 馈送 CPU 采用了容量更大的 LPDDR 封装。这些新用途的推动因素是对高能效数据传输和高带宽的追求。

在加速器中，LPDDR 已成为“第二层”内存的最佳选择，与昂贵的 HBM 相比，它以较低（较慢）的级别提供更便宜的容量。它在构建最高容量和可靠性功能方面有所欠缺，但胜过 DDR5 DIMM，因为它每比特吞吐量消耗的能量要少一个数量级。LPDDR5X 封装在 Nvidia Grace 处理器上最高可达 480GB，这大约是 GDDR 配置容量限制的 10 倍（受电路板布局规则和满足消费者游戏系统信号要求的芯片封装限制），与中型 DDR 服务器配置处于同一范围。使用 128GB 以上的 R-DIMM 可以实现更大容量的 DDR5，但由于封装复杂性和 DIMM 上的额外寄存器（一种缓冲芯片），成本较高。

LPDDR5X 在功耗方面比 DDR 有巨大优势，在成本方面比 HBM 有巨大优势，但每比特能量无法与 HBM 抗衡，而且它需要很多通道（与 CPU 的连接），这会使大容量的电路板布局拥挤不堪。它在纠错 (ECC) 方面也表现不佳，这在大容量下变得更加重要，因为出现错误的可能性更大。为了弥补这一点，必须转移一些容量来支持额外的 ECC。例如，Grace CPU 每个计算托盘有 512GB 的 LPDDR5x，但似乎为可靠性功能保留了 32GB，剩下 480GB 可供使用。

即将推出的 LPDDR6 标准几乎没有任何改进，每个芯片的通道数仍然很高，速度提升幅度相对较小，纠错支持也有限。LPDDR6 不会成为 HBM 的竞争对手。

GDDR6X（G 代表图形）专注于图形应用，以低成本提供高带宽，但延迟和功耗更高。虽然在游戏 GPU 中很有用，但它的设计具有板级容量限制和功率水平，限制了可以使用它的 AI 应用程序的大小。

然后是 HBM3E（第三代高带宽内存，带有增强型“E”版本）。它优先考虑带宽和电源效率，但价格非常昂贵。HBM 的两个定义特征是更宽的总线宽度和垂直堆叠的内存芯片。单个 HBM 芯片每个 I/O 有 256 位，是 LPDDR 的 16 倍，LPDDR 的总线宽度每个芯片只有 16 位。芯片垂直堆叠，通常为 8 个或更多，每 4 个芯片分组一个 I/O；总的来说，该封装可以提供 1024 位带宽。在 HBM4 中，这个数字将翻倍到 2048 位。为了充分利用 HBM，最好将其与计算引擎一起封装，以减少延迟和每位的能量。为了在保持计算短连接的同时扩大容量，必须将更多芯片添加到堆栈中。

HBM 的高成本主要源于这种芯片堆叠需求。在典型的 HBM 堆栈中，8 或 12 个 DRAM 芯片（路线图上计划增加到 16 个或更多）堆叠在一起，电源和信号通过每个芯片中的硅通孔 (TSV) 布线。TSV 是直接穿过芯片的导线，用于连接芯片。与用于连接堆叠芯片的旧式引线接合方法相比，TSV 密度更高、性能更高、成本更高。在 HBM 堆栈中，必须通过 TSV 布线 1,200 多条信号线。必须为它们分配相当大的区域，使得每个 HBM DRAM 芯片的尺寸是相同容量下标准 DDR 芯片的两倍。这也意味着对 DRAM 芯片的电气和热性能有更高的分级要求。

这种复杂性会降低产量。例如，三星的 DRAM 设计失误及其使用落后的 1α 节点导致其 HBM 产量极低。封装是另一个主要挑战。由于产量相对较低，正确对齐 8+ 个芯片（每个芯片有数千个连接）非常困难，因此成本高昂。目前，这是 HBM 供应商之间的主要区别之一，因为SK Hynix 可以使用其 MR-MUF 封装成功生产 HBM3E，而三星则难以提高其产品的产量。美光有一个可行的解决方案，但需要大幅扩大生产规模。

尽管成本高昂且产量有限，HBM3E 目前仍是内存行业有史以来最有价值、利润率最高的产品。这主要是因为对于大型 AI 加速器而言，没有其他类型的 DRAM 是可行的替代品。尽管随着三星提高产量以及美光扩大生产，利润率可能会下降，但 AI 加速器对内存的需求将继续增长——在一定程度上抵消了这一新供应带来的好处。

![](/picture/d663f025-7f33-40ca-835e-ffe0f023e3ba_1240x379.webp)
HBM 在带宽和封装密度方面占据主导地位。来源：SemiAnalysis

简而言之，高带宽和非常高的带宽密度以及最佳的每比特能量和真正的 ECC 功能使 HBM3E成为目前AI 加速器的明显赢家。这就是 Nvidia 的 H100 和 AMD 的 MI300X 等产品使用它的原因。GDDR6/X 虽然容量很小，但按相同指标排在第二位。LPDDR5 和 DDR5 甚至更差，都不适合加速器的需求。

当前的 HBM 解决方案价格昂贵，而且扩展难度越来越大。我们为什么会陷入这种境地？

**HBM 路线图**

HBM 是一种围绕传统 DRAM 理念构建的封装解决方案，但采用密度和相邻性封装，以尝试解决 AI 和其他形式的高性能计算的带宽和功率问题。

目前，所有领先的 AI GPU 都使用 HBM 作为内存。2025 年的计划是 12-Hi HBM3e，配备 32 Gb 芯片，每堆栈总共 48 GB，数据速率为每线 8 Gbps。在 GPU 服务器中，首批支持 CPU 的统一内存版本已随 AMD 的 MI300A 和 Nvidia 的 Grace Hopper 一起推出。

Grace CPU 具有高容量 LPDDR5X，而 GPU 具有高带宽 HBM3。但是，CPU 和 GPU 位于不同的封装中，通过 NVLink-C2C 以 900 GB/s 的速度连接。这种模型集成起来更简单，但在软件方面更困难。连接到另一个芯片的内存的延迟要高得多，可能会影响大量工作负载。因此，内存并不完全统一，并带来了自身的挑战。

![](/picture/c890a2a0-d36e-4ddb-b389-ab9741090a91_2134x1200.webp)
![](/picture/240e148e-5f00-419d-9777-debe9e74725e_1536x856.webp)
资料来源：三星、美光

HBM4 还需要几年时间才能问世，三星和美光声称它将达到 16-Hi，每堆栈 1.5 TB/s。这比我们目前的带宽高出一倍多，而功耗仅为 1.3-1.5 倍，但这种扩展还不够，因为内存的功耗总体上还在继续增加。HBM4 还将改为每堆栈 2048 位宽度，将数据速率略微降低至 7.5 Gbps，有助于降低功耗和实现信号完整性。数据速率很可能会提高到 HBM3E 的水平，或者类似水平。

另一个重大变化是 HBM 基片。基片将采用 FinFET 工艺制造，而不是现在使用的平面 CMOS 技术。对于不具备这种逻辑能力的美光和 SK 海力士，基片将由代工厂制造，台积电已经宣布他们将成为 SK 海力士的合作伙伴。此外，还将为个别客户定制基片。

我们将发布有关 HBM 定制的单独报告，但这里有一个快速入门指南：

HBM4 公告预测至少将使用 2 种不同形式的基础芯片，从而允许针对不同的速度和长度优化内存接口。控制 DRAM 状态机的功能可能会转移到基础芯片上，以更有效地控制 DRAM 芯片，而仅垂直连接可能会降低每位的能量。

定制 HBM 可以实现我们今天看到的传统基于 CoWoS 的组件之外的多种其他封装架构。可以使用中继器 PHY 来菊花链连接多行 HBM - 尽管超过 2 级的任何情况都会看到收益递减。

![](/picture/0d848872-00c9-48e3-9ced-548e9c626921_1352x658.webp)
来源：SK海力士

随着 HBM4 和后续产品的推出，混合键合技术已被提出。这将允许更薄的 HBM 堆栈，因为凸块间隙被消除，并且散热效果更好。此外，它将允许 16-20+ 层的堆栈高度。它还可以减少少量功耗，因为信号传输的物理距离将减少。然而，挑战是巨大的——生产 16+ 个芯片的键合堆栈并不容易，没有一个是完全平坦的——目前还没有人接近大批量制造的解决方案。

所有初始 HBM4 都不会使用混合键合，并且我们预计这种情况将比大多数人希望的持续更长时间。

CPU、GPU 或加速器与内存之间的连接位于基础芯片中。改进这种连接是克服内存限制的一种可能途径。Eliyan 是一家由美光和英特尔等公司资助的初创公司，该公司正利用其 UMI 自定义界面率先采用这种方法。

![](/picture/d43509ad-0713-4ac0-b745-4b4c95966433_2739x2096.webp)
![](/picture/a507cb31-7f32-4b6d-aed2-bf8d586a3463_3284x2541.webp)
![](/picture/32e42c96-325f-43b4-91dd-040f3b287438_3426x2651.webp)
![](/picture/24b0de3a-b907-479b-b5c8-72ab2d5b73b1_533x416.webp)
来源：Eliyan

此 UMI 接口与 ASIC 芯片一起使用，后者可用作 HBM 堆栈的基础芯片或其他内存类型的模块控制器。此芯片组包含内存控制器和内存芯片的物理互连 (PHY)。UMI 外部连接到主机 GPU，连接到主机的结构。它们采用全 CMOS 工艺制造，速度快且高效，使用先进的“Nulink”协议连接到主机，并消除主机硅片上的内存控制器占用空间。

Eliyan 的封装技术甚至可以使用标准基板，并且比常规先进封装具有更大的覆盖范围。这可能允许 HBM 不与 ASIC 芯片相邻，而是更远，这意味着可以容纳更高的容量。他们的方法还占用了主机上的更少面积和海岸线，这意味着可以增加通道宽度。标准化的 UMI 内存芯片可以允许使用 HBM、DDR、CXL 内存等，而无需固定为特定类型，从而显着提高灵活性。虽然这种方法可能会带来短期改进，但它并不能解决 HBM 的根本成本问题。

**新兴记忆**

自从 DRAM 和 NAND 占据主导地位以来，人们一直在研究更好的替代方案。这些方案的总称是“新兴存储器”。这个称呼有点用词不当，因为到目前为止，它们都没有成功“崛起”成为大批量产品。不过，考虑到围绕人工智能的新挑战和激励措施，它们值得至少进行简短的讨论。

最有前景的离散应用存储器是 FeRAM。它们不使用存储电容器中的电介质（绝缘材料），而是使用铁电体（在电场中极化的材料）。它们具有非易失性的理想特性，即它们可以在关闭时存储数据，并且不会在刷新上浪费电力或时间。

美光在 IEDM 2023 上展示了令人鼓舞的结果，其密度可与 D1β DRAM 相媲美，同时具有良好的耐用性和保留性能。换句话说，**如果不是因为成本问题，它是 AI/ML 用途的良好候选者。与传统 DRAM 相比，它的制造过程复杂，并且使用了更多特殊材料，以至于它目前根本没有竞争力**。

MRAM 是另一个有前景的研究领域。数据不是通过电荷存储，而是通过磁性方式存储。大多数设计使用磁隧道结 (MTJ) 作为位存储单元。

![](/picture/db640a71-bda0-4de0-89a9-20c46efa7791_892x673.webp)
磁隧道结 RAM，采用磁性机制而非电气机制。资料来源：SK Hynix

在 IEDM 2022 上，SK Hynix 和 Kioxia 展示了间距为 45nm、临界尺寸为 20nm 的 1 选择器 MTJ 单元。它们共同实现了迄今为止最高的 MRAM 密度 0.49 Gb/mm 2 ，高于 Micron 的 D1β DRAM （密度为 0.435 Gb/mm 2 ）。该单元甚至采用 4F 2设计。他们的目标是以分立封装的形式生产，作为 DRAM 的替代品。

目前，没有任何替代存储器能够挑战 DRAM。有些存储器单元更大或更慢。有些存储器的工艺更昂贵。大多数存储器的耐用性有限。有些存储器的产量较低。实际上，磁性存储器或相变存储器的出货产品以 MB 而不是 GB 为单位。这种情况可能会改变，这关系到很多钱，而且可能存在一种隐秘的制胜组合，但在这两种设备和生产规模方面都还有很多工作要做。

**内存计算**

DRAM 从一开始就受到其架构的限制。它是一个简单的状态机，没有任何控制逻辑，这有助于降低成本，但这意味着它依赖于主机 (CPU) 来控制它。

这种模式根深蒂固：现代 DRAM 制造工艺经过了高度优化和专业化，因此无法实际生产控制逻辑。行业组织 JEDEC（联合电子设备工程委员会）在制定新标准时也要求尽量减少逻辑干扰。

![](/picture/d2a37746-c1ed-4919-9b53-848a50148fea_842x850.webp)
“哑” DRAM：控制逻辑与内存分开，因此命令必须通过缓慢、低效的接口。来源：SemiAnalysis

DRAM 芯片完全依赖于主机：所有命令都通过一个共享接口传输到内存中的多个存储体，代表主机中的多个线程。每个命令都需要 4 个或更多步骤以精确的时间发出，以保持 DRAM 正常运行。DRAM 芯片甚至没有避免冲突的逻辑。

使用古老的半双工接口会加剧这种情况：DRAM 芯片可以读取或写入数据，但不能同时读取或写入数据。主机具有 DRAM 的精确模型，并且必须预测接口是否应在每个时钟周期设置为读取或写入。命令和数据通过不同的线路发送，这降低了时序复杂性，但增加了线路数量和 GPU 或 CPU 上的“滩头”拥挤。总体而言，内存接口的比特率、滩头密度和效率比逻辑芯片使用的替代 PHY 低了一个数量级。

这些缺点的结果是，服务器上最常见的 DDR5 DIMM 在主机控制器和接口上消耗了超过99%的读取或写入能量。其他变体略好一些 - HBM 能量使用大约 95% 用于接口，5% 用于内存单元读取/写入 - 但仍然远未达到 DRAM 的全部潜力。

功能完全放错了地方。当然，解决方案是将其移到正确的位置：控制逻辑应该与内存一起放在芯片上。这就是内存计算 (CIM)。

**内存计算：释放银行潜力**

DRAM 库具有令人难以置信的性能潜力，但由于接口的原因，这些潜力几乎被完全浪费了。

组是 DRAM 构造的基本单位。它们由 8 个子组组成，每个子组有 64Mb（8k 行 x 8k 位）的内存。组一次激活并刷新 1 行 8k 位，但在任何 I/O 操作中仅输入或输出 256 个。此限制是由于感测放大器的外部连接：虽然行由 8k 个感测放大器支持，但只有 1/32 个感测放大器（256）连接到子组外，这意味着读取或写入操作限制为 256 位

![](/picture/201752d9-91cf-4952-aa84-d69f080becb9_2736x1903.webp)
(a) 高电容器的密集垫限制了对感测放大器的访问。来源：SemiAnalysis。(b) 聚焦离子束 [FIB] 拆解 DDR4 DRAM 的感测放大器区域。来源：Marazzi 等人。《HiFi-DRAM：通过使用 IC 成像揭示感测放大器实现高保真 DRAM 研究》，ISCA 2024 (c) 1β DRAM 中垫区边缘的图形。来源：美光

感测放大器位于一个峡谷中，四周环绕着高大的电容器。在上面苏黎世联邦理工学院的 FIB 拆解图中，您可以看到较高处的布线需要延伸至下方的高通孔才能与感测放大器接触。

即使接口有限，每次只能访问 32 个中的 1 个，一个存储体的峰值读写容量也大约为 256Gb/s，平均接近 128 Gb/s，因为至少 50% 的时间用于切换到新的活动行。每 16Gb 芯片有 32 个存储体，一个芯片的全部潜力为 4TB/s。

在层次结构的更上层，存储体以存储体组的形式连接，存储体组又连接到 DRAM 芯片的接口。在 HBM 中，每个芯片有 256 条数据线，峰值吞吐量为每芯片 256 GB/s。这个瓶颈只能利用存储体潜在潜力的1/16 。

![](/picture/c0c73dc0-1ec4-4171-a670-0494a26bc88e_748x694.webp)
来源：SemiAnalysis

更糟糕的是，将一个比特从芯片中传输出去需要 2pJ 的能量，比将其移入或移出单元所需的能量多 20 倍。大部分能量发生在 DQ（数据问号，用于读取和写入的数据线）线两端的两个接口处，以及主机上的控制器逻辑中。

在这种浪费的架构下，不可避免地需要付出努力来获取更多的潜在性能。

**内存计算：DRAM 的全部潜力**

即使是简单的理论示例也表明，这里存在巨大的潜力。实施 UCIe（通用小芯片互连）标准将允许每毫米边缘实现 11 Tbps 的吞吐量——几乎比 HBM3E 高 12 倍。每比特能量将从 2pJ 下降到 0.25pJ，降幅达一个数量级。UCIe 甚至不是最新的解决方案……仅举一个例子，Eliyan 专有的 Nulink 标准就声称有更大的改进。

![](/picture/45f156b0-308a-4698-9e3d-9f7d3f3a2d85_784x364.webp)
来源：Tom’s Hardware

需要注意的是，如果主机结构通过接口扩展，则必须在 DRAM 端处理结构命令集的子集。每个组都需要在本地实现状态机（预充电、地址选择、激活、读/写、关闭等）。这需要在 DRAM 上制造（相对）复杂的片上逻辑。

**内存计算：前进之路和可能的赢家**

当然，在 DRAM 芯片中添加逻辑并非易事。好消息是 HBM 包含一个 CMOS 基础芯片，当 3D DRAM 出现时，几乎可以肯定的是，良好的 CMOS 逻辑会绑定在内存堆栈的顶部或下方。换句话说，该架构适合在内存中包含一些计算，芯片制造商将有动力这样做。

这里有一些唾手可得的成果：想想如果 HBM 采用 GDDR7 速率（每条数据线 32Gbps），可以做些什么。GDDR7 表明，DRAM 芯片上可以制造速度足够快的晶体管，而 TSV 到基座堆栈的垂直距离不到 1 毫米，这应该可以将每位能量保持在 0.25pJ/位范围内。这引出了一个问题：为什么 JEDEC 不在这里采用改进的标准？

基础芯片上的外部接口可以大幅升级为现代设计，每毫米边缘提供超过 1TB/秒的传输速度，每比特仅消耗几 pJ 的能量。有人将在这场知识产权战争中大获全胜。虽然 JEDEC 可能会采用一种选择作为标准，但更有可能的是，速度更快的内存/GPU 供应商组合将完成这一选择，因为 JEDEC 通常需要数年时间。

![](/picture/80a44926-f968-480e-b8f8-ebced851c14d_664x762.webp)
来源：SemiAnalysis

随着第三方基础芯片的接受，我们已经看到 HBM4 可能出现真正的变化，这必将引发实验。我们可能会看到卸载通道控制、互连上的纯结构扩展、在几厘米的距离内每比特能耗降低，以及菊花链连接到远离主机的其他 HBM 行，或连接到第二层内存（如 LPDDR 组）。

通过这种方式，设计可以避开在内存堆栈内部进行计算的功率限制，而是使用基础芯片上的现代化接口，让相邻芯片具有带宽和低每位能耗，就像在内存中进行计算一样。

<https://www.semianalysis.com/p/the-memory-wall?utm_campaign=post&utm_medium=web>

# 10. Microprocessor 和 Microcontoller 有什么区别？

微处理器和微控制器都是集成电路 （IC） 的类型，都是电子设备的“大脑”，但它们具有不同的功能和应用。

🚀 假设您正在建造一座房屋：

1） 微处理器：这就像建筑师的蓝图，勾勒出房子的整个设计和结构。它包含每个房间、功能和系统的详细计划。

2） 微控制器：这就像一个特定的电气元件，例如恒温器或烟雾探测器。它具有专门的功能，旨在与其他组件配合使用以创建一个完整的系统。

🚀 主要区别：

1） 范围：微处理器处理房屋的整体设计和协调。微控制器专注于房屋内的特定任务，例如控制温度或检测烟雾。

2） 复杂性：微处理器更复杂，因为它们需要管理整个房子的系统。微控制器更简单，专注于其特定任务。

3） 集成：微处理器与各种微控制器和其他组件一起工作，创建一个功能性房屋。微控制器集成到房屋的系统中以执行其特定任务。

🚀 微处理器：

1） 通用计算机：微处理器本质上是单芯片上的通用计算机。它可以执行广泛的指令，可用于各种应用。

2） 复杂任务：微处理器旨在处理复杂任务，例如运行操作系统、执行软件应用程序和执行密集计算。

3） 无内置外设：微处理器通常没有内置外设，如定时器、模数转换器 （ADC） 或数模转换器 （DAC）。这些外围设备需要从外部连接。

🚀 微控制器：

1） 专用计算机：微控制器是专为嵌入式系统设计的专用计算机芯片。它针对特定任务进行了优化，并具有内置外围设备。

2） 嵌入式系统：微控制器通常用于洗衣机、冰箱、汽车和工业自动化系统等设备。

3） 内置外设：微控制器具有内置外设，允许它们与物理世界进行交互，例如传感器、执行器和通信接口。

🚀 总结：
微处理器：用于复杂任务的通用计算机。
微控制器：用于嵌入式系统的专用计算机，内置外设。

![](/picture/1728185266812.jpg)

# 11. CFET

## 11.1 台积电、IBM 和三星将于 12 月在一场活动中展示其下一代 CFET 晶体管创新

据eeNewsEurope报道， IBM、IMEC、三星和台积电的研究人员将在 2024 年 12 月即将举行的国际电子设备会议 (IEDM) 上展示他们在垂直堆叠互补场效应晶体管 (CFET) 方面的最新研究成果。CFET 通常被视为环绕栅极晶体管的后继者，将实现未来的技术扩展，但业界尚未采用 GAA FET 进行大规模生产。

CFET 的概念是将 n 型晶体管和 p 型晶体管堆叠在一起，最早由 IMEC 研究机构于 2018 年提出。即使在今天，CFET 的实际实现仍广泛处于研究领域。根据 IMEC 自己的路线图，如果一切顺利，CFET 可能会在 A5 节点实现大规模生产，预计在 2032 年左右。尽管如此，英特尔和台积电等公司近年来开始展示 他们在 CFET 领域的进步，因此看看 IEDM 会带来什么是很有意义的。

![](/picture/CFET.png)

台积电将讨论其在 48nm 栅极间距（相当于 5nm 工艺）上开发单片 CFET 反相器。该反相器采用堆叠的 n 型和 p 型纳米片晶体管，背面有触点，可实现高达 1.2V 的电压传输，两种晶体管类型的亚阈值斜率在 74 至 76mV/V 之间。尽管这标志着一个重要的里程碑，但台积电承认该技术目前尚未准备好进行商业生产。

台积电设计的关键创新包括垂直漏极侧局部互连、背面金属化漏极（BMD）和背面栅极通孔（BVG），它们共同改善信号布线并优化功率、性能和面积（PPA）。

从技术上讲，这种架构为未来几年性能和功率效率的持续提升以及晶体管密度的提高提供了途径。不过，台积电的 CFET 进步仍处于实验室阶段，需要数年时间才能进入该公司的晶圆厂。

IBM Research 和三星将展示一款“单片堆叠 FET”，其特点是采用阶梯式通道设计，下部通道比上部通道宽，从而降低了堆叠高度并缓解了高纵横比带来的挑战。这项研究还涵盖了通道和源/漏极区域的隔离技术，以及双功函数金属的使用。有关金属或栅极间距的详细信息将在会议上公布。

IMEC 将展示其在“双排 CFET”方面的工作，旨在进一步在垂直和水平方向上扩展 CFET。IMEC 认为，这种晶体管设计可以在 7a 级（7 埃）制造工艺中实现，而这距离我们还有六到七代的时间。有趣的是，“双排 CFET”不具有直接背面电源接触，并且采用 60nm 栅极间距进行探索，类似于 7nm 节点。

虽然会议上发表的论文表明 CFET 技术已经取得了重大进展，但这种晶体管距离大规模生产还有数年时间，因为仍必须克服与制造复杂性相关的挑战。

IEDM 会议将于 2024 年 12 月 7 日至 11 日在旧金山举行，会议结束后可在线访问录制的演讲。

<https://www.tomshardware.com/tech-industry/tsmc-ibm-and-samsung-to-present-their-next-gen-cfet-transistor-innovations-at-an-event-in-december>

# 12.Memory Hierarchy: Basics

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/Memory%20Hierarchy%20Basics.pdf>

# 13. Potential of EUV for high volume manufacturing of DRAM

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/Potential%20of%20EUV%20for%20high%20volume%20manufacturing%20of%20DRAM.pdf>

# 14. 台积电 高带宽 die-to-die IEDM2024

![](/picture/D2D-Interconnect.jpg)

最近，台积公司 年在 IEEE Open Journal of the Solid-State Circuits Society https://lnkd.in/gupeBDjB 上发表了一篇关于实现高带宽 die-to-die （D2D ） chiplet interconnects 的关键设计注意事项的综述。

摘录：
📝运行速率为 56-112Gbps 的串行器/解串器 （SerDes ） 通常用于 2D/2.1D/2.2D/2.3D 封装中，以最大限度地提高每引脚数据速率。相比之下，基于 2.5D 中介层的封装通常配备高速并行数据链路，因为它们具有卓越的能源和面积效率。同时，先进的 3D 堆叠技术最受益于更简单、低速的并行链路，这些链路具有最少的缓冲器和触发器，并且没有专用的均衡器/校准电路，从而实现了比 2.5D 更高的数据面积/带宽密度和能效。
📝对于大多数倒装芯片封装 （2D/2.1D/2.2D/2.3D），焊料凸点和金属走线的间距相对较粗。因此，人们通常被迫通过具有差分信号的串行链路（例如 PCIe-32/64Gbps、CEI-112/224Gbps）来最大化每个引脚的数据带宽密度。
📝先进的 2.5D 封装技术允许在每个单元几何结构的更多并行单端信号链路上应用每个引脚的较低数据速率，以最大限度地提高带宽密度（例如，4-32Gbps 的 UCIe x64），同时简化系统设计并提高能效。
📝3D 堆叠的密度继续上升（间距 P≤9μm）。根据涵盖 UCIe-3D™ 的最新 UCIe 2.0 标准，每个 3D 互连的有效面积应小于凸块的面积，以最大限度地提高互连效率（≜带宽密度 x 能效），并且每个并行数据链路应保持 5Gbps 的“慢速”，以减轻时序工作负载。无需采用专用校准或线性均衡，从而进一步降低了系统复杂性和开销。
📝先进封装中常见的去耦帽 （decap） 类型包括——从上到下;如下所示—A） 片上去耦电容，通常是电容密度为 ~50nF/mm² 的超高密度金属内金属电容器 （SHDMIM） 或 ~10nF/mm² 的硅电容器，B） 上中介层去耦电容，例如 >1000nF/mm² 的嵌入式深沟槽电容器 （eDTC），以及 C） 封装上/衬底分立式去耦电容，通常在 μF 范围内。

🔍观察：
“设计与技术协同优化”（DTCO ）已成为与先进封装和测试相关的多方面工程考虑的统称。（让我们都称自己为 DTCO 专业人士，或者简称为“DTCO 专业人士”。

延伸阅读：
🏷️全文： https://lnkd.in/gdq7wqP4
🏷️排序   Chiplets ：https://lnkd.in/gjej2Yqk
🏷️小芯片 （V）：https://lnkd.in/dUAk5PkP
🏷️小芯片 （VI）：https://lnkd.in/gKKse9_x
🏷️小芯片 （VII）：https://lnkd.in/gyr6ZrV6
🏷️小芯片 （VIII）：https://lnkd.in/gzJeAQFV
🏷️2024  IMAPS UCIe：https://lnkd.in/gYDjZVwz
🏷️小芯片封装类型：https://lnkd.in/g4HT59N4

<https://www.linkedin.com/posts/mingliangliu_d2d-chiplet-interconnects-activity-7271910436294262786-eYqM?utm_source=share&utm_medium=member_desktop>

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/High-Bandwidth_Chiplet_Interconnects_for_Advanced_Packaging_Technologies_in_AI_ML_Applications_Challenges_and_Solutions.pdf>
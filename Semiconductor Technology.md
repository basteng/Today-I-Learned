- [1.CMOS 图片 来自领英 Hyeongwon Seo](#1cmos-图片-来自领英-hyeongwon-seo)
- [2.14nm FinFET 晶体管TEM](#214nm-finfet-晶体管tem)
- [3. SK Hynix HBM](#3-sk-hynix-hbm)
- [4. 长鑫存储技术有限公司 通过使用堆叠层而不是 4F2 的 3D DRAM 路线](#4-长鑫存储技术有限公司-通过使用堆叠层而不是-4f2-的-3d-dram-路线)
- [5. 实现高密度半导体结构的考虑因素：现代 DRAM 中的 4F2 和 6F2](#5-实现高密度半导体结构的考虑因素现代-dram-中的-4f2-和-6f2)
- [6. 刻蚀](#6-刻蚀)
- [7. 新型存储](#7-新型存储)

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
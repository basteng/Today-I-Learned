- [1. 三菱电机公司新闻稿宣布推出全球首款能够支持 4G、5G 及超 5G/6G 宽带操作的 GaN 功率放大器。](#1-三菱电机公司新闻稿宣布推出全球首款能够支持-4g5g-及超-5g6g-宽带操作的-gan-功率放大器)
- [2.MERL 负责GaN的研究人员 IEDM2022 总结](#2merl-负责gan的研究人员-iedm2022-总结)

<div STYLE="page-break-after: always;"></div>

# 1. 三菱电机公司新闻稿宣布推出全球首款能够支持 4G、5G 及超 5G/6G 宽带操作的 GaN 功率放大器。

三菱电机公司今天宣布，它已经开发出据称是世界上第一款氮化镓 (GaN) 功率放大器，该放大器使用单个功率放大器实现 3,400MHz 的频率范围，该公司已证明该放大器可用于在单个基站中以不同频率运行的 4G、5G 和 Beyond 5G/6G 通信系统。该放大器有望使无线电单元 (收发器) 与不同的通信系统共享，从而实现更节能的基站。

![PA](/picture/PA1.jpg)

三菱电机研究人员 Toshiaki Koike-Akino 和 Koon Hoo Teo 帮助开发了该技术和设备。技术细节将于本月在 IEEE 国际微波研讨会 2023 上公布。

请参阅以下链接以获取三菱电机的完整新闻稿。

<https://www.mitsubishielectric.com/news/2023/0608.html>

# 2.MERL 负责GaN的研究人员 IEDM2022 总结
Toshiaki Koike-Akino

Executive Summary

Teo attended the 68th annual international Electron Device Meeting (IEDM) 2022 held in San Francisco, California,USA. The meeting is considered as the gold standard conference for reporting the latest development and breakthrough in semiconductor and device technology. This meeting was very well attended by the in-person conference of more than 2000 participants.

Similar to the previous years, this year conference includes areas in device design, multi-physics and device modeling, manufacturing, etc. In particular, it also includes nanometer CMOS technology, advanced novel quantum and nano-scale devices technology, optoelectronics, negative capacitance, advanced process technology and analog memory devices for AI. As for GaN technology, there were about 15 papers presented, which has one of the highest number of papers for a given technology at this meeting.

Specifically, papers using compact models of MRAM, memory devices such as ferroelectric devices, and ultra low temperature CMOS for quantum computing were presented. Models achieved uSec fast simulation using analytical functions as solutions. There were a few papers on SiC and one of which review conventional superjunction SiC power device, with the focus of using high-energy (MeV) implantations. There is also a paper on the use negative capacitance FETs which for the first time, reported the device design using a single-layer (SL)- graphene to achieve a subthreshold slope (SS) of 31 mV/dec with unnoticeable hysteresis.

As expected, Intel reported a new generation of integration architectures. Intel demonstrated that its performance includes 9x+ interconnect power reduction and density improvements.

GaN applications as usual, are chiefly divided into RF and power electronics. For power electronics, GaN device was reported to have a 10 A/cm2 current density at supply voltage of 50 V, which is higher than the state-of-the-art
Si devices. In another paper a 1200V/70mΩ GaN-on-sapphire devices demonstrates a high efficiency of >99% in hard-switched conditions of 900:450V buck converter at frequency of 50kHz. A vertical GaN superjunction p-n diodes are shown for both GaN and sapphire substrates with a breakdown voltage performance over 1100 V. A final paper on current and future potentials of vertical GaN power devices grown on GaN substrates was presented. Development of GaN bulk substrate, fundamental material properties, device epitaxial growth, advanced ion implantation and latest MOS interface are presented. 

There were more paper presented on GaN for the RF applications. N polar GaN with breakthrough performance at 94GHz at 5.8W/mm with 38.5% power efficiency. Monte Carlo thermal modelling of GaN and InP devices validated by partial experimental data was reported. Both transient and steady state studies were carried out and it reveals peak temperature increases are threefold larger than conventional study using bulk diffusion. A first demonstration of GaN HEMTs for both Power and RF applications on a common platform with Fe/C Co-doped Buffer was presented. In another paper, trapping in back barrier (BB) of GaN HEMTs was examined. BB trapping is alleviated by increasing 2DEG density Nsheet concentration. A novel device BB design criterion was proposed.

There is also another report on a comprehensive analysis of ESD for GaN on Si HEMTs. Transient I-V curves were verified with TCAD and pinpointed 3 different types of failure mechanisms. A heat spreader for GaN HEMTs is implemented with polycrystalline diamond. With a 500nm-thick all-around diamond, it lowers gate temperature at 9.5W/mm DC power without impact in device performances. In another paper, a high-K GaN NMOS transistor was demonstrated. A 100nm-source-field-plated with a 30nm LG GaN demonstrates a record fMAX=680GH. In another paper, a novel Hybrid gate p-GaN power HEMT technology is proposed to enhance Vth stability. It is experimentally demonstrated that the-HEMT can achieve higher gate reliability than commercial products. 

IEDM is a conference that covers many areas of semiconductor devices and technology. Though there were more than average number of papers presented on GaN at this meeting, the areas of application still only confined to RF
and power electronics applications. Potentially, GaN has many more other applications, such as ultra-high and ultra-low temperature operations, audio engineering and cable applications, etc, which this meeting fails to address. 

执行摘要

Teo 参加了在美国加利福尼亚州旧金山举行的第 68 届国际电子设备会议 (IEDM) 2022。该会议被认为是报告半导体和设备技术最新发展和突破的黄金标准会议。超过 2000 名参与者参加了此次会议。

与往年类似，今年的会议涵盖了设备设计、多物理和设备建模、制造等领域。特别是，它还包括纳米 CMOS 技术、先进的新型量子和纳米级设备技术、光电子学、负电容、先进工艺技术和用于 AI 的模拟存储设备。至于 GaN 技术，有大约 15 篇论文发表，这是本次会议上针对特定技术的论文数量最多的一次。

具体来说，论文使用了 MRAM、存储设备（如铁电设备）和用于量子计算的超低温 CMOS 的紧凑模型。模型使用分析函数作为解决方案实现了 uSec 快速模拟。有几篇关于 SiC 的论文，其中一篇回顾了传统的超结 SiC 功率器件，重点是使用高能 (MeV) 注入。还有一篇关于使用负电容 FET 的论文，首次报道了使用单层 (SL) 石墨烯的器件设计，实现了 31 mV/dec 的亚阈值斜率 (SS)，且滞后现象不明显。

正如预期的那样，英特尔报告了新一代集成架构。英特尔证明其性能包括 9 倍以上的互连功率降低和密度改进。

GaN 应用通常主要分为射频和电力电子。对于电力电子，据报道，GaN 器件在 50 V 电源电压下具有 10 A/cm2 的电流密度，高于最先进的 Si 器件。在另一篇论文中，1200V/70mΩ 蓝宝石基 GaN 器件在 900:450V 降压转换器的硬开关条件下，频率为 50kHz，效率高达 99% 以上。论文展示了垂直 GaN 超结 p-n 二极管，适用于 GaN 和蓝宝石衬底，击穿电压性能超过 1100 V。论文最后介绍了在 GaN 衬底上生长的垂直 GaN 功率器件的当前和未来潜力。论文介绍了 GaN 块体衬底的开发、基本材料特性、器件外延生长、先进离子注入和最新的 MOS 接口。

论文中介绍了更多关于 GaN 的 RF 应用。N 极性 GaN 在 94GHz 下以 5.8W/mm 的功率效率实现了突破性性能，功率效率为 38.5%。论文报告了通过部分实验数据验证的 GaN 和 InP 器件的蒙特卡罗热模型。进行了瞬态和稳态研究，结果表明峰值温度升高比使用体扩散的传统研究高三倍。首次展示了在具有 Fe/C 共掺杂缓冲层的通用平台上用于功率和射频应用的 GaN HEMT。在另一篇论文中，研究了 GaN HEMT 背障壁 (BB) 中的捕获。通过增加 2DEG 密度 Nsheet 浓度可以缓解 BB 捕获。提出了一种新颖的器件 BB 设计标准。

还有另一份关于全面分析 Si 基 GaN HEMT 的 ESD 的报告。使用 TCAD 验证了瞬态 I-V 曲线，并确定了 3 种不同类型的故障机制。GaN HEMT 的散热器采用多晶金刚石实现。使用 500nm 厚的全方位金刚石，它可以在 9.5W/mm 直流功率下降低栅极温度，而不会影响器件性能。在另一篇论文中，展示了高 K GaN NMOS 晶体管。 100nm 源场镀层采用 30nm LG GaN 实现了创纪录的 fMAX=680GH。在另一篇论文中，提出了一种新型混合栅极 p-GaN 功率 HEMT 技术来增强 Vth 稳定性。实验证明，该-HEMT 可以实现比商用产品更高的栅极可靠性。

IEDM 是一个涵盖半导体器件和技术许多领域的会议。虽然本次会议上发表的关于 GaN 的论文数量超过平均水平，但应用领域仍然仅限于 RF
和电力电子应用。GaN 可能还有更多其他应用，例如超高和超低温操作、音频工程和电缆应用等，而本次会议未能解决这些问题。

<https://www.merl.com/publications/docs/TR2023-013.pdf>

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/TR2023-013.pdf>

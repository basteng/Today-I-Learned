- [1.关于封装内光学 I/O 的三个常见误解](#1关于封装内光学-io-的三个常见误解)
- [2. Lizhenhao Paper](#2-lizhenhao-paper)
  - [2.1 《Bandwidth Analysis of High-Speed InGaN Micro-LEDs by an Equivalent Circuit Model》](#21-bandwidth-analysis-of-high-speed-ingan-micro-leds-by-an-equivalent-circuit-model)
    - [2.1.1 阅读笔记](#211-阅读笔记)
  - [2.2 《High-Speed Micro-LEDs based on Nano-Engineered InGaN Active Region towards Chip-to-Chip Interconnections》](#22-high-speed-micro-leds-based-on-nano-engineered-ingan-active-region-towards-chip-to-chip-interconnections)
- [3. Wanglei Paper](#3-wanglei-paper)
- [4. Ayar Labs](#4-ayar-labs)
  - [4.1 Ayar Labs 暗示产品将在未来 2-3 年内出货 (HPC wire)](#41-ayar-labs-暗示产品将在未来-2-3-年内出货-hpc-wire)
  - [4.2 Ayar Labs 旨在以光速消除人工智能的瓶颈 (Bloomberg podcast)](#42-ayar-labs-旨在以光速消除人工智能的瓶颈-bloomberg-podcast)
  - [4.3 光学 I/O 如何助力生成式 AI 的未来：与 Vladimir Stojanovic 的访谈](#43-光学-io-如何助力生成式-ai-的未来与-vladimir-stojanovic-的访谈)
  - [4.4 我们正在使用 Ayar Labs 的光学 I/O 解决方案重新思考下一代 AI 架构，以实现纵向扩展和内存扩展。](#44-我们正在使用-ayar-labs-的光学-io-解决方案重新思考下一代-ai-架构以实现纵向扩展和内存扩展)
  - [4.5 GlobalFoundries 与 Silicon Catalyst 合作，加速为半导体初创公司提供差异化​​技术解决方案](#45-globalfoundries-与-silicon-catalyst-合作加速为半导体初创公司提供差异化技术解决方案)
  - [4.6 光进铜退，已成定局？](#46-光进铜退已成定局)
  - [4.7 HPE 与 Ayar Labs 合作，为 Slingshot Interconnect 添加硅光子技术](#47-hpe-与-ayar-labs-合作为-slingshot-interconnect-添加硅光子技术)
  - [4.8 SuperNova™ 远程光源](#48-supernova-远程光源)
  - [4.9 人工智能基础设施的未来：利用光学 I/O 实现盈利之路](#49-人工智能基础设施的未来利用光学-io-实现盈利之路)
  - [4.10 如何在不破坏数据中心的情况下打造更强大的芯片 - economist](#410-如何在不破坏数据中心的情况下打造更强大的芯片---economist)
  - [4.11 ECOC 2024](#411-ecoc-2024)
  - [4.12 通过三重谐振光子分子实现高效宽带可调谐射频光转换](#412-通过三重谐振光子分子实现高效宽带可调谐射频光转换)
  - [4.13 光学技术：革新带宽密度和能效 示意图](#413-光学技术革新带宽密度和能效-示意图)
  - [4.14 Ayar Labs 与合作伙伴合作解决 HPC 和 AI 系统中的 I/O 瓶颈问题 - SC24](#414-ayar-labs-与合作伙伴合作解决-hpc-和-ai-系统中的-io-瓶颈问题---sc24)
  - [4.15 SC24 演示](#415-sc24-演示)
  - [4.16 2024.12.12获得AMD、Intel和Nvidia的1.55亿美元投资](#416-20241212获得amdintel和nvidia的155亿美元投资)
- [5. Avicena](#5-avicena)
  - [5.1《High Bandwidth GaN-based Micro-LEDs at Temperatures up to 400°C》](#51high-bandwidth-gan-based-micro-leds-at-temperatures-up-to-400c)
  - [5.2 硅光子学联合封装。 凉！ 但它实用吗？Bardia Pezeshki post at Linkedin](#52-硅光子学联合封装-凉-但它实用吗bardia-pezeshki-post-at-linkedin)
  - [5.3 Techopedia 专访 Bardia Pezeshki](#53-techopedia-专访-bardia-pezeshki)
    - [5.3.1 计算挑战：能源、处理能力和低延迟](#531-计算挑战能源处理能力和低延迟)
    - [5.3.2 “用光说话的芯片”](#532-用光说话的芯片)
    - [5.3.3 长距离光子学与短距离通信](#533-长距离光子学与短距离通信)
    - [5.3.4 用例和应用：现实生活中的光子学](#534-用例和应用现实生活中的光子学)
    - [5.3.5 底线](#535-底线)
  - [5.4 2024 Hotchips演讲](#54-2024-hotchips演讲)
  - [5.5 Data goes blue with GaN interconnects - Avicena《Compound Semiconductor》 VOLUME 27 ISSUE IV 2021](#55-data-goes-blue-with-gan-interconnects---avicenacompound-semiconductor-volume-27-issue-iv-2021)
  - [5.7 光学芯片互连有望加速计算应用 - Bardia Pezeshki electronicdesign 专访](#57-光学芯片互连有望加速计算应用---bardia-pezeshki-electronicdesign-专访)
  - [5.8 专利：使用基于 MicroOLED 的互连系统 SYSTEMS USING MICROLED-BASED INTERCONNECTS](#58-专利使用基于-microoled-的互连系统-systems-using-microled-based-interconnects)
  - [5.9 高温大带宽蓝色 InGaN/GaN 微型 LED](#59-高温大带宽蓝色-ingangan-微型-led)
  - [5.10 304 通道 MicroLED CMOS 收发器 IC，总计 1 Tbps，每比特亚皮焦耳容量](#510-304-通道-microled-cmos-收发器-ic总计-1-tbps每比特亚皮焦耳容量)
  - [5.11 专利：相干光纤束平行光链路  COHERENT FIBER BUNDLE PARALLEL OPTICAL LINKS](#511-专利相干光纤束平行光链路--coherent-fiber-bundle-parallel-optical-links)
  - [5.12 专利：使用 microLED 的芯片级光学互连 Chip-scale optical interconnect using microLEDs](#512-专利使用-microled-的芯片级光学互连-chip-scale-optical-interconnect-using-microleds)
  - [5.13 专利：带分线的 LED 互连，适用于内存应用 Led interconnect with breakout for memory applications](#513-专利带分线的-led-互连适用于内存应用-led-interconnect-with-breakout-for-memory-applications)
  - [5.14 专利：增强型 microLED，用于芯片间通信 Enhanced microLEDs for inter-chip communications](#514-专利增强型-microled用于芯片间通信-enhanced-microleds-for-inter-chip-communications)
  - [5.15 高温下高速蓝色 InGaN/GaN 微型 LED 的复合率分析 Recombination Rate Analysis of High-Speed Blue InGaN/GaN micro-LEDs at Elevated Temperatures](#515-高温下高速蓝色-ingangan-微型-led-的复合率分析-recombination-rate-analysis-of-high-speed-blue-ingangan-micro-leds-at-elevated-temperatures)
  - [5.16 使用基于 MicroLED 的光学链路互连网络 Interconnect networks using microled-based optical links](#516-使用基于-microled-的光学链路互连网络-interconnect-networks-using-microled-based-optical-links)
  - [5.17 304 通道 MicroLED CMOS 收发器 IC，总计 1 Tbps，每比特亚皮焦耳容量 304 channel MicroLED based CMOS transceiver IC with aggregate 1 Tbps and sub-pJ per bit capability](#517-304-通道-microled-cmos-收发器-ic总计-1-tbps每比特亚皮焦耳容量-304-channel-microled-based-cmos-transceiver-ic-with-aggregate-1-tbps-and-sub-pj-per-bit-capability)
  - [5.18 乐高演示 ECOC2024 Bardia Pezeshki - 20240921 Linkedin](#518-乐高演示-ecoc2024-bardia-pezeshki---20240921-linkedin)
  - [5.19 了解基于 microLED 的互连如何释放 HPC 和 AI 的潜力 - Jess Brown](#519-了解基于-microled-的互连如何释放-hpc-和-ai-的潜力---jess-brown)
  - [5.20 Avicena 在欧洲光通信会议上展示了基于 microLED 的 LightBundle 技术，覆盖范围达 30 米](#520-avicena-在欧洲光通信会议上展示了基于-microled-的-lightbundle-技术覆盖范围达-30-米)
  - [5.21 采用光纤的芯片到芯片垂直发射光通信](#521-采用光纤的芯片到芯片垂直发射光通信)
  - [5.22 Avicena 任命前 Oclaro 首席执行官 Greg Dougherty 为董事会成员](#522-avicena-任命前-oclaro-首席执行官-greg-dougherty-为董事会成员)
  - [5.23 20241023 加利福尼亚州硅谷举行的 PECC 峰会](#523-20241023-加利福尼亚州硅谷举行的-pecc-峰会)
  - [5.24 光学互连高带宽存储器架构专利](#524-光学互连高带宽存储器架构专利)
  - [5.25 CPO Example - MicroLED Parallel D2D Links](#525-cpo-example---microled-parallel-d2d-links)
    - [5.25.1 Parallel Versus Serial: Design of an Optical Receiver With Integrated Blue Photodetectors and Digitally Tunable Low-End Cutoff Frequency for MicroLED-Based Parallel Interchip Communication](#5251-parallel-versus-serial-design-of-an-optical-receiver-with-integrated-blue-photodetectors-and-digitally-tunable-low-end-cutoff-frequency-for-microled-based-parallel-interchip-communication)
  - [5.26 High Bandwidth GaN-Based Micro-LEDs at Temperatures up to 400 ◦C](#526-high-bandwidth-gan-based-micro-leds-at-temperatures-up-to-400-c)
    - [5.26.1 参考文献16 电注入 III 族氮化物发光二极管中的差异载流子寿命和传输效应](#5261-参考文献16-电注入-iii-族氮化物发光二极管中的差异载流子寿命和传输效应)
    - [5.26.2 参考文献12 III 族氮化物量子异质结构中的载流子动力学和库仑增强捕获](#5262-参考文献12-iii-族氮化物量子异质结构中的载流子动力学和库仑增强捕获)
  - [5.27 Cignal.ai评价Avicena](#527-cignalai评价avicena)
  - [5.28 Bardia Pezeshiki - MicroLED阵列有冗余](#528-bardia-pezeshiki---microled阵列有冗余)
  - [5.29 使用基于 LED 的并行性实现快速光学互连 gazettabyte](#529-使用基于-led-的并行性实现快速光学互连-gazettabyte)
  - [5.30 不同的光链路配置 - DR8 为 1.6 TB，使用 224G SerDes - PECC峰会](#530-不同的光链路配置---dr8-为-16-tb使用-224g-serdes---pecc峰会)
  - [5.31 LED同样有调制能力 - PECC峰会](#531-led同样有调制能力---pecc峰会)
  - [5.32 Avicena 采用uLED做为AI组网的光源](#532-avicena-采用uled做为ai组网的光源)
  - [5.33 SC24上的图片](#533-sc24上的图片)
  - [5.34 LightCounting在Supercompute 24 的亮点中介绍了 Avicena](#534-lightcounting在supercompute-24-的亮点中介绍了-avicena)
- [6. 《廉价光源可使人工智能更节能》Nature](#6-廉价光源可使人工智能更节能nature)
- [7. 多孔硅](#7-多孔硅)
- [8. -3 dB带宽](#8--3-db带宽)
- [9. LED和LD光调制的区别](#9-led和ld光调制的区别)
- [10.模拟光纤通信相关知识](#10模拟光纤通信相关知识)
  - [10.1 LED光通信背景知识](#101-led光通信背景知识)
  - [10.2 LED调制带宽](#102-led调制带宽)
- [11. PCIe诞生20年来最大变革！引入光学传输](#11-pcie诞生20年来最大变革引入光学传输)
- [12.厦门大学与阳明交大研发红/黄光Micro LED光通信技术](#12厦门大学与阳明交大研发红黄光micro-led光通信技术)
  - [12.1 MicroLED网 新闻](#121-microled网-新闻)
  - [12.2 厦门大学与国立阳明交通大学及 富士康 （鸿海研究院）- 使用蓝色、绿色和红色 InGaN µLED 进行高速 WDM 可见光通信的实验研究](#122-厦门大学与国立阳明交通大学及-富士康-鸿海研究院--使用蓝色绿色和红色-ingan-µled-进行高速-wdm-可见光通信的实验研究)
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
  - [23.1 Andy Bechtolshelm - 2024 Hotchips：](#231-andy-bechtolshelm---2024-hotchips)
  - [23.2 400G 以太网之路由 Bechtolsheim 的意图铺就](#232-400g-以太网之路由-bechtolsheim-的意图铺就)
  - [23.3 Andreas “Andy” Bechtolsheim ECOC 2024 演讲](#233-andreas-andy-bechtolsheim-ecoc-2024-演讲)
  - [23.4 20241023 加利福尼亚州硅谷举行的 PECC 峰会](#234-20241023-加利福尼亚州硅谷举行的-pecc-峰会)
  - [23.5 OCP](#235-ocp)
- [24.数据中心交换芯片](#24数据中心交换芯片)
- [25. 初创公司](#25-初创公司)
  - [25.1 Lightwave](#251-lightwave)
  - [25.2 POET](#252-poet)
- [26. RC-LED](#26-rc-led)
  - [26.1 可见光共振腔发光二极管原理及发展概况 - 北工大](#261-可见光共振腔发光二极管原理及发展概况---北工大)
- [27. 复旦 迟楠](#27-复旦-迟楠)
  - [27.1 硅基氮化镓微型LED，实现高速可见光通信信号探测](#271-硅基氮化镓微型led实现高速可见光通信信号探测)
    - [27.1.1 实验装置](#2711-实验装置)
  - [27.2 基于单个磷光白色 LED 的自适应比特分配 OFDM 的 2.0-Gb/s 可见光链路](#272-基于单个磷光白色-led-的自适应比特分配-ofdm-的-20-gbs-可见光链路)
  - [27.3 采用硬件预均衡电路的 Gb/s VLC 传输](#273-采用硬件预均衡电路的-gbs-vlc-传输)
  - [27.4 利用 GaN 激光器实​​现无处不在的通信 - Compound Semiconductor](#274-利用-gan-激光器实现无处不在的通信---compound-semiconductor)
- [28. Nvidia](#28-nvidia)
  - [28.1 Nvidia 展示了光学连接的 GPU 系统可能是什么样子](#281-nvidia-展示了光学连接的-gpu-系统可能是什么样子)
- [29. OELab动态](#29-oelab动态)
  - [29.1 清华大学罗毅院士团队到北京芯能交流技术 2022.9](#291-清华大学罗毅院士团队到北京芯能交流技术-20229)
- [30. 光互连的思考](#30-光互连的思考)
  - [30.1 光互连的思考：哪些铜互连将被光互连取代 VPIphotonics](#301-光互连的思考哪些铜互连将被光互连取代-vpiphotonics)
  - [30.2 信息图 Tuesday （IT）：光互连将以 5 比 1 甚至 10 比 1 的比率增长比 XPU 更快 Marvell](#302-信息图-tuesday-it光互连将以-5-比-1-甚至-10-比-1-的比率增长比-xpu-更快-marvell)
- [31. 新型深紫外微型 LED 阵列推动无掩模光刻技术发展 - 中科大](#31-新型深紫外微型-led-阵列推动无掩模光刻技术发展---中科大)
- [32. 用于传感、生产和通信的紫外线微型 LED - 柏林费迪南德-布劳恩研究所 (FBH)](#32-用于传感生产和通信的紫外线微型-led---柏林费迪南德-布劳恩研究所-fbh)
- [33. Introduction and Research Trends on Micro LED Technology](#33-introduction-and-research-trends-on-micro-led-technology)
- [34. Influence of dislocation density on internal quantum efficiency of GaN-based semiconductors - 余佳东](#34-influence-of-dislocation-density-on-internal-quantum-efficiency-of-gan-based-semiconductors---余佳东)
- [35. InGaN quantum dots for micro-LEDs - 汪莱](#35-ingan-quantum-dots-for-micro-leds---汪莱)
- [36. 基于等效电路模型的GaN基Micro-LED调制带宽分析 - 厦门大学/复旦 田鹏飞](#36-基于等效电路模型的gan基micro-led调制带宽分析---厦门大学复旦-田鹏飞)
- [37. 使用网络分析仪测量确定 LED 等效电路](#37-使用网络分析仪测量确定-led-等效电路)
- [38. 关于铜在计算领域的未来，需要记住的九件事 Marvell](#38-关于铜在计算领域的未来需要记住的九件事-marvell)
- [39. GaAs-AlGaAs 高亮度 LED 用于光通信系统的功率和调制带宽](#39-gaas-algaas-高亮度-led-用于光通信系统的功率和调制带宽)
  - [39.1 Google给出的总结](#391-google给出的总结)
  - [39.2 豆包给出的总结](#392-豆包给出的总结)
- [40. Ethernet over POF 塑料光纤以太网（Ethernet over POF）技术概述](#40-ethernet-over-pof-塑料光纤以太网ethernet-over-pof技术概述)
  - [一、塑料光纤（POF）的特点与应用](#一塑料光纤pof的特点与应用)
    - [（一）特点](#一特点)
    - [（二）应用](#二应用)
  - [二、POF与以太网](#二pof与以太网)
    - [（一）POF支持以太网的必要性](#一pof支持以太网的必要性)
    - [（二）POF以太网实现方式](#二pof以太网实现方式)
  - [三、总结](#三总结)
- [41. MicroLED Displays Industry status and Roadmap](#41-microled-displays-industry-status-and-roadmap)
- [42. MicroLED 展现出神经形态计算的潜力](#42-microled-展现出神经形态计算的潜力)
- [43. 850nm超结构单横模VCSEL芯片，助力短距离高速光通信 - 常瑞华团队](#43-850nm超结构单横模vcsel芯片助力短距离高速光通信---常瑞华团队)
- [44. 片间光互连发展态势分析 - 信通院 刘璐团队](#44-片间光互连发展态势分析---信通院-刘璐团队)
- [45. 微软：基于Micro-LED＋CIS的模拟光学计算实现加速计算](#45-微软基于micro-ledcis的模拟光学计算实现加速计算)
  - [45.1 arXiv上的论文](#451-arxiv上的论文)

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

### 2.1.1 阅读笔记

- 其实一个LED可以看做一个通信系统，输入电压即输入，输出即LED的光。实际上等效电路可以计算频率响应曲线 H(f)，也即信号与系统里的传递函数，通过传递函数就可以计算-3dB带宽。
- 引用模型的参考文献，好好读一下，尤其是参考文献19，Avicena 400℃的文章里也提到这篇文章
  
  [19].Differential carrier lifetime in AlGaN based multiple quantum well deep UV light emitting diodes at 325 nm
  [20].Capacitance measurements of p-n junctions: Depletion layer and diffusion capacitance contributions


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

## 4.4 我们正在使用 Ayar Labs 的光学 I/O 解决方案重新思考下一代 AI 架构，以实现纵向扩展和内存扩展。

![image](/picture/ayarlabs1.jpg)

## 4.5 GlobalFoundries 与 Silicon Catalyst 合作，加速为半导体初创公司提供差异化​​技术解决方案

加州硅谷和纽约州马耳他，2024 年 9 月 9 日——GlobalFoundries（纳斯达克股票代码：GFS）（GF）和全球唯一专注于半导体解决方案的孵化器+加速器Silicon Catalyst今天宣布，GF 已作为战略合作伙伴和实物合作伙伴 (IKP) 加入孵化器的半导体初创企业生态系统。此次合作将为创新型初创公司提供 GF 差异化平台，以加速下一代物联网、汽车和生成式人工智能应用的开发和商业化，同时预测医疗和量子计算等未来增长市场。

作为战略合作伙伴，GF 将与 Silicon Catalyst 密切合作，招募、评估和选择寻求参与其计划的早期初创公司。作为 IKP 生态系统的成员，GF 将提供 PDK、MPW、基础 IP 和参考设计，以加快 GF 22FDX®、硅光子学和氮化镓 (GaN) 平台上已获批准的早期公司的产品上市时间。

Silicon Catalyst 校友 Ayar Labs 首席执行官兼联合创始人 Mark Wade 表示：“我们与 GlobalFoundries 的长期合作关系对我们将突破性的光学 I/O 解决方案推向市场起到了重要作用。与 Silicon Catalyst 等项目合作，再加上使用 GlobalFoundries 的平台，使 Ayar Labs 等公司能够专注于我们最擅长的领域——突破 AI 基础设施的界限，以应对 AI 模型日益增长的规模和复杂性。”

格芯首席技术官 Gregg Bartlett 表示：“格芯市场领先的差异化关键芯片技术根植于创新与协作。通过与 Silicon Catalyst 合作，我们将与早期初创公司合作，让我们能够亲眼目睹新兴创新，突破我们差异化技术的界限，提供定制解决方案，让这些公司在进入市场时获得竞争优势。”

Silicon Catalyst 首席执行官 Pete Rodriguez 表示：“GlobalFoundries 致力于推动创新，为客户提供差异化​​技术解决方案。我们很高兴他们加入 Silicon Catalyst 生态系统。我们的合作为初创公司提供了一个独特的机会，让他们与 GF 合作，获得其差异化、经济高效的解决方案。这一宝贵的合作有望推动半导体创新的新一轮发展，同时帮助新公司应对从创意到实现的挑战。”

Silicon Catalyst 的生态系统包括 350 多名半导体行业顾问、14 个战略合作伙伴、70 个实物合作伙伴、广泛的投资者网络以及与国内外主要学术机构的紧密联系。此次合作将使 GF 能够深入了解半导体行业。 

欢迎加入 Silicon Catalyst 团队，参加 9 月 9 日至 12 日在加利福尼亚州圣何塞举行的 AI 硬件和边缘 AI 峰会，Silicon Catalyst 投资组合公司的三位首席执行官将在技术会议上发言。与会者受邀参观 AI 创新展区的 Silicon Catalyst 展位，以了解有关 GF 和 Silicon Catalyst 合作伙伴关系的更多信息，以及它将如何帮助半导体初创公司构建支持 AI、量子计算、汽车和物联网等变革性行业的基础解决方案。

<https://gf.com/gf-press-release/globalfoundries-and-silicon-catalyst-partner-to-accelerate-differentiated-technology-solutions-for-semiconductor-startups/>

## 4.6 光进铜退，已成定局？

Ayar Labs提出的三个性能指标，吞吐量、交互性、处理的盈利能力

![image](/picture/ayar-simulator-figures-of-merit.jpg)

Nvidia 2026 年路线图上的未来“Rubin”GPU 以及 2027 年内存升级，可能会采用当前的电气/铜线方式和假设的光纤/光纤方式进行架构。看一下这个：

![iamge](/picture/ayar-simulator-next-gen-gpu-table.jpg)

如下所示，随着现有的 Hopper 和 Blackwell 配置从 8 个 GPU 扩展到 64 个 GPU，所有机器都被推入批量性能领域，只有使用铜 NVLink 互连的 Rubin 机架式机器才能进入人机领域。但是，借助节点内和节点间的光学 I/O 以及扩展到 256 个 Rubin GPU，Nvidia 可以构建一台可以扩展到人机和机器对机器领域的推理机，同时在交互性和成本方面提供可接受的改进。

![image](/picture/ayar-simulator-hopper-blackwell-rubin-gpt-x.jpg)

该图表是 Ayar Labs、Eliyan、Avicena、Lightmatter 和 Celestial AI 等公司的广告。我们强烈怀疑 Rubin 会将 NVLink 转移到光学互连，坦率地说，考虑到Nvidia 多年前所做的原型设计以及 Nvidia 已经与 Ayar Labs 以及很可能与上面提到的其他一些公司合作的工作，我们已经预料到这样的机器了。

NVLink 只是一种协议，现在或许是时候将其转移到光学传输中了。我们迫不及待地想看看 Nvidia 会在这里做些什么。在机架中塞入更多 GPU 并将功率密度提高到 200 千瓦或人们谈论的疯狂的 500 千瓦可能不是答案。光学互连会将这个铁芯稍微隔开一点，也许足以防止光学器件出现不良行为。

<https://www.nextplatform.com/2024/09/13/copper-wires-have-already-failed-clustered-ai-systems/>

## 4.7 HPE 与 Ayar Labs 合作，为 Slingshot Interconnect 添加硅光子技术

随着这些设备的带宽不断增加，电信号传输距离也随之缩短。到目前为止，材料科学家以及 PHY 和 SerDes 设计师已经能够避免这种情况的发生，但迟早，元素周期表中可用的原子会耗尽，这就是硅光子学的发展如此重要的原因。

惠普企业 (Hewlett Packard Enterprise) 在光通信方面也不甘示弱，光通信是 The Machine 的核心之一，The Machine 是一个以内存为中心的并行系统，由惠普实验室于多年前构建，作为光互连和内存池的试验台。HPE 也是 Gen-Z 协议的支持者，甚至在美国能源部 PathForward 计划的支持下为服务器创建了光学 Gen-Z 交换机和电光 Gen-Z 适配器，我们早在 2019 年 9 月就对此进行了详细介绍。此后不久，与竞争对手 HPE 一起作为 Gen-Z 的主要支持者的戴尔展示了基于 Gen-Z 技术的内存服务器。

但是，当它考虑如何将硅光子学应用于未来几代 Slingshot 以太网互连的交换机 ASIC 和网络接口时（我们最近与 HPE 讨论了这个问题），该系统制造商决定与 Ayar Labs 合作，这是一家由美国国防高级研究计划局资助的硅光子学初创公司，于 2019 年初推出了首款电光芯片，我们在当年夏季晚些时候的 Hot Chips 2019 会议上了解了很多相关信息。Ayar Labs 认为，超过 112 Gb/秒的本机信令（在消除编码开销后转换为 100 Gb/秒），电信令将遇到瓶颈。正如我们最初在本文指出的那样，四年前，安迪·贝克托尔斯海姆（Andy Bechtolsheim，Arista Networks、Granite Systems 和 Sun Microsystems 的创始人）就曾表达过这种观点，但现在看来，到 2025 年，电信号将再次获得喘息机会，并向 224 Gb/秒（编码后为 200 Gb/秒）的原生速度迈进。障碍已经消失。但在未来几年的某个时候，它将成为真正的障碍。

每个交换机 ASIC 和每个网络适配器都将利用 50 Gb/秒、100 Gb/秒和未来的 200 Gb/秒信号、NRZ 和 PAM-4 编码（可能还有其他级别的脉冲幅度调制编码）和通道数的组合来创建 200 Gb/秒、400 Gb/秒、800 Gb/秒甚至 1.6 Tb/秒的设备。但根据英特尔 Barefoot Networks 网络团队和 Broadcom 硅光子学团队已经创建的研究和原型，我们认为，在未来一两代互连中，这堵电信号墙必须被硅光子学突破。（我们指的是路线图，而不是即将从晶圆厂推出的产品。）

这并不遥远，因此 HPE 和 Ayar Labs 建立了合作伙伴关系。

Terpstra 解释道：“如果你看看 400 Gb/秒或 800 Gb/秒交换机的外观，就会发现其内部设计越来越复杂。过去，对于带宽较低的交换机设计，你有一个交换机 ASIC，只需将电信号一直传输到前面板即可。在某些情况下，现在你无法再这样做，或者必须使用特殊电缆。我们将在 Slingshot 产品组合中遇到这个问题，我们与 Ayar Labs 的交流已经一年多了，他们通过创建基于硅光子学和集成封装的光互连，在该领域处于领先地位。他们不只是要制造组件，他们实际上想要创建一个生态系统，这使他们成为我们的完美合作伙伴。其他组件供应商将需要相同类型的集成、共封装硅光子学。我们必须有异构解决方案，我们不能想出专有的东西。这种方法存在一些阻力。我们有十年的硅光子学研究经验，我们本可以将它产品化，但我们故意选择不这么做。我们真正需要的是广泛的行业联盟，这样我们才能真正创建合法的异构系统。”

Ayar Labs UK 商业运营高级副总裁兼董事总经理 Hugo Saleh 说，这正是 Ayar Labs 想要做的事情。

Saleh 解释说：“由于我们将光从封装中传输出去，因此我们希望专注于构建一个生态系统，该生态系统可以协调使用的波长数量、波长之间的距离以及峰值的高度。” “我们对我们构建的光学 I/O 和芯片感到兴奋，但我们专注于光的特性，以便我们能够实现未来供应商之间的互操作性。要使这个生态系统蓬勃发展，必须有其他公司参与这一业务。这就是为什么我们很高兴与 HPE 合作，因为他们可以设定期望并对供应商提出要求。”

自从退出隐身模式以来，Ayar Labs 一直在与英特尔进行某种形式的合作，因此可以合理地预期，一些超大规模企业和云构建商可能会开始尝试，而戴尔、浪潮、联想和 IBM 也可能效仿。思科系统可能会更难一些，因为它有自己的网络业务。但正如我们多次讨论的那样，硅光子学将成为实现可覆盖整个数据中心的分解和可组合基础设施的关键技术之一。

作为与 Ayar Labs 合作协议的一部分，惠普的风险投资部门 Hewlett Packard Pathfinder 将向这家 SiPho 新创公司投入一笔未披露金额的资金。Ayar Labs 已筹集了 6450 万美元的种子资金以及两轮风险投资（不包括 HPE 的投资），投资者包括英特尔资本和 Globalfoundries，以及 BlueSky Capital、Applied Ventures、Castor Ventures 和 Lockheed Martin Ventures 等。

<https://www.nextplatform.com/2022/02/24/hpe-taps-ayar-labs-to-add-silicon-photonics-to-slingshot-interconnect/>

## 4.8 SuperNova™ 远程光源

SuperNova™ 远程光源是 Ayar Labs TeraPHY™ 光学 I/O 小芯片解决方案的支柱，用于下一代 AI 架构，提供多达 16 种波长的光，并为多达 16 个端口供电。 

SuperNova™ 的核心是我们的 16 波长分布式反馈 （DFB） 激光阵列，这是一种先进的光子芯片，可在单个阵列中提供多种波长的光，以优化、简化和降低波分复用 （WDM） 应用的封装成本。 

欢迎在 2024 年 9 月 23 日至 25 日的法兰克福 ECOC 展会期间在 C106 展位观看我们现场演示这项开创性的使能技术。

![image](/picture/Ayarlabs_lightsource.jpg)

## 4.9 人工智能基础设施的未来：利用光学 I/O 实现盈利之路

高盛最近的一份报告显示，科技公司、企业和公用事业公司未来几年将在人工智能基础设施上投入超过 1 万亿美元。尽管投入如此巨额，但人工智能领域仍未实现重大盈利突破。到目前为止，硬件堆栈（芯片制造商、硬件制造商以及主板和机架制造商的代工厂）一直是这笔资本支出的主要受益者。然而，目前产出是否能与投资回报率相称仍存在疑问。

AI 基础设施的根本挑战源自芯片级互连瓶颈，这会影响堆栈顶部的单位经济效益。封装内光学 I/O 代表着一种解决方案和转折点，能够将下一代 GenAI 的盈利能力提高 20 倍，并将交互性提高 3-4 倍。

在这篇博文中，我们讨论了影响人工智能未来盈利能力的三个关键问题：

 1.当今大规模人工智能系统最大的瓶颈在哪里？
 2.有哪些技术和产品可以解决这些问题？
 3.我们还能做些什么来提高新应用的盈利能力和性能领域？

**当今人工智能系统的最大瓶颈**

ChatGPT 推出已近两年，SaaS 公司的淘金热似乎已停滞。随着 AI 模型的规模和复杂性不断增长，底层基础设施的功能和经济性无法按需扩展。事实上，由于总拥有成本 (TCO) 高昂，且电气 I/O 产生的带宽距离瓶颈限制了硬件架构的性能，AI 应用的单位经济性（例如每代币美元）仍然过高。

我们的最新研究概述了我们面临的挑战，并强调了对 AI 基础设施采用新方法的需求——利用光的方法。这种新方法是释放 AI 盈利能力、解决带宽距离瓶颈以及提供扩展结构路线图的关键。

AI 的需求和复杂性不断增长，增长速度快于内存带宽和容量，这导致计算成本越来越高。在当今的 AI 基础设施中，传统的铜和可插拔光学器件无法有效地将计算进步从封装扩展到集群。这导致效率低下、功耗增加和成本增加。同时，铜互连将扩展域大小限制在单个机架上。这通过限制有效内存带宽和容量来限制集群性能。最终，这限制了在这种集群上运行的推理模型的盈利能力和交互性。（图 1）

“铜线互连已经无法以经济的方式支持 AI 工作负载。行业目前面临的情况是，硬件制造商需要大幅提高这些系统的经济高效吞吐量。否则，我们都会走向互联网泡沫。”

Ayar Labs 首席执行官 Mark Wade

![image](/picture/Comparison-of-throughput-versus-profitability-1.webp)
图 1：当今领先的 AI 扩展解决方案之一与潜在未来解决方案的吞吐量与盈利能力比较。

**扩展 GenAI 推理性能**

让我们首先考虑一下目前可用的选项：使用电气 I/O 增强扩展结构的性能需要在机架中添加更多加速器，这会增加机架的功率密度。或者，可插拔光学器件可以连接机架以外的加速器，从而提高交互性，但其高功率和高成本会损害盈利能力。

这导致 GenAI 推理受到两个因素的限制：

1.**内存带宽**：设置将注意力缓存和模型权重从内存加载到 GPU 所需的时间
2.**扩大结构**：确定专家/张量并行 GPU 之间传达激活所需的时间。

扩展GenAI 的整体推理性能需要增加扩展域内并行工作的 GPU 或加速器的数量。解决这些问题至关重要，需要对 AI 基础设施进行创新变革——转向基于光的解决方案——以使行业实现盈利。

**加速新应用的盈利之路**

盈利能力是人工智能应用的主要指标，也是每家公司（和投资者）都在争取的最终目标——不同的互动水平会影响这一目标的实现。为了更好地理解人工智能的盈利之路，我们引入了三个大规模人工智能的品质因数（图 2）： 

- 吞吐量：该指标是 AI 应用盈利能力的关键组成部分。其定义为用户数量除以每个输出令牌的时间。
- 交互性：这表示在查看在其上运行的不同推理工作负载时，AI 模型的响应速度和交互速度有多快。它被定义为每输出 token 的时间除以 1。
- 盈利能力：该指标旨在提供成本结构的概念以及应用程序实现盈利空间的能力。它被定义为吞吐量除以成本和功率。

![image](/picture/Figures-of-merit-1.webp)

图 2：大规模 AI 的品质因数。

通过关注这些指标，我们可以更好地评估和提高人工智能应用的盈利能力，以支持行业的增长和创新。

为了准确预测 AI 推理应用级性能，我们创建了一个系统架构模拟器（图 3）来得出这些应用级性能指标。该工作负载模拟器考虑了各种输入，包括模型规格、技术组件、模型优化、算法细节、网络结构和成本。我们甚至花时间和精力来调整该模拟器以适应当今和未来市场上的各种模型和 GPU。

![image](/picture/Predicting-AI-inference-1.webp)

图 3：Ayar Labs 的系统架构模拟器。

**光学 I/O：GenAI 盈利的关键**

需要一种新的方法来扩大性能，以提高 AI 的单位经济效益和每代币每秒美元的“代币经济学”。光学 I/O 提供了明确的解决方案和盈利途径（图 4 和图 5）。如何实现？通过突破带宽距离瓶颈，基于光学 I/O 的扩大结构可增强推理和训练的应用级性能，优化 TCO 指标，包括吞吐量、交互性和盈利能力。

![image](/picture/Composable-AI-Infrastructure-1.webp)

图 4：使用 Ayar Labs 的光学 I/O 扩展网络。

![image](/picture/Next-Gen-AI-Platform-1.webp)

图5：下一代AI平台的理论路线图。

传统的电气 I/O 需要将所有东西塞在一起才能提高性能，从数据中心基础设施的角度来看，这会带来两个问题：

1.向机架输送电力的挑战在于，数据中心基础设施并非设计为每个机架输送 120 kW 的电力。（典型的 CPU 机架为 20 kW，加速器机架高达 40 kW）
2.管理机架内功率密度的挑战要求冷却解决方案取得重大进步。

光学 I/O 可缓解这些压力。通过使扩展结构能够连接每个集群的更多 GPU 或加速器，同时跨越更大的距离，光学 I/O 可提高集群性能，而无需增加每个机架的功率。实际上，您可以部署每个机架 16 个或 32 个 GPU 或加速器，并构建更多更适合数据中心基础设施的机架，所有这些都通过光学 I/O 连接。（图 6）。

![image](/picture/Scale-out-scale-up.png)

图 6：Ayar Labs 的光学 I/O 非常适合 AI 扩展结构。

数据中心运营商正在评估这些解决方案，以更好地理解价值主张。最终目标是推动“代币经济学”直至人工智能应用的大幅改进，确保当前对人工智能的投资能够带来可观的经济产出和盈利能力。这包括数据中心和用户的盈利能力，同时通过增强交互性（用户和机器与人工智能模型交互的速度）为客户提供明显的经济价值。

随着光学 I/O 作为关键技术的出现，我们可以通过解决功率和热密度问题并突破带宽距离瓶颈来扩展交互性和连接性的盈利领域。

![image](/picture/GPT-4-Performance-Estimates-1.webp)

图 7：对于当今的 GPT-4 模型的批量和人机推理工作负载，光学 I/O 可以显著提高盈利能力 6 倍、交互性 4 倍。

我们的系统架构模拟器发现，对于当今的 GPT-4 模型（例如具有 1.8 万亿个参数的模型），光学 I/O 可以显著提高批量和人机推理工作负载的盈利能力 6 倍，交互性 4 倍（图 7）。下面是对批处理和人机交互的简要说明：

- **批处理**：批处理或离线推理是指机器学习模型在大型数据集上运行，并根据一批信息生成输出。这些批处理运行通常按某个重复的时间表（例如每小时或每天）生成。然后，这些推理存储在数据库或文件中，可供开发人员或最终用户使用。批处理的示例包括电子商务网站上的产品评论摘要或基于观看习惯的流媒体电影推荐。
- **人机交互**：通过人工参与或实时/在线服务，我们无需等待数小时甚至数天才能批量生成预测，而是可以在需要时立即生成预测 - 立即将这些结果提供给用户。人机交互的目标通常是优化模型每秒可以处理的交易数量。正如您可能想象的那样，示例包括 ChatGPT 和我们今天从公司看到的任何 copilot 产品。

**对未来 GPT-X 模型及其他方面的影响**

展望未来两三年，随着具有约 14 万亿个参数的 GPT-X 模型（模型大小增加了 8 倍，低于每两年 16-25 倍的预计趋势）变得司空见惯，光学 I/O 的优势将变得更加明显。（图 8）

![image](/picture/GPT-4-and-GPT-X-1.webp)

图 8：当前的 GPT-4 模型和对 GPT-X 的估计。

根据我们的系统架构模拟器，光学 I/O 有可能将盈利能力提高 20 倍，同时将交互性提高 3-4 倍。事实上，光学 I/O 成为 GPT-X 未来模型所有用例的唯一可行技术——并且是超越当今人机交互的未来代理推理模型可能性的关键。（图 9）

![image](/picture/GPT-X-Performance-Estimates-1.webp)

图 9：光学 I/O 有可能将未来 GPT-X 模型的盈利能力提高 20 倍，同时将交互性提高 3-4 倍。

只有光学 I/O 才能让多个 AI 副驾驶或代理在所谓的机器对机器多代理交互中相互“交谈”。想象一下，一位工程师正在研究一项专利，并利用副驾驶来利用两个代理的专业知识。第一个代理专注于工程，第二个代理专注于法律。这两个代理共同努力，提供快速、相关的见解，从而提高副驾驶在专利开发方面对工程师的价值。基于当今的能力，这很难想象，但在光学 I/O 的帮助下，这比人们想象的更接近现实。

尽管 GenAI 可能无法满足消费者和投资者的期望，但盈利之路仍然可行。光学 I/O 为 AI 打开了闸门，改善了 AI 应用的单位经济性，打破了电气 I/O 带来的带宽距离瓶颈。这将使 AI 系统和人类都能获得更好的盈利能力和交互性，同时也使未来的多智能体推理模型超越当今的人机互动。

<https://ayarlabs.com/blog/the-future-of-ai-infrastructure-a-path-to-profitability-with-optical-i-o/?utm_campaign=240924-september-newsletter&utm_medium=email&_hsenc=p2ANqtz-_-OmEwtwbWFmv9IfVoPwsbLuvDgtXFMhYVUncG9d9XwUAROM7IoIcTHV9vHv8Fx1gzOw_rxwMaR9BOjVBvruqF6MyCzg&_hsmi=326160012&utm_content=326160012&utm_source=hs_email>

## 4.10 如何在不破坏数据中心的情况下打造更强大的芯片 - economist

英伟达是人工智能 ( ai ) 淘金热的领头羊，其推出的 Blackwell芯片包含 2080 亿个晶体管，分布在两个“芯片”上，每个“芯片”的面积约为 800 平方毫米，用于容纳处理器电路。两个芯片通过每秒 10 TB（即 1 万 GB）的芯片间连接连接。每个芯片两侧是四个高带宽内存 ( hbm ) 芯片块，总共可存储 192 GB 的数据。用于制造这种巨型芯片的先进封装方法现在备受关注，有人猜测它们可能会导致生产延迟。

Blackwell 将不同部件组合在一起，表明了芯片制造商在提高计算能力的同时控制能耗时必须突破的技术极限。一年下来，这些价值 7 万美元的巨型芯片将消耗 5.2兆瓦时，大约相当于美国普通家庭能耗的一半。增加更多晶体管是提高芯片处理能力的最佳方式：与芯片间数据传输相比，单个芯片内的通信速度可能快一千倍，能耗却低一百倍。但自从 Dennard 缩放定律在 2000 年代中期遇到瓶颈以来，缩小晶体管并没有显著提高能效。Gordon Moore 提出了另外两个塞入更多晶体管的技巧：增加芯片尺寸（即让芯片更大）和利用“设备和电路的巧妙性”。1971 年，英特尔处理器 4004 的芯片尺寸为 12 平方毫米。当前的光刻工具无法制造大于 800 平方毫米的芯片，大约相当于每个 Blackwell 芯片的尺寸。电路巧妙是唯一的其他途径。

一个聪明的想法是更有效地利用芯片面积。从侧面看，半导体芯片就像一个多层蛋糕，底层是构成晶体管的层，顶层堆叠着 10-20 层金属线。尖端芯片可以使用近 100 公里的细金属线（数十亿个晶体管之间的连接总和）。这使芯片变成了一条拥挤的数据和电源线高速公路。顶层是厚厚的金属线，用于在芯片上分配电力。由于这些粗大的电源线从顶层一直延伸到底层以连接到晶体管，它们可以占用用于路由电信号的近五分之一的区域。

烤蛋糕

为了腾出更多空间，领先的代工厂目前正在研究“背面供电”，即将粗电源线移到晶体管下方的一层，即芯片的“背面”。这样做有三个好处。首先，它释放了空间，使晶体管上方的所有区域均可用于路由数据。由于金属线拥堵情况减少，晶体管组（称为门）可以更紧密地封装在同一空间中。其次，晶体管下方的电源线需要更短的连接来连接它们，而这些连接可以更粗，从而使供电更节能。最后，这些坚固的电源线在需求激增期间不易受到电压尖峰的影响，从而确保晶体管更快地切换。结果是无需缩小晶体管尺寸即可获得速度更快、更节能的芯片。

但是将电源线移到晶体管下方会在制造过程中引入额外的步骤。通常，一旦芯片的多层结构构建完成，就会将晶圆翻转并封装在将内部电路与外界连接的封装中。对于背面供电，翻转之后必须进行抛光和添加电源线。额外的步骤值得付出努力。2023 年，英特尔采用了背面供电和更智能的组件布局，这使得晶体管速度提高了 6%，封装密度提高了 10%，而组件尺寸不小于以前使用的组件。

另一种策略是不要将所有功能都塞进一个芯片，而是为每项任务选择最佳制造技术。虽然高速处理器需要最先进的节点，但芯片的其他部分，比如与外界通信的模块，并不需要最小的晶体管。将芯片分成更小的块（称为“芯片”），然后将它们封装在一起，可以让芯片制造商将芯片上的最大面积用于处理单元，因为其余电路被转移到其他芯片上。与封装外的电路相比，同一封装中的芯片之间的通信速度更快，能耗更低。

![](/picture/20240921_TQC934-Artboard_1.png)
长期以来，封装一直是芯片制造的弱势方。代工厂专注于生产硅晶圆。但随着芯片的兴起，封装成为人们关注的焦点（见图）。芯片的组装方法是将采用不同工艺技术的多个芯片并排放置在称为中介层的层上。然后，这些芯片通过“微凸块”粘合到中介层上。

中介层位于通常由有机树脂制成的基板上，充当桥梁，通过高密度布线将芯片相互连接，并通过封装将它们连接到外界。这允许芯片之间快速传输数据并提高功率效率。Nvidia 的 Blackwell 处理器使用台积电的版本，将其两个芯片和八个hbm芯片组合成一个超级芯片。台积电计划开发比最大芯片大六倍的中介层，以承载多个处理芯片和hbm堆栈。

与此同时，英特尔公布了放弃使用树脂、将芯片堆叠在玻璃上的计划。玻璃的超平整度更适合细间距、高密度布线，并且具有更好的热稳定性和机械稳定性，尤其是在较大尺寸时。该公司表示，这种转换可以将连接密度提高十倍于有机中介层。

芯片技术的下一个重大飞跃是将芯片直接堆叠在一起，从而缩短芯片之间的距离。内存制造商是此类 3D 堆叠的先驱。用于专业AI芯片的HBM通常堆叠 8 到 12 个内存芯片，这些芯片通过高容量布线连接，从而增加内存和处理器之间的带宽。

训练人工智能模型需要数百个处理器连接在一起
如今，人工智能芯片也纷纷效仿。3D封装每平方毫米可提供10,000个连接，而并排封装每平方毫米可提供25个连接。更多连接意味着芯片之间​​的数据传输更顺畅。它还更节能，移动每个比特所需的能量不到前一版本的1%。另一家芯片设计公司AMD制造的MI 300X是Nvidia H 100的竞争对手，它将八个加速器芯片堆叠在四个中介层芯片上，以及八个HBM堆栈，都堆叠在一个封装中。

这些收益是有代价的。AMD 的 Samuel Naffziger指出，由于多个芯片在组合成单个封装之前需要进行测试，因此 3D封装增加了制造过程的时间和复杂性。将芯片封装在一起还会增加芯片中的热密度。为了便于散热，芯片设计师将产生最多热量的层放置在堆栈的顶部，并将产生热量较少的组件（如内存）放置在下面。

训练人工智能模型需要庞大的系统，其中数百个处理器连接在一起。即使将芯片塞进封装中，大量数据仍然需要在这些独立的处理器及其连接的内存芯片之间传输。铜线是连接主板上组件的常用方法，速度慢且浪费能源。因此，一些公司开始使用光来加快速度。

光纤电缆是互联网的骨干，承载着 99% 的洲际互联网流量。这些电缆还用于短距离连接数据中心的机架。在这两种情况下，光纤两端的设备都会将信号从电脉冲转换为光，反之亦然。现在，光通信也正在向硅片领域迈进。<font color=red>美国初创公司 Ayar Labs 是开发用于处理器之间光通信的芯片组的公司之一</font>。它的芯片组位于封装的边缘，可将电信号转换为光，然后通过光纤发送。在接收端，另一组芯片组将光转换回电信号，并将数据传送给封装中的处理器。该公司声称，这将使芯片间带宽提高十倍，能效提高八倍。

郊区和摩天大楼

节能、高速芯片间通信的终极飞跃是将所有芯片压缩成一个芯片，包含多层处理器、内存和传感器。这样芯片的不同部分之间的连接就更加紧密了。斯坦福大学的 Subhasish Mitra 将此比作从庞大的郊区布局转变为高耸的摩天大楼。

就像摩天大楼有电梯供人们上下穿梭一样，这个巨型芯片需要数百万个连接来在计算层和内存层之间传输数据。这些电梯还可以帮助保持芯片凉爽，将热量传导到底层。最终，芯片制造商可以将这些芯片塔并排聚集在一起。米特拉先生认为，这可以将能源效率提高一千倍。

制造这样的芯片非常困难。传统晶体管的制造温度可能超过 1,000°C。由于晶体管位于多层，摩天大楼晶体管上纵横交错的金属线会熔化。为了实现垂直芯片的愿景，上层的逻辑和内存技术必须在低于 400°C 的温度下制造。较新的晶体管技术（如碳纳米管和 2d材料）可以在低于 400°C 的温度下加工，可能比硅更适合。米特拉先生已经在 90nm 节点上展示了这种芯片的一个版本，该版本由碳纳米管和内存层构建而成。

2015 年，戈登·摩尔承认，他对自己预测的持续时间感到“惊讶”。但他认为，要将摩尔定律再延续几十年，需要“大量优秀的工程技术”。台积电认为，到 2030 年，这些方法的结合可以在芯片上产生一万亿个晶体管。芯片制造商显然还没有完成。

<https://www.economist.com/technology-quarterly/2024/09/16/how-to-build-more-powerful-chips-without-frying-the-data-centre>

## 4.11 ECOC 2024

• Altera 、Ayar Labs 和 Corning Optical Communications 展示了采用康宁高级玻璃波导模块的 4 Tbps 光学 FPGA 的概念验证
• Ayar Labs 和 Sivers Photonics 现场演示了 Ayar Labs 的业界首个符合 CW-WDM MSA 标准的 16 波长光源和 Sirers 的 16 波长 DFB 激光阵列

## 4.12 通过三重谐振光子分子实现高效宽带可调谐射频光转换

我们最近在 Optics Letters 上发表的题为“Efficient wideband tunable radio frequency–optical conversion via triply resonant photonic molecules”的论文被选为“聚焦光学”。你可以在这里找到这项工作的一个很好的总结（https://lnkd.in/eePZ9a-w）。该论文现在对任何感兴趣的人开放获取。

在这项工作中，我们提出了一种新颖的三腔配置，通过为射频光转换过程提供目标射频载波的宽带可调谐性，该配置可以在 5G/6G 无线通信、毫米波光子学和雷达系统中发挥重要作用。在我攻读博士学位的早期，我们成功地演示了该设计与 GlobalFoundries 的 45RFSOI 平台上的 LNA 的单片集成，所有这些都在单个芯片上。虽然完整的期刊论文目前正在进行中，但您可以在此处 （https://lnkd.in/eC_TDsUf） 访问我们实验演示的相关会议论文。

特别感谢 Milos Popovic 教授和 Xinchang Zhang 教授对论文的贡献。这项工作由最近的 NSF FuSe 计划奖资助，并与加州大学伯克利分校的 Vladimir Stojanovic 教授和 Ruocheng Wang 合作完成。我们还要感谢 Ayar Labs 和 GlobalFoundries 多年来支持这些单片电子光子平台的开发，使这些 CMOS 工艺能够实现如此复杂的射频调制器。

<https://www.linkedin.com/feed/update/urn:li:activity:7251423725034553344/>

![](/picture/Ayarlabs2.jpg)
![](/picture/Ayarlabs3.jpg)
![](/picture/Ayarlabs4.jpg)
![](/picture/Ayarlabs5.jpg)

## 4.13 光学技术：革新带宽密度和能效 示意图

电线提供 10 到 100 Gbps 的带宽，能耗更高 （~10 pJ/bit）。相比之下，光子线（使用单模光纤）实现了 10 到 20 Tbps 的带宽，而消耗的带宽不到 1 pJ/bit。

光学器件通过在更小的物理占用空间内利用多个波长来提供卓越的带宽密度，从而实现更快、更节能的数据传输。

资料来源：Ayar Labs

![](/picture/Ayarlabs6.jpg)

## 4.14 Ayar Labs 与合作伙伴合作解决 HPC 和 AI 系统中的 I/O 瓶颈问题 - SC24

在SC24，Ayar Labs 的业务开发经理 Jeff Demain 和 Corning Optical Communications 的联合封装业务开发总监 Benoit Fleury 演示了概念验证演示，展示了 Ayar Labs 的 TeraPHY 光学 I/O 小芯片与康宁先进的玻璃波导的直接集成。

<https://www.linkedin.com/posts/ayar-labs_sc24-optical-photonics-activity-7272409007011573760-wI0s?utm_source=share&utm_medium=member_desktop>

## 4.15 SC24 演示

Ayar Labs的官网上也有SC24的预告，先翻译一下。他们与富士通有限公司、英特尔、康宁公司、Altera等一起展示其技术在各种人工智能基础设施概念中的应用。

      在Ayar Labs的展位上，将展示一个概念模型，该模型将Ayar Labs的光学I/O解决方案与富士通A64FX处理器集成在PRIMEHPC FX700机箱中，每个CPU集成两个TeraPHY™光学I/O芯片，代表高达16 Tbps的双向带宽。       除了展示的模型外，Ayar Labs和富士通还共同发表题为“满足下一代人工智能/高性能计算系统架构性能和总体拥有成本要求的新型基于光学的扩展结构”的演讲，讨论当前架构中的关键挑战和未来系统的要求，同时Ayar Labs将解释基于光学I/O的扩展结构如何提高这些系统的系统级性能并降低总体拥有成本。       

在SC24上进行的其他演示和展示包括：
- 创新的人工智能系统架构工具：位的参观者可以看到Ayar Labs的光学I/O对扩展大型语言模型（LLM）推理的影响，在未来的GPT模型中，盈利能力可提高多达20倍，交互性可提高3 - 4倍。
- 利用光学FPGA推进人工智能：Ayar Labs、Altera和康宁合作开创了一种新的光学现场可编程门阵列（FPGA）解决方案。这个概念验证通过将Ayar Labs的TeraPHY™光学I/O芯片与康宁的玻璃波导模块集成到Altera的FPGA结构中，提供了4 Tbps的双向I/O数据传输。
- 4 Tbps In-Package 光I/O解决方案：SC24的嘉宾可以体验Ayar Labs由其SuperNova™光源驱动的4 Tbps光学I/O解决方案的现场演示。参观者可以亲眼看到在无需前向纠错（FEC）的情况下，以极低的延迟实现超高效的数据传输。
- 可拆卸光学连接器生态系统：Ayar Labs将重点介绍用于光学I/O的可拆卸光学连接器的最新进展，包括最新的英特尔可拆卸光子玻璃互连和Teramount TeraVERSE®可拆卸连接器。这些连接器使Ayar Labs用于人工智能的封装内光学I/O解决方案能够灵活、高效且具有成本效益地进行部署和维护。       底下就是现场展示的光IO照片了。图中有展示了两个SuperNova光源，Altera FPGA集成TeraPHY光IO chiplet，以及4个光IO，通过Corning的玻璃波导基板形成互连。

![](/picture/Ayarlabs7.jpg)
![](/picture/Ayarlabs8.jpg)
![](/picture/Ayarlabs9.jpg)

连接器方案展示了Intel Foundry和Teramount的两套方案，Intel的方案是Glass interposer，而Teramount是带反射镜硅基板的大容差表面耦合，都是专门给CPO/OIO应用开发的高密连接方案。

![](/picture/Ayarlabs10.jpg)
![](/picture/Ayarlabs11.jpg)

后边就是他们的外置光源展示，第二代SuperNova的光源从第一代的8波长×8光纤升级到了16波长×8光纤的128信道。

![](/picture/Ayarlabs12.jpg)

## 4.16 2024.12.12获得AMD、Intel和Nvidia的1.55亿美元投资

今天，Ayar Labs 宣布已获得 AMD 、Intel Capital 和 英伟达 的 1.55 亿美元投资，以满足对可扩展、经济高效的 AI 基础设施的迫切需求。

Advent Global Opportunities 和 Light Street Capital 引领了 D 轮融资，以加速 Ayar Labs 封装内光学互连产品的大批量生产。

感谢我们所有的投资者和合作伙伴，感谢你们在大规模提供光学 I/O 以满足大规模 AI 工作负载需求方面的支持！

<https://ayarlabs.com/news/ayar-labs-155m-series-d-to-address-ai-infrastructure-includes-amd-intel-capital-nvidia?utm_campaign=241108-series-d&utm_source=linkedin&utm_medium=social>

![](/picture/1733926105037.jpg)

<https://www.linkedin.com/posts/ayar-labs_optical-photonics-semiconductor-activity-7272613202532691968-osUe?utm_source=share&utm_medium=member_desktop>

彭博社采访CEO

Ayar Labs 旨在利用光学创新减少 AI 基础设施瓶颈。首席执行官 Mark Wade 讨论了他们最新的 $155M 融资以及他们如何与 Nvidia、Intel 和 AMD 等合作伙伴合作 

<https://trib.al/nHxUk3O>

<https://www.linkedin.com/posts/bloombergtelevision_ayar-labs-aims-to-reduce-ai-infrastructure-activity-7272700598842535936-GxHI?utm_source=share&utm_medium=member_desktop>

彭博新闻

Nvidia、AMD 和英特尔投资为芯片带来光明的初创公司

- 光学互连设计公司 Ayar Labs 融资 1.55 亿美元
- 这家加州公司的估值目前超过 10 亿美元

Ayar Labs Inc.是一家专门利用光在芯片之间传输数据的公司，随着业界追求更高效的人工智能处理，该公司获得了美国三大半导体设计公司的投资。

这家总部位于加利福尼亚州圣何塞的公司表示，在由 Advent Global Opportunities 和 Light Street Capital 领投的一轮融资中，该公司从Nvidia Corp. 、AMD Ventures 和 Intel Capital 筹集了 1.55 亿美元。联合创始人兼首席执行官马克·韦德 (Mark Wade)告诉彭博新闻社，凭借这笔投资，Ayar Labs 的估值超过了 10 亿美元。

人工智能热潮是一项耗电大、投资昂贵的事业。支持人工智能的技术主要是 Nvidia 图形处理单元，用于同时处理多项任务，这要求服务器系统快速、持续地传输数据。这会产生瓶颈，需要大量电力，并且在运行时会产生大量热量。Ayar Labs 针对这些挑战的解决方案是使用光或光子来加速数据传输。

“人工智能工作负载确实对现有硬件基础设施造成了巨大压力，尤其是在互连方面，”韦德说。“我们已经想出了一种替代这些电气互连的方法。”

几十年来，人们一直使用光来传输数据，例如连接各大洲的海底光缆。Ayar Labs 已将该技术缩小了几个数量级，以将其装入芯片封装中。

韦德表示，客户已经在试用 Ayar Labs 的芯片，他的目标是到 2026 年中期让这些芯片具备大批量生产资格。他说，本轮融资的资金将用于扩大生产规模。

如今，这些芯片由GlobalFoundries Inc.生产，Ayar Labs 还与英特尔公司合作，将其技术整合到这家圣克拉拉公司的制造产品中。Wade 的初创公司还在与行业领导者台湾半导体制造公司洽谈。

VentureTech Alliance与台积电建立了战略合作伙伴关系，是 Ayar Labs 的现有投资者。台积电是今年成立硅光子学行业联盟的多家公司之一，该联盟旨在帮助加速该技术的使用，包括芯片封装。

<https://www.bloomberg.com/news/articles/2024-12-11/nvidia-amd-and-intel-invest-in-startup-bringing-light-to-chips?accessToken=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzb3VyY2UiOiJTdWJzY3JpYmVyR2lmdGVkQXJ0aWNsZSIsImlhdCI6MTczMzkyMTEyMCwiZXhwIjoxNzM0NTI1OTIwLCJhcnRpY2xlSWQiOiJTTzk0S0NUMEcxS1cwMCIsImJjb25uZWN0SWQiOiJBMTkwM0Q0NjcwOTU0MEYwQjA5RjA2NUE3NTk0OTEyQSJ9.AO42H3j_1j1qyMEvnIJzWlLWPnmN6qqDR_NnTPBE5io>

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

## 5.4 2024 Hotchips演讲

<https://events.zoom.us/ejl/Aoq11R4nSJcHRv0c5cDQkB3kzhWGFrJgrvvzDI9aQvc1Itt0s2sU~AxApfK-xtbOe5Mxq-obdLfvfRLEM6Ql-B-U_6qHeAHG2zgV273-oJZy6QJr78kjymBh-T3pMXY7MJXOmpTKs-aSmCf_Wc1i0oCe4/home>

## 5.5 Data goes blue with GaN interconnects - Avicena《Compound Semiconductor》 VOLUME 27 ISSUE IV 2021

MOST OF THE ENERGY consumed in computing systems is not in the computation, but in moving data, and the longer the distance, the greater the challenge in terms of energy and density.  At longer length scales, fibre optic links have replaced copper, but at short distances the significant amount of energy required to convert data back and forth between photons and electrons makes optical interfaces prohibitive.

计算系统中消耗的大部分能量并不在于计算，而是在于数据的传输，而且传输距离越长，能耗和密度的挑战就越大。在较长的距离上，光纤链路已经取代了铜线，但在短距离内，将数据在光子和电子之间相互转换所需的大量能量使得光学接口变得难以实现。

Although it may raise a few eyebrows, at these shorter length scales, optimized optical emitters derived from GaN microLEDs could be a promising candidate for optical communications by leveraging their success in the display industry. Such a move could transform the $400 billion computer hardware industry and enable  entirely new architectures for parallel computing, machine learning, and processors.

尽管这一想法可能引起一些质疑，但在这些较短的距离尺度上，通过利用GaN微型LED在显示行业中的成功，优化的光学发射器可能成为光通信的有力候选者。这样的创新可能会变革价值4,000亿美元的计算机硬件行业，并推动并行计算、机器学习和处理器的新型架构的实现。

Within the semiconductor industry, the days of enjoying rapid rates of progress on multiple fronts are long gone. There has been little increase in chip clock rates during the last two decades. There are also limits on the number of IC package input and output pins. Consequently, almost all high-performance chips utilize high-speed Serializers/De-serializers – known as SerDes – for input/output on the periphery of the die. Their role is to dramatically increase the bit rate compared with on-chip clock speeds so that all the information can be to squeezed through a limited number of pins. This takes energy, real estate, and chokes data flow – and the situation is only going to get worse with future system advances being realised primarily through new architectures that interconnect more chips rather than improvements in raw transistor performance.

在半导体行业，享受多方面快速进步的日子早已一去不复返。过去二十年里，芯片时钟频率几乎没有提升，芯片封装输入输出引脚数量也有限制。因此，几乎所有高性能芯片都在芯片边缘使用高速串行器/解串器（SerDes）进行输入输出。SerDes的作用是显著提升比特率，以便通过有限的引脚传输所有信息。然而，这需要消耗能量、占用芯片面积，并限制数据流动。而随着未来系统的进步主要通过更多芯片的互连而非晶体管性能的提升来实现，这一问题只会更加严重。

Basic physics accounts for the decline in performance of longer electrical interconnects, which are limited by resistance and capacitance of electrical lines. When lines are longer, more capacitance needs to be charged and discharged through their resistance. Increasing density is also problematic – making wires thinner and closer together increases both resistance and capacitance, decreasing maximum interconnect lengths. And that’s by no means the only issue to consider. There’s crosstalk, non-linearities in the dielectric constant of the material causing distortions in the waveform, and the skin effect, which causes an increase in electrical resistance at higher frequencies.  By packaging chips on silicon interposers with a far higher density of lines, electrical data-pipes can be connected to very wide busses and operate close to the clock speed of the chips. However, for reasons 
already outlined, a high density limits the reach, with chips typically having to be placed edge-to-edge. It is common to co-package high-bandwidth memory chips adjacent to the processor (see the leftmost illustration in Figure 1), and communicate over a bus that is typically about 1000 lanes wide, running at only 1 or 2 Gbit/s. Note that Intel’s AIB bus, TSMC’s LIPINCON bus and the Open Compute Project BoW busses are all wide and slow, with hundreds or thousands of lanes, each operating at 1 Gbit/s to 16 Gbit/s.

基本的物理原理解释了较长电气互连性能下降的原因，这主要受限于电线的电阻和电容。当导线变长时，需要通过电阻对更大的电容进行充放电。提高密度同样存在问题——让导线变得更细、更靠近会增加电阻和电容，从而缩短最大互连长度。而这绝不仅仅是需要考虑的问题。还有串扰、材料介电常数的非线性导致的波形失真，以及在更高频率下导致电阻增加的集肤效应等问题。

通过将芯片封装在具有更高线密度的硅中介层上，可以将电信号通过数据通道连接到非常宽的总线，并接近芯片时钟速度运行。然而，由于前面提到的原因，高密度限制了传输距离，芯片通常需要边缘对边缘放置。常见做法是将高带宽存储芯片与处理器并排封装（见图1最左侧的插图），并通过约1000条通道的总线通信，这些总线的运行速度通常仅为1到2 Gbit/s。值得注意的是，英特尔的AIB总线、台积电的LIPINCON总线以及开放计算项目的BoW总线都是宽而慢的，每个通道的运行速度为1 Gbit/s到16 Gbit/s，且总线拥有数百到数千条通道。

**Different optics**
 
 It has been known for decades that even very short optical interconnects promise significant power and density advantages over electrical interconnects. This advantage, based on ‘quantum impedance transformation’, hinges on the use of low-capacitance,  high-quantum-efficiency optoelectronic devices. Unfortunately, despite decades of effort, such sources are still to emerge for short links. Edge-emitting lasers, VCSELs, quantum-well modulators and silicon photonics modulators all fall far short of what is needed for practical short optical interconnects (from 1 mm to 10 m). A litany of issues has prevented success, including a high drive power, large size, poor high-temperature performance, expensive and bulky packaging, and a poor yield.

几十年来，人们已经知道，即使是非常短的光互连也在功耗和密度方面具有显著优势，这种优势源于“量子阻抗变换”，依赖于低电容、高量子效率的光电器件。然而，尽管数十年的努力，适用于短距离互连的理想光源仍未出现。边发射激光器、VCSELs（垂直腔面发射激光器）、量子阱调制器和硅光子调制器等都远未达到实际短距离光互连（1毫米到10米）的要求。阻碍成功的因素多种多样，包括高驱动功耗、体积大、在高温下表现差、昂贵且笨重的封装，以及较低的良率。

These challenges are not insurmountable. What’s needed is a very different approach; our team in Mountain View, California is pioneering a new type of optical emitter derived from high-speed microLEDs. These devices that we call CROMEs (cavity-reinforced optical micro-emitters) utilize very innovative epitaxial and device structures to achieve far shorter carrier lifetimes, and a much higher modulation bandwidth than their more common cousins deployed in ubiquitous lighting and display applications. We have demonstrated CROMEs that are fast enough for current and future high-performance IC interconnects.  


这些挑战并非无法克服。我们需要的是一种截然不同的方法；我们位于加利福尼亚州山景城的团队正在开创一种全新的光发射器，这种发射器源自高速微型LED。我们称之为CROME（腔增强光微发射器）的设备采用了非常创新的外延和器件结构，从而实现了更短的载流子寿命和比常用于照明和显示的传统微型LED更高的调制带宽。我们已经展示了足够快的CROME技术，可以满足当前和未来高性能集成电路互连的需求。

A significant advantage of using visible light is that it allows the fabrication of low-capacitance, large-area CMOS detectors, which can be integrated with simple amplifier circuits to form fast, extremely low power receivers. Thanks to the large area of the detectors, alignment is simple while the packaging cost is low.


使用可见光的一个显著优势在于，它能够制造低电容、大面积的CMOS探测器，这些探测器可以与简单的放大电路集成，形成高速、超低功耗的接收器。由于探测器面积较大，对准变得简单，且封装成本低。

There are several options for moving the light between chips. This can be carried out with monolithically fabricated waveguides on an interposer or with various kinds of multicore and imaging fibres. The use of high density multicore fibres is well established, having been employed for decades in imaging applications, and used in borescopes, medical endoscopy and other ‘display’ applications. Operating in the visible spectrum with optimized CROMEs and CMOS-compatible photodetectors that are integrated with amplifiers, virtually all capacitance is eliminated. We estimate that such links can deliver an energy efficiency below 100 fJ/bit and deliver a multi-Tbit/s throughput at a density in excess of 10 Tbit s-1 mm-2.

在芯片之间传输光信号有多种选择，可以通过在中介层上单片集成的波导来实现，也可以使用多芯光纤和成像光纤等多种方式。高密度多芯光纤技术已经非常成熟，几十年来已被用于成像应用，如内窥镜、医疗内镜和其他“显示”应用。在可见光谱中，使用优化的CROME发射器和与放大器集成的CMOS兼容光电探测器，几乎可以完全消除电容。我们估计这种链路可以实现每比特低于100飞焦耳的能效，并在超过10 Tbit/s mm²的密度下实现多Tbit/s的数据吞吐量。

 A block diagram of our ‘LightBundle’ approach, together with details of a single lane, is shown in Figure 2. Each lane consists of an optical transmitter, a fibre core (or waveguide), and a receiver. The CROME transmitters are powered by simple drive circuitry, driven between 20 μA and 500 μA and optically coupled to a waveguide. Each light emitter has a diameter between 1 μm and 10 μm and may be modulated up to around 10 Gbit/s. The receiver consists of a silicon photodetector, optically coupled to a waveguide and monolithically integrated with CMOS transimpedance and limiting amplifiers. There has already been considerable interest in high-speed visible wavelength LEDs for free-space optical interconnects and ‘LiFi’, where LEDs are used to generate ambient lighting and transmit data. Such LEDs have a range of criteria to fulfil, needing to be both very efficient and fast. But in a chip-to-chip application considerations are markedly different, and one can trade off quantum efficiency for speed. In fact, the benefits of doing so are tremendous. By optimizing the device’s doping, quantum well structure, device design, and other features, CROMEs can be fast enough for very high-density, high performance IC interconnects. We have demonstrated CROME-based links with wide open eyes at even 10 Gbit/s (see Figure 3), a speed previously accessible only with high-speed lasers or modulators.  


图2展示了我们的“LightBundle”方法的框图以及单通道的详细结构。每个通道由一个光发射器、光纤芯（或波导）和接收器组成。CROME发射器由简单的驱动电路供电，工作电流在20 μA到500 μA之间，并与波导进行光耦合。每个光发射器的直径在1 μm到10 μm之间，可调制至约10 Gbit/s。接收器由硅光电探测器组成，光耦合到波导，并与CMOS跨阻放大器和限幅放大器单片集成。

高速可见光LED在自由空间光互连和“LiFi”领域引起了广泛关注，这些应用中LED不仅用于环境照明，还用于数据传输。这类LED需要同时具备高效能和高速度，但在芯片间互连应用中，考虑因素截然不同，可以在量子效率和速度之间做权衡。事实上，这样的优化带来了巨大的好处。通过优化器件的掺杂、量子阱结构、器件设计等特性，CROME可以达到非常高密度和高性能IC互连所需的速度。我们已经展示了基于CROME的链路，在高达10 Gbit/s的速度下依然具有宽眼图（见图3），这是以往仅通过高速激光器或调制器才能实现的速度。

Other factors that increase speed at very low current densities are coulombic enhancement, microcavity effects, and non-radiative recombination. All these help the CROMEs achieve high modulation speeds. Figure 4 shows some CROME experimental results. At very low current densities the 3dB bandwidth reaches about 2 GHz (or around 4 Gbit/s for on-off modulation). Good link performance is realised at drive currents of a few tens of microamps. This allows 
the power consumption per bit to be far lower than  that for lasers. Note that even very small VCSELs, the most energy-efficient lasers, typically have a threshold current of a milliamp. Using blue light for data transmission is incredibly advantageous at the receiver. Silicon is a nearly ideal material for detecting blue light, with an absorption length of just 0.2 μm. This enables CMOS-compatible fabrication of receivers with integrated photodiodes. 
These photodiodes with very low parasitic capacitance (less than 10 fF) allow use of innovative, simplified transimpedance amplifier designs, enabling receiver power dissipation of below 50 fJ/bit. Such a low power is not possible with ‘typical receivers’, which are hampered by a much higher capacitance and greater complexity.

其他在极低电流密度下提升速度的因素包括库仑增强、微腔效应和非辐射复合，这些都帮助CROME实现了高调制速度。图4展示了一些CROME的实验结果。在非常低的电流密度下，3dB带宽可达到约2 GHz（相当于开关键控下约4 Gbit/s）。在驱动电流为几十微安时，链路表现良好。这使得每比特的功耗远低于激光器。即便是能效最高的激光器，如极小型的VCSEL，阈值电流通常也需要毫安级别。

使用蓝光进行数据传输在接收端非常有利。硅是检测蓝光的理想材料，其吸收长度仅为0.2微米。这使得接收器可以采用CMOS兼容的制造工艺，并集成光电二极管。这些光电二极管具有极低的寄生电容（小于10飞法），可以采用创新、简化的跨阻放大器设计，使接收器的功耗低于50飞焦耳/比特。这样的低功耗是典型接收器难以实现的，因为它们受限于更高的电容和更复杂的设计。

 Such a detector structure can be fabricated by using the source and drain implant/diffusions for the CMOS transistors to make lateral p-i-n diodes. Our eight-element array, used for the multi-channel measurements of Figure 4, shows a bandwidth of over 6 GHz (see Figure 5). The shadowing by the fingers on the detector and a thin SOI substrate limited quantum efficiency to about 50 percent, but  quantum efficiencies of more than 90 percent should be achievable in optimized devices.

 这种探测器结构可以通过利用CMOS晶体管的源极和漏极掺杂/扩散来制造横向p-i-n二极管。我们用于图4中的多通道测量的八元素阵列显示了超过6 GHz的带宽（见图5）。由于探测器上的电极遮挡和薄SOI基板，量子效率限制在约50％，但在优化的器件中，量子效率超过90％是可以实现的。

 **Perfecting the package**
 
 We use highly multimode fibres and waveguides to realise efficient optical coupling to the sources and detectors. This relaxes alignment tolerances. One of the merits of this approach is that it allows us to select between a variety of useful packaging architectures, each with a different range of benefits. Our fibre-based links are optimized for longer interconnects, spanning distances from 10 cm to 10 m. These links transfer data between chips and multi-chip modules at the board, shelf and rack levels. Transmitters are connected to receivers using high core-count or imaging fibre (see Figure 6). A typical imaging fibre has hundreds or thousands of cores, each with a diameter ranging from 2 μm to 20 μm. Manufacture involves standard ‘stack and draw’ optical fibre fabrication techniques. Optical channels can be sent through this fiber on a square grid with 20 μm centre-to-centre spacing, with each carrying 4 Gbit/s. This gives an areal interconnect bandwidth density of 10 Tbit s-1 mm-2. Sending 256 of these channels through a fiber provides a total throughput of 1 Tbit/s. As such a fibre is less than 500 μm in diameter, multi-fibre ribbons and cables capable of carrying more than 10 Tbit/s are very compact and flexible. That’s in dramatic contrast to bulky DAC twinax. Since all our processes are fully CMOS compatible, interconnects can also be made directly from the surface of a large complex IC. This direct ‘optical pin-out’ enables ultra-dense, ultra-low-power optical interconnects directly from anywhere on an IC. Operating with an interconnect density of 10 Tbit s-1 mm-2 and an energy per bit of just 100 fJ/bit, these links could provide outputs and inputs for a 100 Tbit/s (bidirectional) switch IC from a 20 mm2 footprint, and a power consumption of just 20 W.  

 我们使用高模态光纤和波导来实现对光源和探测器的高效光耦合，这样可以放宽对准公差。该方法的优点之一是它允许我们在多种有用的封装架构之间进行选择，每种架构都有不同的优点。我们的光纤链接优化用于较长的互连，跨度从10厘米到10米。这些链接用于在板级、架子级和机架级之间传输芯片和多芯片模块的数据。发射器通过高核数或成像光纤与接收器连接（见图6）。典型的成像光纤具有数百到数千个光纤核心，每个核心的直径范围从2微米到20微米。制造过程中使用标准的“堆叠和拉伸”光纤制造技术。光信号可以通过这种光纤在20微米中心间距的方形网格中传输，每条光信号通道的速率为4 Gbit/s。这提供了10 Tbit/s/mm²的面积互连带宽密度。通过光纤传输256条这样的通道可以提供总吞吐量1 Tbit/s。由于光纤的直径小于500微米，多光纤带和电缆能够携带超过10 Tbit/s的数据，非常紧凑且灵活。这与笨重的DAC双轴电缆形成了鲜明的对比。由于我们所有的工艺完全兼容CMOS，互连还可以直接从大型复杂IC的表面制造。这种直接的“光学引脚输出”使得从IC的任何地方实现超密集、超低功耗的光互连成为可能。以10 Tbit/s/mm²的互连密度和每比特仅100飞焦耳的能量，这些链接可以为100 Tbit/s（双向）开关IC提供输入和输出，面积为20 mm²，功耗仅为20瓦。

  For distances of just 1 mm up to 10 cm, data can be routed through lithographically formed waveguides. An array of multimode waveguides, formed from SiO2 , SiN or polymers, can be fabricated on a planar substrate. Deploying these ‘optically-enhanced’ interposers greatly increases practical interconnect distances while decreasing power consumption. The use of lithographic registration enables small sources, which have a typical diameter below 2 μm, to be efficiently coupled into optical waveguides that are only slightly wider than the CROME diameterCompelling credentials

  对于距离仅为1毫米到10厘米的数据传输，可以通过光刻形成的波导来进行。由SiO₂、SiN或聚合物制成的多模波导阵列可以在平面基板上制造。使用这些“光学增强”中介层大大增加了实际的互连距离，同时减少了功耗。光刻注册的使用使得直径通常小于2微米的小型光源能够有效地耦合到仅比CROME直径稍宽的光波导中。

   The strengths of our CROME interconnect technology go well beyond performance. They also fulfil all the other requirements for practical high-volume products: they have a high reliability, they deliver excellent high temperature operation, they are low in cost, easy to package, and they are compatible with existing high volume manufacturing and test capabilities. Our links’ optical interfaces are formed from a variety of technologies that are used in very high volumes in different applications. From a manufacturing perspective, CROME arrays can be thought of as very small GaN microLED displays. As regular readers know, GaN is manufactured in huge volumes for solid state lighting and power devices and is becoming increasingly important for displays. Production of this device is underpinned by a massive ecosystem that supports high volume, low-cost manufacturing. In general, GaN is a far more reliable and robust material system than other III-Vs, such as GaAs and InP, due to its excellent high-temperature performance and insensitivity to defects. Unlike devices made from other III-Vs, those built from GaN can operate at high temperatures, such as 150 °C, with extremely low failure-in-time rates.

   我们的CROME互连技术的优势远超性能层面。它们还满足了高容量产品的所有其他要求：具有高可靠性，优秀的高温操作性能，低成本，易于封装，并且与现有的大规模生产和测试能力兼容。我们的链路光学接口采用了各种在不同应用中以非常高的数量使用的技术。从制造的角度来看，CROME阵列可以视为非常小的GaN微型LED显示器。如常读者所知，GaN用于固态照明和功率器件的生产规模巨大，并且在显示器中越来越重要。该器件的生产得到了支持大规模、低成本制造的大型生态系统的支撑。一般来说，由于GaN具有优良的高温性能和对缺陷的不敏感性，GaN比其他III-V族材料（如GaAs和InP）更为可靠和稳健。与其他III-V族材料制成的器件不同，GaN器件能够在高温（如150°C）下运行，并具有极低的故障率。

  We are able to draw on existing high-volume manufacturing processes used in the lighting and display industries for the mass transfer of thousands to millions of CROMEs from a sapphire source wafer to a target silicon CMOS driver wafer containing transceiver circuitry. Compared to display requirements, the data interconnect is very undemanding: there are fewer than tens of thousands of lanes, and the application is insensitive to colour and brightness variations, both critical concerns for display makers. Another positive for us is that some redundancy can be built in with spare channels, which is also done in wide slow electrical busses. 

  我们能够利用现有的用于照明和显示行业的高容量制造工艺，将成千上万到数百万个CROME从蓝宝石源晶圆转移到包含收发器电路的目标硅CMOS驱动晶圆上。与显示要求相比，数据互连的要求非常宽松：通道数量少于几万，而且应用对颜色和亮度变化不敏感，这对于显示制造商来说是关键问题。另一个积极因素是，我们可以通过备用通道来增加一些冗余，这与宽慢速电气总线中的冗余处理类似。

  Our transceiver circuitry and our photodiodes are manufactured using standard CMOS. We can use older process nodes, thanks to the modest link speeds. For coupling we can use polymer micro optics, similar to those in smartphone cameras.  By leveraging all these high-volume technologies, we estimate that the costs of these Tbit/s wide parallel GaN-based links are one to two orders of magnitude lower than the cost of other high speed serial optical link technologies, such as pluggable optical transceivers, board mounted optics, or even silicon photonics co-packaged optics aimed for datacenter and computing environments. Although our technology is multimode and limited to 10 m reaches, it clearly promises to have an important role to play in advancing the performance of computing systems

  我们的收发器电路和光电二极管使用标准CMOS制造。由于链路速度较低，我们可以使用较旧的工艺节点。对于耦合，我们可以使用类似于智能手机摄像头中使用的聚合物微光学技术。通过利用这些高容量技术，我们估计这些Tbit/s级宽的GaN基链接的成本比其他高速串行光学链接技术（如可插拔光学收发器、板载光学组件或甚至针对数据中心和计算环境的硅光子学集成光学）低一个到两个数量级。尽管我们的技术是多模的，且范围限制在10米以内，但它显然有望在提升计算系统性能方面发挥重要作用。

  **OPPORTUNITIES FOR CROME-BASED LINKS**

  CLOUD-SCALE data centres and high-performance computing are dominated by interconnects. To ease the data bottleneck, a great deal of attention and investment has been directed at the copackaging of silicon photonics with ASICs, GPUs and memory. CROME-based interconnects offer a complementary technology to silicon photonics. While silicon photonics may provide an excellent solution for interconnects longer than 10 m, CROME-based  links offer a far more dense, lower-cost solution at smaller length scales.

  在云规模数据中心和高性能计算领域，互连技术占据主导地位。为了缓解数据瓶颈，很多关注和投资都集中在将硅光子学与ASIC、GPU和内存进行联合封装上。基于CROME的互连提供了硅光子学的互补技术。虽然硅光子学可能为超过10米的互连提供卓越的解决方案，但基于CROME的链路在较短长度尺度上提供了更高密度、成本更低的解决方案。

  CROME-based interconnects could provide welcome solutions to various problems. As switch ASICs in routers and switches move to more than 100 Tbit/s total throughput, CROME-based interconnects could move the data from the switch ASIC to the chassis front plate, where standard ethernet transceivers could be deployed, and down the rack to the NIC cards in the servers. In the move towards disaggregated infrastructure, CROME-based links could provide low latency, low power connections to shared memory or connect processor clusters. These high-density links increase connectivity for both learning and inference in machine-learning and deep neural networks. 


基于CROME的互连可以为各种问题提供令人欢迎的解决方案。随着路由器和交换机中的交换ASIC总吞吐量超过100 Tbit/s，CROME基的互连可以将数据从交换ASIC传输到机箱前面板，在那里可以部署标准以太网收发器，然后向下传输到服务器中的网络接口卡。在向解耦基础设施发展的过程中，CROME基的链路可以提供低延迟、低功耗的连接，以连接共享内存或处理器集群。这些高密度链路增加了机器学习和深度神经网络中学习和推理的连接性。

Looking further ahead, there are opportunities for optical interfaces to be implemented directly on large complex ICs, where they will provide the best power, latency, density, and cost. In decades gone by, the fundamental density and power limitations of electrical interconnects compelled the migration to SerDes-based input/output (I/O) for high-speed interfaces. Now these interfaces consume significant IC power and real-estate, and low power optical interfaces hold much promise. Introducing them could unlock the door to a new generation of ICs incorporating ‘lightweight’ high-performance IOs with greatly improved density, latency, and reach while consuming far less IC real estate and power.


展望未来，光学接口有可能直接集成在大型复杂IC上，这将提供最佳的功耗、延迟、密度和成本。在过去，电气互连的基本密度和功耗限制迫使我们迁移到基于SerDes的高速输入/输出（I/O）接口。如今，这些接口消耗了大量的IC功耗和空间，而低功耗光学接口则充满了潜力。引入光学接口可以开启IC的新一代技术，将“轻量化”的高性能I/O集成在IC中，显著提高密度、降低延迟和扩展范围，同时减少IC占用的空间和功耗。

 In the latter part of the twentieth century, numerous groups in academia and research labs looked to photonics to revolutionize computing, pointing out that optical beams enable very high connectivity. 
 
In this vein, a team at AT&T Bell Laboratories demonstrated simple optical computers using quantum well modulators with gratings and holograms. But despite massive funding and huge interest from DARPA and other resources, the technology never matured – perhaps because the components and the applications needed to make these breakthroughs did not exist. Today that’s not the case. The technology and the need are now both there, and perhaps the dreams of the visionaries can be realized with these new CROME devices.


在二十世纪后期，众多学术和研究实验室的团队希望通过光子学来革新计算，指出光束能够实现非常高的连接性。

在这一背景下，AT&T贝尔实验室的一个团队展示了使用量子阱调制器、光栅和全息图的简单光学计算机。然而，尽管得到了大量资金和来自DARPA等资源的巨大关注，这项技术从未成熟——可能是因为当时所需的组件和应用尚未存在。今天情况不同了。技术和需求现在都已经到位，也许这些新型CROME设备可以实现当年那些先知梦想的愿景。

**Quantum Impedance Transformation解释**

量子阻抗变换（Quantum Impedance Transformation）是一个涉及量子力学和电路理论的概念。简单来说，它描述了在量子系统中，如何通过特定的操作或设备改变量子电路的阻抗特性。为了更好地理解这个概念，可以分几个方面来解释：

阻抗的概念：在电路理论中，阻抗是指电路中对电流的阻碍程度，类似于电阻的概念，但它不仅包括电阻，还包括电容和电感的影响。阻抗的变换通常指通过某些方法改变电路的阻抗特性，以达到特定的功能或效果。

量子系统中的阻抗：在量子系统中，特别是量子电路（如超导量子比特电路）中，阻抗的概念也存在。这些量子电路的行为可以用类似于经典电路中的阻抗概念来描述，但通常涉及到量子态、量子叠加和量子纠缠等现象。

量子阻抗变换的应用：量子阻抗变换可以用于设计和优化量子电路中的元件和连接，确保它们在量子计算和量子信息处理中工作得更加高效。例如，在超导量子计算中，通过适当的阻抗匹配，可以提高量子比特的操作速度和准确性。

总的来说，量子阻抗变换是一个多学科交叉的领域，将量子力学与电路理论结合起来，以解决量子计算和量子通信中遇到的实际问题。

## 5.7 光学芯片互连有望加速计算应用 - Bardia Pezeshki electronicdesign 专访

<https://www.electronicdesign.com/podcasts/inside-electronics/podcast/55140590/electronic-design-optical-chiplet-interconnect-promises-to-accelerate-computing-apps>

## 5.8 专利：使用基于 MicroOLED 的互连系统 SYSTEMS USING MICROLED-BASED INTERCONNECTS

背景：
传统上，IC 是通过印刷电路板 (PCB) 上的走线进行连接的。然而，所需的 IC 封装和粗 PCB 线宽严重限制了 IC 和互连密度。最近，IC 已使用硅和有机中介层进行互连，其中裸 IC 芯片通过细电线连接。这些中介层可实现比 PCB 更高的 IC 和互连密度，但仍然存在重大限制。例如，密集窄线（<1 微米宽）的互连长度通常因欧姆损耗和为较长线的电容充电所需的能量而限制在 <1 厘米。这反过来通常会限制与最近相邻 IC 的连接。此外，即使对于长度只有几毫米的连接，芯片到芯片连接的驱动功率也会变得很大，并根据功耗限制系统。此外，与 IC 可以在三维空间中定位和互连相比，使用平面基板作为中介层会显著限制 IC 密度、互连密度和拓扑以及功耗。

<https://www.freepatentsonline.com/y2024/0302605.html>

论文pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US20240302605A1_SYSTEMS%20USING%20MICROLED-BASED%20INTERCONNECTS.pdf>

## 5.9 高温大带宽蓝色 InGaN/GaN 微型 LED

High Temperature and Large Bandwidth Blue InGaN/GaN Micro-LEDs

摘要

展示了在极高温度下带宽最高的 InGaN/GaN 微发光二极管（290°C 时为 3.2 GHz）。进行了差分载流子寿命分析，以了解复合对调制响应的影响。

<https://opg.optica.org/viewmedia.cfm?uri=OFC-2024-Th3D.6&seq=0>

## 5.10 304 通道 MicroLED CMOS 收发器 IC，总计 1 Tbps，每比特亚皮焦耳容量

304 channel MicroLED based CMOS transceiver IC with aggregate 1 Tbps and sub-pJ per bit capability

数据连接限制了 ML/AI 和 HPC 系统等高级计算应用的性能。它们的能效、密度和成本要求对性能至关重要，并且正在突破铜互连的根本极限。光互连被认为是解决这一瓶颈的潜在解决方案。单模光纤上的硅光子 (SiPh) 链路（通常使用外部 DFB 源）已显示出低功耗结果（~5pJ/bit）[1],[2]。多模光纤中基于 VCSEL 的链路已显示出低至 1pJ/bit 的结果 [3]，通常采用比 SiPh 更简单的封装。这些传统的光链路通常在几个通道上以数十 Gb/s 的速度运行，并且两端都需要 SerDes。

<https://ieeexplore.ieee.org/abstract/document/10527157>

## 5.11 专利：相干光纤束平行光链路  COHERENT FIBER BUNDLE PARALLEL OPTICAL LINKS

发明背景
计算和网络性能需求不断增长。突出的应用包括数据中心服务器、高性能计算集群、人工神经网络和网络交换机。
几十年来，晶体管尺寸的缩小和芯片尺寸的增大推动了集成电路 (IC) 性能和成本的大幅改善，这可以概括为著名的摩尔定律。数十亿个晶体管的数量使得之前分散在多个 IC 上的功能可以整合到单个片上系统 (SoC) 上。
然而，随着边际性能效益的降低、良率的下降和每个晶体管成本的上升，进一步缩小晶体管尺寸所带来的效益正在急剧下降。除了这些限制之外，单个 IC 只能包含有限的功能，而这些功能之所以受到限制，是因为 IC 的工艺无法同时针对不同的功能（例如逻辑、DRAM 和 I/O）进行优化。事实上，将 SoC“分解”成更小的“芯片”有很多好处，包括：每个芯片的工艺都可以根据其功能进行优化，例如逻辑、DRAM、高速 I/O 等；芯片非常适合在多种设计中重复使用；芯片的设计成本较低；由于芯片体积更小，器件更少，因此良率更高。
然而，与 SoC 相比，Chiplet 的一个主要缺点是使用 Chiplet 通常需要更多的芯片间连接。与 SoC 中功能块之间的片上连接相比，芯片间连接通常密度低得多，需要的功率也高得多（例如以每比特能量为单位）。
将光源和探测器耦合到波导（包括光纤）通常占光链路成本的大部分并限制其密度。
发明内容
基于微型 LED (uLED) 光源的光学互连可能提供一种方法来克服部分或全部这些限制。微型 LED 通常可定义为直径小于 100 微米的 LED，在一些实施例中为小于 20 微米，在一些实施例中为小于 4 微米，在一些实施例中为小于 1 微米，并且可以制成直径小于 1 微米的 LED。在一些实施例中，uLED 光源可以支持长度大于 1 米、速率大于 1 Gbps 的光学链路，具有较低的驱动功率和非常高的密度。
由大量紧密封装的光纤组成的相干光纤束 (CFB) 通常用于成像和照明应用。然而，它们的独特性质非常适合克服芯片间互连的短而高度并行的光链路中的成本和密度问题。在一些实施例中，相干光纤束为光发射器和光接收器之间的数据通信提供光链路。在一些实施例中，光发射器包括 LED 作为光源，在一些实施例中，LED 是 uLED。在一些实施例中，光接收器包括光电探测器。在一些实施例中，uLED、相干光纤束和光电探测器位于同一封装内，这被称为多芯片模块。在一些实施例中，多芯片模块包括位于公共基板上的多个半导体芯片。在一些实施例中，光发射器是多个半导体芯片中的第一个芯片。在一些实施例中，光接收器是多个半导体芯片中的第二个芯片。在一些实施例中，光发射器是与多个半导体芯片中的第一个芯片相关联的第一光收发器。在一些实施例中，光接收器是与多个半导体芯片中的第二芯片相关联的第二光收发器。
一些方面提供了用于光发射器和光接收器之间的数据通信的光链路，包括：包括多个光发射器子阵列的光发射器阵列，多个光发射器子阵列中的每个光发射器子阵列包括多个微型LED；由多个子束组成的光纤束，每个子束由多个多模光纤组成，每个光纤包括纤芯，多个子束中的每个子束的纤芯用于接收来自相应的一个光发射器子阵列的光；以及包括多个光接收器子阵列的光接收器阵列，多个光接收器子阵列中的每个光接收器子阵列包括多个光电探测器，多个光接收器子阵列中的每个光接收器子阵列用于接收来自光纤束纤芯的光。
在一些方面，光发射器阵列是与第一半导体芯片相关联的第一光收发器的。在一些方面，光接收器阵列是与第二半导体芯片相关联的第二光收发器的。在一些方面，每个子束内的光纤之间保持一致性。在一些方面，不同子束中的光纤之间不保持一致性。在一些方面，多个子束中的每个子束中的光纤输出的相对位置与每个子束中的光纤输入的相对位置相同。在一些方面，微型 LED 附接到第一基板。在一些方面，微型 LED 附接到还包括微型 LED 驱动电路的 IC。在一些方面，光电探测器安装到第二基板。在一些方面，光电探测器与 IC 上的接收器电路单片集成。在一些方面，来自每个微型 LED 的光仅耦合到单个芯中。在一些方面，每个光电探测器仅接收来自单个芯的光。在一些方面，来自每个微型 LED 的光耦合到多个芯中。在一些方面，多个光电探测器用于接收每个微型 LED 产生的光。一些方面还包括至少一个旋转镜，用于将来自微型 LED 的光导向光纤束的输入端。一些方面还包括每个光发射器子阵列的旋转镜，用于将来自光发射器子阵列的微型 LED 的光导向与光发射器子阵列相关联的子束的输入端。一些方面还包括耦合光发射器阵列和光纤束的输入阵列光耦合组件。在一些方面，输入阵列光耦合组件包括四十五度旋转镜，使得入射到镜子上的光以九十度角反射，第一透镜位于旋转镜和微型 LED 之间，第二透镜位于旋转镜和光纤束之间。
通过阅读本公开内容，可以更全面地理解本发明的这些方面和其他方面。

<https://www.freepatentsonline.com/y2024/0305379.html>

论文pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US20240305379A1_COHERENT%20FIBER%20BUNDLE%20PARALLEL%20OPTICAL%20LINKS.pdf>

## 5.12 专利：使用 microLED 的芯片级光学互连 Chip-scale optical interconnect using microLEDs

发明背景
本申请一般涉及使用光链路进行短距离连接的高速电子封装。

随着时间的推移，光学互连已取代了电气连接。光纤的低光损耗、光的固有高带宽、无干扰以及无寄生电感和电容，这些特性都有利于光调制以进行互连。从长距离开始，随着时间的推移，光学的优势已在较短距离范围内得到证实。如今，几米内的最高速度链路几乎总是光学链路。在过去十年中，数据中心的增长以及用于连接交换机和服务器的光学元件的大规模部署，为光学元件带来了巨大的产量，并导致了制造基础设施的巨大创新和投资，从而降低了光学成本，进一步推动了其部署。

然而，当长度小于一米时，互连仍然是电气的，这会成为性能的障碍。诸如 CPU 和 GPU 之类的集成电路很大，而通过硅片发送数据和时钟信号可能会受到互连金属的 RC 时间常数的限制。将信息从芯片传输到共同封装的内存并连接到外围设备都会消耗大量电力，因为电气互连有损耗，会使信号失真，并且具有需要电力来充电的电容。通常必须使用时钟和数据恢复电路来定期清理信号，这会消耗大量电力。在服务器中，不到 5% 的电力消耗用于门中的实际计算，而超过 95% 的电力消耗用于在 IC 之间、封装外传输数据以及与外围设备通信。

除了电线的 RC 和损耗问题之外，还有一个限制，即这些互连通常局限于二维平面，例如芯片、陶瓷封装、硅中介层或电路板的表面。

随着摩尔定律的放缓，短距离范围内的电气互连问题已成为一个关键障碍。现在，更大的计算能力更多地是通过并行性获得的，这强调了处理器块之间的通信。人工智能电路和图形处理单元的重要性日益增加，但都受到短距离通信障碍的限制。芯片时钟同步困难、内存带宽有限以及访问数据的延迟长，都阻碍了高速计算。

例如，GPU（图形处理单元）和微处理器倾向于高速访问大量内存。可用内存量和从内存访问数据的延迟是电气互连限制带来的严重限制。延迟最低的内存是板载缓存——直接集成到与处理器相同的芯片中。但可以集成的缓存量是有限的。为了访问更多内存，高带宽内存 (HBM) 使用先进的封装技术与处理器一起封装，例如使用硅中介层或硅桥。图1 显示了处理器和内存共同封装的示意图。图1 节目半导体封装 111带有图形处理器单元 (GPU)芯片 113位于半导体封装的中心。HBM 芯片115 a - f位于 GPU 芯片的外围。为了访问更多内存，处理器可以通过较慢的总线（PCIe/CXL/或 GenZ）与较远的内存进行通信。但这当然是以更高的延迟和较慢的传输速率为代价的。

HBM 模块可以实现在内存堆栈 121是 DRAM 堆栈，安装在连接到图形处理器 113通过穿过硅中介层 123两者都位于其上。堆栈可以有 8 层高，并且可能有 128 个通道连接到每个芯片以形成 1024 线宽的总线。传输速率为 0.5 GT/s，未来将增加到 2 GT/s 或更高，从而使每个 HBM 的总传输速率达到 500 Gb/s 到 2 Tb/s。GPU 通常有 4 个这样的 HBM 模块，总传输速率高达 10 Tb/s，总可访问内存约为 150 GB。

当然，处理器之外还有更多的 DDR 内存可用，通常容量约为 256 GB 到 2 TB，传输速率较慢，约为 250 GB/s。使用 PCIe 总线可以访问更大的存储空间，但传输速率较慢，约为每 x16PCIe 64 GB/s。

![image](/picture/memory%20bandwidth.png)

从根本上来说，光学技术渗透到这些较小环节的障碍在于产生光和通过适当的介质传输光。
在传输方面，激光器通常不适合大量用于短距离互连。边缘发射激光器通常相对较大，长度为几百微米。它们通常在与硅不兼容的 III-V 材料上生长，产量远低于硅电子器件。半导体激光器具有高温度敏感性，在处理器 IC 的正常温度下，功率和可靠性会迅速下降。激光器的阈值电流也约为几毫安，这会浪费电力。垂直腔激光器（而不是波导边缘发射激光器）可能被认为更合适，因为它们更小，阈值电流更低，但它们对温度更加敏感。已经研究了使用外部激光器和片上调制器，但波导调制器有损耗，消耗大量电能，并且通常与边缘发射激光器大小相同。垂直腔调制器对温度敏感且难以使用。
最近，硅光子学和 III-V 材料与硅的异质集成推动了光收发器的发展，并有望在缩短光链路距离方面取得突破。然而，硅光子学也有损耗，消耗的功率与 III-V 元件相同。
介质也是一个问题。将光纤耦合到硅芯片以及将横向光波导与同封装激光器和电子设备集成起来既复杂又昂贵。此外，它不会打破平面信号二维限制。使用 VCSEL 或垂直腔调制器，可以在自由空间中、芯片上和芯片外使用光学器件，但讨论过的所有与激光器有关的问题仍然适用。

<https://patents.google.com/patent/US12074192B2/en>

论文pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US12074192_Chip-scale%20optical%20interconnect%20using%20microLEDs.pdf>

## 5.13 专利：带分线的 LED 互连，适用于内存应用 Led interconnect with breakout for memory applications

发明背景

数字 IC 的数据连接有限，如今已成为计算的一个重大瓶颈。在过去的几十年里，数据处理（算术）的速度增长速度远远超过了芯片间、芯片间和电路板间数据传输能力的增长速度。处理器和内存之间的问题尤为严重。尽管光学技术长期以来一直被视为缓解这一瓶颈的潜在解决方案，但几乎所有短距离数据连接仍然是电气连接。

具体而言，在可访问的内存量和从内存传输数据的速度之间存在权衡。驱动因素是内存与逻辑相比密度从根本上较低，以及将内存远离逻辑会导致带宽和延迟损失。

目前，占据市场主导地位的两种内存技术是动态随机存取存储器 (DRAM) 和静态随机存取存储器 (SRAM)。SRAM 的密度较低 (KiB-MiB)，每比特需要 6-10 个晶体管，但延迟非常低，约为 1 纳秒。相比之下，DRAM 的密度高得多 (GiB-TiB)，每个单元只需要一个晶体管，但延迟约为 100 纳秒。DRAM 状态也会衰减，因此读出后必须“刷新”。此外，DRAM 工艺与标准 CMOS 逻辑不兼容，因此两者无法轻易集成到同一芯片中。

不同内存技术在延迟和密度方面的差异推动了“内存层次结构”的发展。处理器中的算术单元必须能够以接近单周期的速度访问某些内存，因此，在芯片上进行计算的位置放置了延迟极低、密度极低的小块 SRAM。这被称为 1 级 (L1) 缓存。密度更高、延迟更高的大块 SRAM 放置在距离算术单元较远的位置，通常由单个芯片上的不同处理单元共享。这些被称为 L2 和 L3 缓存。延迟是由 SRAM 单元和通过 SRAM（逻辑互连）的 RC（电阻电容）延迟共同决定的。处理器的内存控制单元会尝试在需要之前将指令和数据从主内存加载到 L1—L3 缓存中，以避免从主内存进行昂贵的提取。缓存的“命中率”描述了从缓存返回数据的内存请求的比例。

图1 显示了具有不同缓存级别的多核处理器的典型架构。处理器芯片111包括多个处理器核心115 a - n。每个核心包括电路，例如电路 117 一个​第一个处理器核心 115 a，用于执行逻辑和相关功能。每个核心都有自己的 L1 和 L2 缓存，例如分别为119 a 1、a 2和121。三级缓存 123在核心之间共享。L1 通常采用“分割”设计，具有单独的指令缓存119 a 1和数据缓存119 a 2。这提供了更高的带宽，但命中率却降低了。处理器按层次结构在缓存中移动：如果在 L1 缓存中找不到指令或数据，它会搜索 L2 和 L3 缓存。如果在任何缓存中都找不到数据，则处理器将访问主存储器，从而导致数百个时钟周期的延迟。增加缓存大小会增加命中率，但会以更高的延迟为代价，因为更大的缓存除了更长的互连外，还需要更密集和更慢的单元。除了缓存大小之外，还有许多可调参数，例如在缓存和主存储器之间传输的“块”的大小，以及关联性，即在缓存中存储块的方式数量。将单个缓存拆分为多个独立的“切片”以增加带宽也很常见。这种缓存层次结构依赖于局部性假设：在某个时间 t 在某个内存地址 x 访问的数据会增加在时间 t+1 访问 x 附近的概率。如果内存访问存在很强的空间和时间相关性，则缓存大小可以很小，同时保持高命中率。

当代光刻技术只能在处理器芯片上集成约 100 MiB 的 SRAM，不足以满足标准工作负载。一种解决方案是将少量低延迟嵌入式 DRAM (eDRAM) 集成到多芯片模块 (MCM) 上，并将其与处理器集成。然而，最广泛使用的方法将快速片上 SRAM 与大量高延迟离线 SRAM 相结合。芯片 DRAM 113.这种 DRAM 通常距离处理器几厘米，位于可插拔模块上。由于将许多高速通道路由到 CPU 封装的挑战，宽 DRAM 总线通常被序列化为几个非常高速的通道，并在处理器内存控制器中反序列化。此外，处理器和内存之间的较大距离以及封装-PCB 交叉可能需要均衡或前向纠错内存总线，这也会增加功耗和延迟。使用标准 DDR DRAM，数百 GiB 到 TiB 的内存可以集成到单个系统中，但现在延迟为数百纳秒。

通过将 DRAM 芯片堆叠在一起形成高带宽存储器 (HBM)，可以实现延迟降低和带宽提高。然后，将此存储器堆栈与硅中介层上的逻辑一起封装，从而允许密集的电气互连阵列形成宽总线。中介层提供的较短距离和较紧密的互连间距消除了对串行器/反串行器 (SERDES) 的需求，从而将延迟降低至约 100 纳秒并降低功耗。但是 HBM 堆栈难以制造，价格昂贵，并且硅中介层的有限面积限制了可以与逻辑集成的存储器数量。此外，存储器堆栈和处理器的接近会导致存储器温度升高，从而增加 DRAM 单元中的泄漏，从而通过增加刷新频率有效地减慢存储器的速度。

提供更多快速缓存的另一种方法是使用先进的封装将内存堆叠在芯片上。图2 这是 3D 缓存架构图，其中内存堆叠在处理器芯片上。图2 64MB SRAM 芯片 215直接安装在处理器 211，充当所有核心共享的 L3 缓存。处理器可能位于打印电路板 213，与空白瓷砖 217 a,b位于处理器的两侧。由于内存直接位于处理器顶部并通过硅通孔 (TSV) 连接，因此无需将数据跨芯片移动到外围进行输入/输出，访问速度更快。在某些实施例中，这种堆叠可以有效地使 L3 缓存的大小增加三倍，并且由于芯片紧密集成，因此仅会增加 4 个时钟周期的延迟。因此，这种实现方式保留了片上 SRAM 相对于 DRAM 的优势。但是，总 SRAM 面积仍然受到逻辑芯片和封装尺寸的限制，因此这种堆叠架构提供的内存量有限。一种简单的解决方案是使用大型封装和逻辑芯片，为 SRAM 提供较大的面积。然而，这需要跨内存和逻辑芯片的长电互连，这会限制频率并主导功率。 HBM 还可以堆叠在处理器芯片旁边或顶部，并且具有更高密度的优势，但如前所述，HBM 本质上具有更高的延迟，并且在处理器封装的高温环境下存在问题。

其他类型的存储器，例如闪存或硬盘磁存储器，其延迟为微秒到毫秒，但可以存储许多 TiB 的数据。

上述传统缓存层次结构对于典型的通用架构来说效果很好，但在不遵循空间和时间局部性假设的专门任务中却无法发挥作用。批量矩阵乘法就是一个例子，它是神经网络训练和推理的核心部分。在这里，传统缓存系统提供的分层小型非均匀内存集无法有效地捕获矩阵乘法中使用的大量同质权重和中间结果集。高级封装（如上述 3D 缓存架构）可以使缓存大小增加几个数量级，但芯片和封装施加的尺寸和热限制限制了总内存量。替代架构（如具有低延迟的大型同质“暂存器”）将非常有益，但无法轻易在硬件中实现。

<https://patents.google.com/patent/US20240241333A1/en>

专利pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US20240241333A1_Led%20interconnect%20with%20breakout%20for%20memory%20applications.pdf>

## 5.14 专利：增强型 microLED，用于芯片间通信 Enhanced microLEDs for inter-chip communications

发明背景
本发明一般涉及LED，并且更具体地涉及光通信系统中的LED。
由于激光器具有窄线宽、单空间模式输出和高速特性，因此在光通信领域中占主导地位。激光器的窄线宽允许高速信号通过色散介质长距离传输，而不会产生不可补偿的脉冲展宽。长距离光纤链路经常受到色散的限制，因此窄线宽激光器对于长距离光纤链路来说可能是必不可少的。激光器的单空间模式也相对容易耦合到单模光纤中。
激光的受激辐射也可能实现较高的调制速度。使用激光直接调制的光链路可能能够以 25 Gb/s 的速度运行，使用 PAM4 调制则可能能够承载 50 Gb/s 的信息。
然而，使用激光可能会给极短距离的光通信（例如芯片到芯片的通信）带来困难。

<https://patents.google.com/patent/US12034096B2/en>

专利pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US12034096_%E5%A2%9E%E5%BC%BA%E5%9E%8B%20microLED%EF%BC%8C%E7%94%A8%E4%BA%8E%E8%8A%AF%E7%89%87%E9%97%B4%E9%80%9A%E4%BF%A1.pdf>

## 5.15 高温下高速蓝色 InGaN/GaN 微型 LED 的复合率分析 Recombination Rate Analysis of High-Speed Blue InGaN/GaN micro-LEDs at Elevated Temperatures

演示了在高温 (250C) 下具有高带宽 (2.6 GHz) 的 InGaN/GaN 微发光二极管。进行复合率分析以了解辐射和非辐射率对不同温度下调制响应的影响。

<https://opg.optica.org/abstract.cfm?uri=cleo_at-2024-ATu4J.6>

## 5.16 使用基于 MicroLED 的光学链路互连网络 Interconnect networks using microled-based optical links

发明背景

对提高计算和网络性能的需求似乎无处不在且永无止境。突出的应用包括数据中心服务器、高性能计算集群、人工神经网络和网络交换机。

几十年来，晶体管尺寸的缩小和芯片尺寸的增大推动了集成电路 (IC) 性能和成本的大幅改善，这可以概括为著名的摩尔定律。数十亿个晶体管的数量使得之前分散在多个 IC 上的功能可以整合到单个片上系统 (SoC) 上。

然而，随着边际性能优势的下降、产量的下降和每个晶体管成本的增加，进一步缩小晶体管尺寸所带来的好处正在急剧减少。除了这些限制之外，单个 IC 只能包含这么多功能，而这些功能受到限制，因为 IC 的工艺无法同时针对不同的功能（例如逻辑、DRAM 和 I/O）进行优化。

事实上，将 SoC“去集成”为更小的“芯片”有显著的好处，包括：

每个芯片的工艺可以根据其功能进行优化，例如逻辑、DRAM、高速 I/O 等。

芯片非常适合在多种设计中重复使用。

芯片的设计成本较低。

由于芯片尺寸更小且设备数量更少，因此产量更高。

然而，与 SoC 相比，Chiplet 有一个主要缺点：使用 Chiplet 通常需要更多的芯片间连接。与 SoC 中功能块之间的片上连接相比，芯片间连接通常密度低得多，需要的功率也高得多（例如以每比特能量为单位）。

<https://patents.google.com/patent/US20240137132A1/en>

专利pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/US20240137132A1_%E4%BD%BF%E7%94%A8%E5%9F%BA%E4%BA%8E%20MicroLED%20%E7%9A%84%E5%85%89%E5%AD%A6%E9%93%BE%E8%B7%AF%E4%BA%92%E8%BF%9E%E7%BD%91%E7%BB%9C.pdf>

## 5.17 304 通道 MicroLED CMOS 收发器 IC，总计 1 Tbps，每比特亚皮焦耳容量 304 channel MicroLED based CMOS transceiver IC with aggregate 1 Tbps and sub-pJ per bit capability

1Tbps 16nm-CMOS 收发器 IC 配备基于 microLED 阵列的发射器和混合硅探测器阵列，运行速度约为 1pJ/bit，使用 304 个通道，每通道 3.3Gbps。图中显示了单通道和各种配置的初始结果。

数据连接限制了 ML/AI 和 HPC 系统等高级计算应用的性能。它们的能效、密度和成本要求对性能至关重要，并且正在突破铜互连的根本极限。光互连被认为是解决这一瓶颈的潜在解决方案。单模光纤上的硅光子 (SiPh) 链路（通常使用外部 DFB 源）已显示出低功耗结果（~5pJ/bit）[1],[2]。多模光纤中基于 VCSEL 的链路已显示出低至 1pJ/bit 的结果 [3]，通常采用比 SiPh 更简单的封装。这些传统的光链路通常在几个通道上以数十 Gb/s 的速度运行，并且两端都需要 SerDes。

<https://ieeexplore.ieee.org/abstract/document/10527157>

## 5.18 乐高演示 ECOC2024 Bardia Pezeshki - 20240921 Linkedin 

One of the challenges with silicon photonics is the complexity of the fiber attach. Lots of single mode fibers, all of which need to be precisely aligned to sub-micron positions ultimately affects costs and impacts yield. MicroLED based LightBundle, on the other hand, where hundreds of low cost illumination fibers are connected simultaneously with low precision is much easier. To prove the point, at the European Conference on Optical Communications next week, we will be doing a demo with Legos -our standard 1mm diameter 331 fiber cable for 1Tb/s link with a connector assembled using standard Lego pieces! Come see it for yourself and play with Legos in Frankfurt next week.

硅光子学的挑战之一是光纤连接的复杂性。 大量的单模光纤，所有这些光纤都需要精确对准亚微米位置，最终会影响成本和产量。 另一方面，基于 MicroLED 的 LightBundle 可以以低精度同时连接数百根低成本照明光纤，这要容易得多。 为了证明这一点，在下周的欧洲光通信会议上，我们将用乐高积木做一个演示 - 我们的标准 1 毫米直径 331 光纤电缆，用于 1Tb/s 链接，连接器使用标准乐高积木组装！ 下周在法兰克福亲眼看看和乐高积木一起玩吧。

![image](/picture/avicena_lego.jpg)

it's an array of borosilicate illumination fiber, each of which is 50um diameter. Almost all core and of course very multimode. These types of fibers are used for lighting. You may have a bundle in your lab microscope light. For us, we make them ordered so all the channels align simultaneously

它是一系列硼硅酸盐照明光纤，每根光纤的直径为 50 微米。 几乎所有的内核，当然还有非常多模式的。这些类型的纤维用于照明。您的实验室显微镜灯中可能有一束。对我们来说，我们让它们有序，以便所有通道同时对齐

## 5.19 了解基于 microLED 的互连如何释放 HPC 和 AI 的潜力 - Jess Brown 

高性能计算（HPC）、人工智能（AI）和机器学习（ML）对处理能力的需求正以前所未有的速度增长，尽管摩尔定律按最严格的定义已经不再适用，但处理器性能仍在稳定提升，只是速度有所放缓。然而，同样的改进并未出现在芯片间和芯片到存储器的互连技术上，两者之间的需求与现实之间的差距正在不断扩大。Avicena公司商务拓展部的Dr. Jess Brown如是写道。

大型语言模型（LLMs）的增长速度已经完全超越了封装内高带宽存储器（HBM）堆栈的内存带宽增长，如图1所示。实际上，在过去的五年中，LLM的参数量增长了几个数量级，而HBM的内存带宽仅增加了一个数量级。电气互连在传输距离、尺寸和功率效率方面存在基本限制，尤其是在更高的数据速率下，这导致了这种差距。因此，需要低功耗、紧凑、短距离、快速的连接技术，同时保持合理的价格水平。本文深入探讨了基于氮化镓微型LED（GaN µLED）的光学连接技术，这种革命性的方法为芯片间互连提供了前所未有的超低功耗、卓越的带宽密度和极低的延迟，与现有的基于SerDes的解决方案形成了鲜明对比。

![image](/picture/Jess%20Brown%20Fig1.png)

**互连技术：选择方案**

目前有两种主要的互连基础技术：电气互连和光学互连。下图（图2）显示了这两种技术在不同配置下的优值图（Figure-of-Merit，FoM）。FoM将带宽密度与能效的乘积与链路距离（从0.1毫米到1000米）进行对比。在短距离通信（<10厘米）中，电气链路仍然表现出最佳性能，而在长距离通信（>10米）中，传统光学技术表现最佳。但在中等距离范围（1厘米到10米）内，这两者均无法提供最佳性能。现有的多模垂直腔面发射激光器（VCSEL）虽然适用于长达100米的距离，但在较短的光互连中并不理想，主要原因是高密度处理器在高温下运行，而VCSEL对高温的容忍度有限。硅光子（SiPh）是另一种正在开发和评估的光互连技术，然而它最初是为中远距离应用开发的，因此在短距离互连中，SiPh的效率表现较差（>5皮焦/比特）。此外，基于VCSEL和SiPh的链路通常使用串行器/解串器（SerDes）来实现每通道超过100Gbps的高链路带宽，但这增加了显著的功耗开销。

因此，在电气和现有光学解决方案之间目前存在一个空白区域，因为这些技术无法为板载数据传输（通常在1厘米到10米之间）提供最佳解决方案，而这正是大多数芯片间互连的距离范围。Avicena的技术可以填补这一空白，并通过基于光学微型LED（µLED）的互连芯片提供优势，提供超高速、低功耗的互连技术，弥合内部处理性能与芯片间通信之间的差距，支持长达10米的互连距离。

![image](/picture/Jess%20Brown%20Fig2.png)

**是否使用SerDes**

分布式数据处理需要在IC（集成电路）之间进行高速数据传输，不论是处理器之间的通信，还是处理器与内存之间的通信，或者两者皆有。数据传输方式有两种选择：并行通信和串行通信。并行数据传输需要多个IC之间的连接，而串行数据传输仅需一对连接。在芯片内部的通信通常是以并行格式完成的，因此为了实现串行互连，需要一个串行器-解串器（SerDes）功能模块，提供并行到串行和串行到并行的转换，从而实现两块IC之间的串行通信。发射部分是并行到串行的转换器，接收部分是串行到并行的转换器，大多数设备支持全双工操作，即同时双向传输数据。

使用SerDes的原因在于它减少了传输数据所需的数据路径数量（以及相关的连接引脚或电线数量），同时实现了高链路带宽。此外，它还解决了电气并行数据传输中常见的一些问题，比如电磁干扰的敏感性和时钟偏移的可能性。SerDes芯片还可能包含编码器、时钟倍频单元、物理编码子模块、时钟和数据恢复单元、输入和输出缓冲区、前向纠错（FEC）块等组件。

对于长距离光互连，使用基于SerDes的互连具有明显优势，因为它们减少了昂贵的激光发射器数量。然而，在几米范围内连接IC时，使用并行链路有明显优势，因为IC内部通常使用宽而相对较慢的总线，时钟速度为几Gbps。Avicena开发了一种基于微型LED（µLED）的光学解决方案，克服了SerDes的缺点，同时保留了光学技术的所有优势。通过取消SerDes的需求，Avicena的LightBundle™由一个GaN µLED和硅光电二极管（PD）阵列组成，并与收发器ASIC相结合。µLED通过光纤束连接到相应的接收端收发器ASIC上的PD阵列，反之亦然。典型的LightBundle链路有数百个通道，每个通道的传输速度为几Gbps，提供每链路超过1Tbps的总吞吐量。每通道的适中速度与典型的IC时钟速度很好匹配，避免了对SerDes的需求，并实现了每比特小于1pJ的最高效光学链路。

GaN µLED已经用于自由空间的可见光通信（VLC），但其数据速率有限。Avicena开发的µLED能够在超过10Gbps的数据速率下工作。通过这一专利技术，已证明这些µLED不仅能以高速调制，还能实现超过2Tbps/mm的带宽密度，并具有每比特小于1pJ的能效。LightBundle收发器芯片可以与处理器通过硅中介层或有机基板共同封装，或者放置在电路板上，通过PCB走线与处理器IC封装连接。唯一的变化是LightBundle IC和处理器IC之间的电气接口。原则上，LightBundle互连可以支持任何电气接口。LightBundle收发器ASIC会将电气数据格式转换为与光学µLED传输格式相匹配的格式。

并行电气接口最适合与LightBundle芯片的并行光学µLED阵列接口配合使用，因为不需要耗电的SerDes。IC可以将电气通道的速率与每个µLED链路的数据速率匹配，或提供简单的复用/解复用功能，以保持最低的延迟和能耗。一个首选的电气接口是正在获得广泛行业支持的通用芯片接口Express（UCIe），但其他协议如BoW或正在发展的UALink也同样可行。

表1比较了并行、SerDes以及Avicena的µLED光学解决方案的优缺点。可以看出，Avicena的LightBundle解决方案为芯片间通信和互连提供了最佳选择。

![image](/picture/Jess%20Brown%20Fig3.png)

**结论**

由于传统基于SerDes的光互连技术的局限性，高性能计算（HPC）、人工智能（AI）和集成电路（IC）行业一直在不断评估创新的解决方案，以实现高带宽密度、高能效和低延迟的短至中距离（几米范围内）互连。微型LED（µLED）技术以其在高分辨率显示器和照明系统中的应用而闻名，现已展现出在芯片级数据通信领域重新定义格局的潜力。通过将光作为数据传输媒介的固有优势与LED阵列的二维布局相结合，基于µLED的光学链路为实现互连架构中前所未有的性能水平提供了一条革命性的路径。

<https://online.flippingbook.com/view/1043419875/10/>

pdf

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/OC24-Autumn-Flipping-Book_with%20links.pdf>

## 5.20 Avicena 在欧洲光通信会议上展示了基于 microLED 的 LightBundle 技术，覆盖范围达 30 米

德国法兰克福--( BUSINESS WIRE )--总部位于加州桑尼维尔的 Avicena 将在德国法兰克福举行的 ECOC 2024 上展示全球首个基于 microLED 的 30 米链路 ( https://www.ecoc2024.org/ )，该链路的覆盖范围是之前公开演示的三倍。与其他光学互连技术相比，Avicena 的 LightBundle TM基于 microLED 的链路可提供卓越的带宽密度、能源效率、可靠性和成本。现在，凭借 30 米的覆盖范围，LightBundle 互连可以跨越整排数据中心机架，从而释放 HPC 和 AI 集群无与伦比的性能。


**“在 30 米的距离内，这些互连可以轻松覆盖数据中心的一排机架或汽车应用中的商用车（如公交车）的整个长度。通过进一步优化设备和光纤，这项技术可以实现 100 米或更长的覆盖范围。”**

人工智能 (AI) 正在推动对计算和内存性能的需求空前激增。这需要更高的密度、更低的功率、处理器之间以及处理器与内存之间的更长互连。

如今，高速互连技术已形成双寡头垄断：距离最远约 1 米的电气链路占主导地位，而基于激光的光学链路则是更长距离的选择。电气互连既经济高效又可靠，而基于激光的链路成本明显更高，并且可靠性有限。“在 Avicena，我们很高兴展示基于 microLED 的链路，其覆盖范围可达 30 米，此前我们曾公开展示过 10 米链路，”Avicena 创始人兼首席执行官 Bardia Pezeshki 表示。“在 30 米的距离下，这些互连可以轻松覆盖数据中心的一排机架或汽车应用中的商用车（如公交车）的全长。通过进一步优化设备和光纤，这项技术可以实现 100 米或更长的覆盖范围。”

Avicena 首席技术官兼联合创始人 Rob Kalman 表示：“与更传统的光互连技术相比，LightBundle 链路具有更高的密度、功率效率和成本，但传输距离较短。将 LightBundle 的传输距离从 10 米扩展到 30 米开辟了重要的新应用，并表明我们正在继续快速推进这项令人兴奋的新技术。”

Avicena 还将在其展位上展示 LightBundle 技术套件使用标准 LEGO TM组件 大大放宽的对准公差。这强调了这样一个事实：与基于单模的硅光子学的严格公差相比，对准基于 LED 的光学链路确实是“小菜一碟”，从而使 LightBundle 能够实现更低的制造成本和更高的封装可靠性。

<https://www.businesswire.com/news/home/20240922201225/en/Avicena-Demonstrates-30m-Reach-of-microLED-based-LightBundle-Technology-at-European-Conference-on-Optical-Communication>

<https://avicena.tech/avicena-demonstrates-30m-reach-of-microled-based-lightbundle-technology-at-european-conference-on-optical-communications/>

## 5.21 采用光纤的芯片到芯片垂直发射光通信

不同半导体封装中的多芯片模块可以是光学数据通过多芯光纤连接的 LED 和光电探测器耦合。这多芯光纤可以穿过半导体封装中的孔，具有半导体封装中的 LED 和光电探测器阵列，提供和分别接收由在多芯片模块

<https://patents.google.com/patent/US20230412282A1/en>

pdf

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Led%20chip-to-chip%20vertically%20launched%20optical%20communications%20with%20optical%20fiber%20-%20patent.pdf>

## 5.22 Avicena 任命前 Oclaro 首席执行官 Greg Dougherty 为董事会成员

2024 年 10 月 15 日 上午 6:00 东部夏令时间

加州桑尼维尔--( BUSINESS WIRE )--Avicena 是一家提供先进 LED 计算光学互连的供应商，该公司今天宣布任命 Greg Dougherty 为其董事会成员，任命立即生效。Dougherty 先生为董事会带来了卓越的执行领导能力和丰富的光通信行业经验，以及在开发创新光学产品和技术方面强大的运营专业知识。

Avicena 首席执行官 Bardia Pezeshki 表示：“我们很高兴欢迎 Greg 这样有能力的高管加入我们的董事会。随着我们继续将创新的 microLED 光学墨水产品化，Greg 的深厚行业知识和专业知识将发挥巨大作用，无论是作为独立光学器件，还是作为用于计算集群中处理器间和处理器到内存互连的共封装芯片。Greg 的见解和指导对公司和我们的投资者来说都是巨大的财富。”

Dougherty 先生目前担任 Infinera 和 MaxLinear 的董事。他自 2013 年 6 月起担任 Oclaro 的首席执行官，直至 2018 年 12 月该公司被 Lumentum 以 18 亿美元收购。他还自 2009 年 4 月起担任 Oclaro 的董事，直至 2018 年 12 月完成出售。在加入 Oclaro 之前，Dougherty 先生自 2005 年 4 月起担任全球领先的智能光子解决方案提供商 Avanex Corporation 的董事，2009 年 4 月 Avanex 与 Bookham 合并成立 Oclaro。 Dougherty 先生还曾于 2002 年 10 月至 2013 年 8 月担任 Picarro, Inc. 董事，该公司是一家使用激光技术的超灵敏气体光谱设备制造商，并于 2002 年 1 月至 2004 年 4 月担任该公司的临时首席执行官。他还曾于 2004 年 1 月至 2009 年 12 月担任斯坦福罗纳德麦当劳之家董事会成员，并担任湾区许愿基金会董事会成员。在职业生涯早期，Dougherty 先生曾于 1997 年至 2001 年担任 SDL 的首席运营官，后来该公司被 JDS Uniphase Corporation 收购，他一直担任该职位直到 2002 年。1989 年至 1997 年，Dougherty 先生还曾担任朗讯科技微电子公司光电子战略业务部的高管职务。

Dougherty 先生表示：“我很荣幸加入 Avicena 董事会。多年前，我很荣幸与一些团队成员共事，现在我很高兴能够帮助将这项创新的互连技术推向产品阶段，从而解决先进电子产品领域可能最大的瓶颈。”

<https://www.businesswire.com/news/home/20241015390740/en/Avicena-Appoints-Former-Oclaro-CEO-Greg-Dougherty-to-its-Board-of-Directors?utm_campaign=shareaholic&utm_medium=linkedin&utm_source=socialnetwork>

## 5.23 20241023 加利福尼亚州硅谷举行的 PECC 峰会

“LPO 是当今的标准，但当你进入 MicroLED +D2D 时，游戏规则才是真正改变的地方——这是一种 AI 放大技术，”Avicena Tech Chris Pfistner 

![](/picture/Avicena1.gif)

## 5.24 光学互连高带宽存储器架构专利

出版日期：2024 年 10 月 17 日
申请日期：2024 年 4 月 11 日

**发明背景**

高性能 IC 与内存之间的互连带宽有限，对系统处理性能有重大影响。目前，带宽最高的内存互连是高带宽内存 (HBM)。HBM 使用垂直堆叠的内存芯片和硅通孔 (TSV)，在非常有限的互连距离内最大化内存容量。

为了实现这种非常高的带宽、高 IC 海岸线密度和低功耗，大型片上系统 (SoC) 111和 HBM 堆栈113通过多芯片封装内的硅中介层115互连，如图1所示。SoC 内有内存控制器121，用于控制与 HBM 堆栈的通信。SoC 和 HBM 堆栈之间的芯片到芯片 (D2D) 互连由 SoC 和 HBM 堆栈上的物理层设备 (PHY) 119 a、b提供，这些物理层设备通过 1024 位宽的总线连接，该总线的最大长度仅为几毫米。这意味着 SoC 可访问的最大 HBM 内存容量受 SoC 海岸线长度和可堆叠的 HBM 芯片数量的限制。这还要求 HBM 非常靠近热 SoC，由于需要相对较高的刷新频率，这会降低 HBM DRAM 的性能。

实现更长（厘米到米）HBM 互连的能力将带来许多好处，其中可能包括使 SoC 能够访问更多的 HBM 容量、将 HBM​​ 与热 SoC 物理分离（可能允许 HBM 在较低温度下运行，从而提高其性能），并且通过适当的架构，给定的 HBM 堆栈可由多个 SoC 访问。

![](/picture/Avicena_patent3.png)

**详细描述**

![](/picture/Avicena_patent1.png)

图5是根据本发明的方面的包括SoC和电子及光子IC芯片的多芯片封装的半框图。

图5是包括 SoC 和电子和光子 IC 芯片的多芯片封装的半框图。SoC 511和电子和光子 IC 芯片513或光收发器芯片均位于硅中介层515上。硅中介层位于多芯片封装517的封装基板519上。SoC、光收发器芯片和中介层全部容纳在多芯片封装内。电子和光子 IC 芯片513可以如本文所述和/或所示。电子和光子 IC 芯片可以包括例如具有有源层的硅基板，所述有源层具有发射电路和接收电路，以及可能的其他逻辑、MicroLED 和光电探测器，所述光电探测器分别粘合到硅基板并耦合到发射和接收电路。

SoC 通过硅中介层上的电气通路与电子和光子 IC 进行电气数据通信。在一些实施例中，电气通路可以形成总线通路。在一些实施例中，总线可以是 1024 位宽的总线。为此，SoC 和电子和光子 IC 芯片中的每一个可以分别包括用于相互通信的芯片到芯片接口521 a、b。

电子和光子集成电路通过一个或多个光耦合器与多芯片封装外部进行光学通信，例如通过图3的光耦合元件。在一些实施例中，光耦合器包括发射方向光耦合器和接收方向光耦合器。

![](/picture/Avicena_patent2.png)

图6A -D 是根据本发明的方面，具有与高带宽存储器（HBM）通信的光子和电子 IC 的布置的半框图。

图6A - D是光子和电子 IC 与高带宽存储器 (HBM) 通信的布置的半框图。图6A显示了电子和光子 IC 芯片611a和高带宽存储器615，它们位于硅中介层 619 上并通过硅中介层619进行通信，电子和光子 IC 芯片中有一个存储器控制器613。电子光子芯片。

在一些实施例中，第二 MCP 包括通过无源硅中介层上的 D2D 互连连接到 HBM 堆栈的 EPIC，其中 EPIC 包括 HBM 内存控制器 (MC)。在一些实施例中，第二 MCP 包括支持 EPIC 和 HBM 堆栈之间的 D2D 互连的有源硅中介层，其中中介层包括 HBM MC。在一些实施例中，第二 MCP 包括安装有 HBM 堆栈的 EPIC，其中 EPIC 包括 HBM MC。在一些实施例中，第二 MCP 包括安装有 HBM 堆栈的 EPIC，其中 HBM 堆栈的缓冲器芯片包括 HBM MC。

<https://github.com/basteng/Today-I-Learned/blob/main/paper/OPTICALLY%20INTERCONNECTED%20HIGH%20BANDWIDTH%20MEMORY%20ARCHITECTURES.pdf>

网页链接
<https://www.freepatentsonline.com/y2024/0345344.html>

## 5.25 CPO Example - MicroLED Parallel D2D Links

在 2024 年 5 月 IEEE Journal of Solid-State Circuits （JSSC） https://lnkd.in/gsam8vuc 中，Avicena Tech 和 密西根大学 报道了一种电光 32 元件接收器 （RX） 阵列，该阵列集成了兼容 CMOS 的蓝光光电探测器，该阵列专为 420nm 波长的基于 MicroLED 的并行光学 Die-to-Die （话题标签#D2D ） 链路量身定制。采用 0.13μm CMOS SOI 工艺制造，每个 RX 阵列元件占用 50μmx50μm 的面积，功耗为 1mW（1V DC 时），灵敏度为 -19.3dBm，同时实现 10-12 的误码率 （BER） 和 0.5pJ/bit 的能效。

摘录（编辑）：

📝在这项工作中，我们将串行 optical 链路的能效与并行链路的能效进行了比较;在相同的数据吞吐量和 BER 下进行短距离芯片间通信。我们的分析预测，将并行链路与其最快的串行链路进行比较，能效提高 >10 倍是可行的。

📝在这项工作中，我们提出了 2Gbps 集成 RX 的设计，为此进行了跨阻噪声优化，以降低直流功耗和有效面积，而不会实际牺牲信噪比 （SNR） 性能。本文报道了一种新颖的差分数字偏移消除 （DDOC） 设计。

📝GaN MicroLED 的波长在 400-450nm 之间;归类为蓝光。

📝蓝光是并行光链路的良好候选者，因为它使紧凑型 RX 能够与具有低单位面积电容的光电探测器集成，这对 P/I（例如，能源效率）和 S/I（例如，参考输入的 RMS 噪声）有益。

📝最好将光电探测器集成到 CMOS 中，因为这样做有助于最大限度地减少与 ESD 二极管和焊盘相关的电容。它还支持高 话题标签#TIA 增益，同时降低 RX 的输入参考噪声和直流功耗。此外，包装成本降低，密度提高。

📝由于在撰写本文时，32 元件 RX 阵列（采用 X-FAB 130nm CMOS SOI 技术）的光纤测试装置尚未完成，因此我们使用自由空间光学测试装置提供单个 RX 阵列元件的测量结果。

🔍观察：
Parallel 或 Serial ，集成光电探测器或片上激光器，MicroLED 、VCSEL 或 FP、420nm、850nm 或 1310nm、NRZ、PAM 或相干...重要的是，在新AI 时代，无论是短距离 （<10m) interchip communications and short-range (<1km) 话题标签#datacenter interconnects (DCI)—and everything in between—demand continued and accelerated scaling in spectral/bandwidth density and energy efficiency. 

VCSEL: Vertical-Cavity Surface-Emitting Laser
FP: Fabry-Perot (laser)
NRZ: Non-Return-to-Zero
PAM: Pulse Amplitude Modulation

![](/picture/1718755938597.jpg)

 Additional reading:

🏷️Full article: https://lnkd.in/gdn9qgUe 

🏷️O-Band Link: https://lnkd.in/gheaJCis 

🏷️TIA Design: https://lnkd.in/g2m9cxpp 

🏷️CPO (IV): https://lnkd.in/g4TM84Kp 

🏷️CPO (V): https://lnkd.in/gAGh_nwK 

<https://www.linkedin.com/posts/mingliangliu_d2d-optical-cmos-activity-7208984910638796801-pBFZ?utm_source=share&utm_medium=member_desktop>

### 5.25.1 Parallel Versus Serial: Design of an Optical Receiver With Integrated Blue Photodetectors and Digitally Tunable Low-End Cutoff Frequency for MicroLED-Based Parallel Interchip Communication

这篇论文发表于《IEEE固态电路杂志》2024年5月刊，标题为“Parallel Versus Serial: Design of an Optical Receiver With Integrated Blue Photodetectors and Digitally Tunable Low-End Cutoff Frequency for MicroLED-Based Parallel Interchip Communication”，主要研究了基于微LED的并行芯片间通信中光接收机的设计。以下是论文的核心内容总结：

1. **并行与串行光链路能效对比**
    - **去除SerDes和CDR**：多数电气通信系统接口宽且单通道速度低，串行光链路需数据序列化和反序列化，并行链路可避免，且能分摊时钟通道功耗，从而提升能效。
    - **光发射机（TX）能效提升**：并行光链路中，各通道比特率降低，接收机输入参考均方根噪声电流减小，为保持信噪比和误码率，发射功率可降低，使并行TX功耗变为串行的\(1 / \sqrt{N}\)。
    - **光接收机（RX）能效提升**：并行接收机阵列元素带宽要求降低，TIA反馈电阻增大、输入参考均方根噪声电流减小，信号摆幅增大。为达相同信噪比，并行接收机阵列元素光电探测器电流减小，通过计算，并行接收机相比串行在能效上有显著提升，且随着并行通道数\(N\)增加，能效提升明显，但存在上限，超过上限后提升饱和。
2. **并行芯片间通信光接收机设计**
    - **集成蓝光光电探测器**：CMOS工艺集成光电探测器可提高前端TIA增益、降低噪声和功耗、减少封装成本、增加阵列密度。本文设计的光电探测器在420nm波长下响应度为0.17A/W，结电容约10fF（15×15µm尺寸）。
    - **差分平衡并联反馈TIA的跨阻 - 噪声优化**：多数光接收机采用基于逆变器的TIA，但存在电源噪声抑制不足和噪声性能问题。本文采用差分放大器配置反馈，通过分析简化电路模型，得出跨阻传递函数、带宽和噪声等表达式，提出跨阻 - 噪声优化方法，设计TIA时使阻尼系数\(\zeta = 0.71\)，以降低噪声、增强带宽，同时确定了优化的输入电容\(C_{I}\)范围（约\(0.3C_{PD}\)），可降低功耗、提高紧凑性，避免使用多级或伸缩式配置来提升直流增益。
    - **后置放大器（PA）和限幅放大器（LA）**：PA1、PA2和\(G_{m}\)晶体管对用于补偿光电探测器直流电流和放大器失调，\(G_{m}\)级在PA2输出端补偿可降低噪声贡献和对DAC分辨率要求，LA采用五级，总增益约46dB，确保在最差条件下也能达到相同信号摆幅。
    - **差分数字失调消除（DDOC）**：传统模拟失调消除电路中，RC滤波器实现低截止频率需大电容，不切实际。本文提出DDOC，通过\(R_{1}C_{1}\)网络滤波、动态比较器、数字增益控制（DGC）、数字积分器和DAC等实现低至几赫兹的截止频率可调，可提供零低频，通过合理选择DAC位数（5位），在保证性能的同时避免确定性抖动过大和设计复杂度过高，确保了DDOC正确运行。
3. **实验结果**：采用0.13µm XFab CMOS SOI工艺制作了光接收机阵列，对单接收阵列元素测试，在1V电源下功耗1mW，面积50×50µm。测试结果表明，误码率为\(10^{-12}\)时灵敏度为 - 19.3dBm，与其他同类工作相比，该原型在能效和紧凑性方面表现出色，证明其是并行芯片间通信有潜力的光接口。

综上所述，论文通过理论分析对比了并行与串行光链路能效，提出了一种适用于并行芯片间通信的光接收机设计，包括集成蓝光光电探测器、优化TIA、设计相关放大器和DDOC电路等，实验结果验证了设计的有效性和优越性。

## 5.26 High Bandwidth GaN-Based Micro-LEDs at Temperatures up to 400 ◦C

<https://ieeexplore.ieee.org/document/10613856>

### 5.26.1 参考文献16 电注入 III 族氮化物发光二极管中的差异载流子寿命和传输效应

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Differential%20carrier%20lifetime%20and%20transport%20effects%20in%20electrically%20injected%20III-nitride%20light-emitting%20diodes.pdf>

### 5.26.2 参考文献12 III 族氮化物量子异质结构中的载流子动力学和库仑增强捕获

本文详细研究了 III 族氮化物量子阱 (QW) 发光二极管的小信号响应，其中同时测量了电响应和光响应。引入了完整的传输复合模型来解释测量结果。这可以正确评估复合寿命并准确量化 QW 中的热电子载流子逃逸。此外，还确定并量化了一种尚未报告的载流子捕获机制；它随着 QW 中载流子密度的增加而增加，并带有库仑散射过程的特征。

<https://pubs.aip.org/aip/apl/article-abstract/109/3/033504/1078292/Carrier-dynamics-and-Coulomb-enhanced-capture-in?redirectedFrom=fulltext>

## 5.27 Cignal.ai评价Avicena

Avicena ( https://avicena.tech/ ) 正在解决光学互连中的功率瓶颈问题，这一问题可能会阻碍未来 AI 节点的增长。Avicena 建议从收发器转向非常小的 LED，以减少短距离（最长 10 米）互连的功耗。该公司已公开展示了其技术，包括在最近的 OCP 会议上。

随着 AI 节点越来越大，数据中心内的功耗问题日益严重。随着数据中心的功率受限，用于光互连的功率无法用于计算。LPO 和 CPO 等解决方案正在努力解决传统（2 公里至 10 公里）数据中心光缆中的功率问题，而几米的超短距离连接仍在使用低功耗铜线连接。然而，随着芯片间速度的提高，铜线将耗尽带宽。Avicena 看到了一种新型低功耗光连接的机会——大规模并行、基于 LED 的互连。

在 Avicena 互连中，GaN LED 阵列耦合成光纤束，光纤束垂直连接到基板。从定义上讲，LED 是低功率光学器件，但运行速度较低，工作距离也比激光器短。借助 LED 网格，Avicena 可以以低得多的速度运行每个 LED，并实现较高的总互连速度。这样做需要芯片进行变速箱处理（这会增加功率和空间要求），但 Avicena 声称，整体链路的功率将低于其他替代方案。

Avicena 面临的挑战与任何新技术在尝试进入 AI 节点时面临的挑战相同：只要现有方法可行，设计和构建就会发展得太快，以至于无法考虑新方法。这里面有一个先有鸡还是先有蛋的问题。大型制造商不想冒险使用未经证实的非标准技术，但除非有人冒这个险，否则该技术无法大规模验证。Avicena 拥有一批在光学领域有着出色业绩的高管，因此如果有人能找到让该技术被接受的方法，那可能就是这个团队。但 Avicena 的成功取决于那些历史上很少冒战略技术风险的公司。

<https://cignal.ai/2024/10/optical-component-startup-tracker/>

## 5.28 Bardia Pezeshiki - MicroLED阵列有冗余

用于数据传输的大型 microLED 阵列的好处是您可以拥有冗余。 不过我不确定我们需要它。 这是 16nm 硅片上 microLED 的所有 288 个调制数据通道，总带宽约为 1Tb/s。

![](/picture/Avicena2.gif)

领英回复1：我们有一些关于这个主题的论文，并在会议上做了一些演示。 这比基于激光或基于铜的方法低得多，并且可以为每毫米海岸线提供许多 Tb/s。 我们认为它比基于激光的系统成本低得多，也更可靠。 缺点是覆盖率。 与 SM 或 MM 光纤方法不同，我们仅限于 10 米或数十米。 非常适合在机箱内、机架内或几个机架之间 - 但不能跨数据中心！

领英回复2：令人印象深刻的 Bardia！冗余如何运作？1：1 ， 1：N， 自动？
显示器通常具有数百万像素的红色/蓝色/绿色。 我们只有几百零一种颜色。 因此，microLED 阵列的良率对于数据互连来说比显示器应用要容易得多！

领英回复3：非常有趣。频道是否都在 C 波段
嗨，保罗。 这些 microLED 互连的目标是解决芯片到芯片中的 I/O 和 AI/ML 应用中的放大问题。 与普通的激光或铜基解决方案相比，这要低功耗、成本更低且非常可靠。 由于我们不会走很远 （~10m），因此没有理由进行超低损耗。 我们使用廉价的照明光纤束，并在这些 LED 和硅探测器最擅长的地方 - 蓝色运行。 所以大约 430nm。

<https://www.linkedin.com/posts/bardia-pezeshki-b75b2b6_nice-thing-about-large-microled-arrays-for-activity-7260324964929519617-LigY?utm_source=share&utm_medium=member_desktop>

## 5.29 使用基于 LED 的并行性实现快速光学互连 gazettabyte

Avicena Tech 展示了其声称的世界上最小的 1 兆兆位光收发器。该公司将在 3 月份即将在圣地亚哥举行的 OFC 活动上透露更多有关如何推进其光学技术实现量产的信息。

该接口技术采用紧凑型发光二极管 (LED)。该接口使用这些微型 LED 阵列将光垂直发射到多模光纤束中。

去年 11 月，Avicena 在科罗拉多州举行的 Supercomputing 23 展会上展示了其 1 兆兆位每秒 (Tbps) 接口。该接口使用 304 个基于 LED 的光学通道，每个通道传输 3.3 千兆位每秒 (Gbps) 的数据，总带宽为 1 兆兆位。

被称为 LightBundle 的收发器设计由一块小型 16nm CMOS 工艺芯片组成。该芯片尺寸为 3mm x 4 mm，包含电气接口和光学电路。其中包括微型 LED，每个微型 LED 的直径都小于 10 微米，可发出蓝光。

LED 排列成二维阵列，采用倒装芯片的方式粘合到芯片上。光电探测器也排列成阵列，并通过多模光纤连接到 LED。

Avicena 销售和营销副总裁 Christoph Pfistner 表示：“在 Lightbundle 芯片的电气方面，你可以放置任何你想要的接口。”ASIC 使用开放计算项目的 OpenHBI 接口作为电气接口。

选择 OpenHBI 是因为超大规模客户的要求。但 Avicena 计划在未来的设计中使用 UCIe 小芯片接口。

**性能指标**

除了可插拔光学模块、板载光学器件和共封装光学器件之外，MicroLED 还提供了另一类光学接口（见下表）。

Pfistner 强调，microLED 方法是互补的，并不与硅光子学直接竞争。

![](/picture/Image+22-01-2024+at+17.07.jpg)

MicroLED 和多模光纤使接口的覆盖范围更短（最多 10 米），而硅光子接口的覆盖范围更广。因此，MicroLED 技术非常适合芯片到芯片的应用，例如将图形处理器单元 (GPU) 与高带宽内存 (HBM) 连接。MicroLED 技术也有利于机架内链路。

尽管如此，Pfistner 还是热衷于强调该技术的优势。首先，无需外部激光源，并且链路消耗的皮焦耳/比特 (pJ/b) 更少。Avicena 表示，该通道消耗 1pJ/b，并表示其路线图表明接口能耗低于 pJ/b。硅光子接口通常消耗 3-5pJ/b，尽管性能指标还应包括外部激光源。 

与硅光子学一样，基于 LED 的解决方案可以在芯片边缘的一小段距离上传输大量带宽，这被称为“前沿”密度。Pfistner 表示，该公司可以实现超过 10Tbps/mm 的接口密度，而该公司的发展规划可能会达到 25Tbps/mm。

鉴于该技术是多模的，将 LED 光源耦合到光纤束时，公差也较为宽松（只有几微米）。这比单模光纤设计（需要亚微米精度）的公差要宽松得多。更宽松的激光制造公差意味着更低的生产成本。

基于 LED 的接口技术还可在 150°C 以上的温度下运行，远高于传统激光器。Pfistner 表示，与 Fred Kish 的北卡罗来纳州立大学 (NCSU) 团队合作，已演示了高达 290°C 的工作温度。

而且，由于该芯片支持短距离跨度上的不归零 (NRZ) 信令，因此与需要信号处理和纠错方案来关闭链路的光纤接口相比，它具有延迟优势。

**有源光缆**

该公司首次将该技术应用于有源光缆产品。

乍一看，这是违反直觉的：有源光缆使用 50 千兆位或 100 千兆位 PAM4 电气接口，而 Avicena 的技术使用许多电气接口，每个接口的速度都较低，仅为每秒几千兆位。因此，在电缆两端的模块内部，需要一个变速箱芯片将 100Gbps 电信号转换为许多低速电信号，然后通过 LED 链路传输。

在接收端也是如此；许多慢速光信号被恢复并从低速电信号复用为高速 50 千兆位或 100 千兆位 PAM4 电信号。

Avicena 正在与一家芯片合作伙伴合作开发一款 12nm 芯片，该芯片带有一个变速箱模块，与其 LightBundle 芯片 IP 相结合。该设计将实现一条 800 千兆以太网有源光缆，其中芯片和光学器件每端的功耗为 5W。

该设计的成本将低于其他光纤设计，成本上可与 800 千兆位有源电缆相媲美，但传输距离更长。该技术还将扩展到 1.6Tbps 有源光缆。

**高带宽内存**

从长远来看，Avicena 正在关注 HBM 的机会。HBM 使用堆叠的高速内存芯片，多个 HBM 位于处理器 IC 周围。目前，业界正在竞相在 HBM 中堆叠更多数据、为 GPU 等处理器提供整体内存以及提高数据访问速度。

然而，HBM 有几个限制。首先，由于散热问题，只能堆叠一定数量的芯片。堆叠底部的内存芯片必须通过其上方的所有芯片散热，而热 HBM 堆叠需要频繁刷新周期来保留数据，这限制了可用带宽。

HBM 的一个优点是它使用大型总线 - 1024 个电气通道宽，每个通道为 6.4 Gbps（HBM3）。这对于 Avicena 的 microLED 光学接口来说是理想的选择。HBM3E 内存使用更快的 9.6Gbps 接口速度。与此同时，预计几年后推出的 HBM4 旨在将电气总线从 1024 通道扩展到 2048 通道，以保证 GPU 设计能够获得数据。

另一个问题是堆栈相对于大型 ASIC 芯片（例如 GPU）的大小。有限的芯片尺寸意味着只能有这么多的 HBM 围绕 ASIC。由于空间限制，高端 GPU 仅限于六个 HBM，芯片每侧有三个堆栈。

使用光学接口有望实现更大容量、高带宽的内存设计，其中堆栈不必挤在 ASIC 周围。内存可以位于更远的地方，但仍然可以以较低的延迟和能耗进行访问。

因此，ASIC 到 HBM 接口是短距离光互连的重要机遇。此外，Avicena 的两家投资者是领先的内存供应商三星和美光。

Avicena 目前专注于准备客户演示套件并提高产量，然后提高首款产品的产量，这些主题将在 OFC 2024 上讨论。

<https://www.gazettabyte.com/home/2024/1/24/using-led-based-parallelism-for-fast-optical-interconnects.html>

## 5.30 不同的光链路配置 - DR8 为 1.6 TB，使用 224G SerDes - PECC峰会

不同的光链路配置 - DR8 为 1.6 TB，使用 224G SerDes，如 Avicena Tech 在 Optica 和 Advanced Photonics Coalition  的 PECC 峰会上的 Chris Pfistner 所示

![](/picture/Different%20Optical%20Link%20Configurations.jpg)

<https://www.linkedin.com/posts/advanced-photonics-coalition_technology-innovation-photonics-activity-7262531545687564288-oAhw?utm_source=share&utm_medium=member_desktop>

## 5.31 LED同样有调制能力 - PECC峰会

LED（发光二极管）简介 - 取代白炽灯和 CFL 灯 - 与激光器不同 - 但具有调制能力，如 Optica 和 Advanced Photonics Coalition  在 PECC 峰会上 Chris Pfistner Avicena Tech 所

![](/picture/LED_Modulated.jpg)

<https://www.linkedin.com/posts/advanced-photonics-coalition_technology-innovation-future-activity-7262347135835086848-0_p2?utm_source=share&utm_medium=member_desktop>

## 5.32 Avicena 采用uLED做为AI组网的光源

Y10T317 Arista对于AI组网光模块发展观点
提到用铜缆具有很好的可靠性，也有低能耗的特点，只是趋肤效应导致其传输距离有限。

![](/picture/Avicena3.png)

100G/ch的传输速率，经过优化后可传输2m左右，前一阵儿Marvell也发布基于他家3nm的128G的PCI互联，也可以采用铜缆互联。

![](/picture/Avicena4.png)

光模块呢，主要是失效率高，可靠性差一些。Avicena给出一个图，说的硅基量子阱工艺的激光器，老化失效导致性能退化，而采用量子点工艺可以缓解这种失效风险。

![](/picture/Avicena5.png)

当然，Avicena给出上面的曲线，是为了提出他家的方案，也就是除了用量子点来缓解量子阱的可靠性隐患。还可以采用uLEC的发光二极管方案，就不仅仅拘泥于硅基量子阱激光器，还是量子点激光器了。

【2024-11-2】 高速光模块所用激光器的各种分类

Y10T278 华为与UCSB硅基外延生长量子点激光器的对比

Avicena给出上面的曲线是为了提出他家的方案，所以隐藏了一个常用设置，就是量子阱激光器更多的是选择在三五族晶圆衬底上的，而不是硅衬底上。Y10T278，有很多图来描述硅的衬底与InP或GaAs的晶格不适配，导致的可靠性风险。

其实传统量子阱工艺在5000-1000小时的老化数据，很多的。

![](/picture/Avicena6.png)

刚才是插了一句话，现在回到Avicena引出的LED方案，就是用发光二极管替代多模VCSEL，在2-20m的距离占得一个席位。距离再长，uLED就支持不了了，再短一点那还是铜的优势更大。

![](/picture/Avicena7.png)

用GaN做的小型化LED，也就是uLED，相比较传统DFB，具有更小的激活能，以及温度无关的劣化特性。

怎么说呢？激活能小，这是个劣势，性能随时间劣化的很快，但是呢，没有突然失效。

就类似端妃的一格电娘娘，弱，可活的久。且在不同温度下的工作状态，都是一样的弱。

![](/picture/Avicena8.png)

活得久，也是个优势。

![](/picture/Avicena9.png)

现在的uLED的调制速率大约可支持到4Gbps，需要256个uLED才能达到1Tbps的总的传输容量。

![](/picture/Avicena10.png)

最大可支持到10-30m的互联，所以Avicena选择<20m这个赛道。

![](/picture/Avicena11.png)

![](/picture/Avicena12.png)

<https://mp.weixin.qq.com/s/7nTEIRgbs8A2hG-sloBGkg>

## 5.33 SC24上的图片

![](/picture/Avicena13.jpg)
![](/picture/Avicena14.jpg)
![](/picture/Avicena15.jpg)
![](/picture/Avicena16.jpg)
![](/picture/Avicena17.jpg)

Avicena是基于MicroLED发射＋多模光纤＋CMOS Image Sensor接收搞的光互连方案，LED虽然速率不高，但胜在功耗低，可靠性高(-55℃到125℃)，密度大(50um pitch)。他们展出的这款1.6T 互连demo，带宽密度为1Tbps/mm，功耗仅有10W，多模光纤传10m，时延仅有6ns，能效说是＜1pJ/bit。分别展出了与HBM互连和GPU的互连。

<https://mp.weixin.qq.com/s/LqOzHsIZzR7bpzhZlBkaGQ>

## 5.34 LightCounting在Supercompute 24 的亮点中介绍了 Avicena

“Avicena 在 SC23 上展示了基于该公司 microLED 技术的微型 1Tb/s 光收发器芯片。LightBundle ASIC 尺寸为 3mm x 4mm，支持高达 10m 的覆盖范围，非常适合芯片间和机架间通信。基于 LED 的接口可在高达 150OC 的温度下工作。氮化镓 microLED 直接集成到 CMOS IC 上。每个 microLED 阵列通过多芯光纤电缆连接到相应的光电探测器。Avicena ASIC 支持 331 个通道，每个通道为 4Gb/s，总带宽超过 1Tb/s。但是，其下一代设计将支持 1.6Tb/s，也将用于 AOC 产品。ASIC 包括用于光发射器和接收器阵列的电路。

在 SC24 上，Avicena 展示了其技术，包括如何将其 LightBundle ASIC 放置在 GPU 旁边的电路板上以及如何将其作为小芯片嵌入 GPU 的模型，见图 10。Avicena 正在利用其技术开发有源光缆，并希望首先证明其板载光学设计技术，然后再推进到共同封装设计。还展示了 4,000 个 50 微米光纤束，可支持高达 12.8Tb/s 的吞吐量。”

![](/picture/Avicena-Demo_SC24-300x225.jpg)

<https://avicena.tech/portfolio-item/sc24/>

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

## 12.1 MicroLED网 新闻

厦门大学和中国台湾阳明交通大学的研究人员通过将氮化铟镓(InGaN)黄光、红光 Micro LED应用于光通信 (VLC)系统当中，实现了更高的光通信效率。

研究人员表示，与光通信系统中常用的硅基光电二极管相比，氮化铟镓光电二极管具有低噪和高灵敏度的优势。

该研究表明，与之前使用的较短波长Micro LED光电二极管相比，此次研究的红/黄光Micro LED对蓝光拥有更高的响应程度。

据悉，长波长的氮化铟镓Micro LED具有在新型显示和可见光通信领域的应用潜力。在本次研究中，研究团队为光通信应用制造了红光和黄光Micro LED，作为光通信发射器和光电二极管 (PD)，并采用应力调制工程和原子层沉积（ALD）技术来提高传输和检测性能。

实验结果表明，在用作光通信发射器时，红光和黄光Micro LED在2000 A/cm²电流密度下表现出439.7和532.5 MHz的高调制带宽，分别实现1.9和2.4 Gbps的数据速率。当用作光通信光电二极管时，具有高铟成分量子阱的长波长Micro LED表现出更长波长吸收边缘，这有望在滤除荧光成分的同时实现对蓝光更高的响应度。

另外，红光和黄光Micro LED光电二极管的响应光谱与大部分蓝色信号重叠，因此对于450 nm的波长光，红光和黄光Micro LED的响应度分别高达0.208和0.135 A/W，高于现有的氮化铟镓LED光电探测器。

此外，研究团队还表示，基于波长选择性，长波长的Micro LED电二极管可滤除缓慢的荧光发射，从而实现高于硅基探测器数倍的白光调制带宽。（来源：LEDinside）

<https://mp.weixin.qq.com/s/rVoYMnpO0djGfXxH_3z2AA>

## 12.2 厦门大学与国立阳明交通大学及 富士康 （鸿海研究院）- 使用蓝色、绿色和红色 InGaN µLED 进行高速 WDM 可见光通信的实验研究

 微型发光二极管 (µLED) 在显示器和可见光通信 (VLC) 中的应用前景广阔。本研究证实了使用 InGaN 蓝色、绿色和红色 µLED 器件的波分复用 (WDM)-VLC 系统的可行性。由于蓝色和绿色半极化器件中的弱极化电场以及红色器件中的应力优化结构，这些器件表现出显着的色彩稳定性和高调制带宽。聚合数据速率达到 11.14 Gbps。此外，蓝色、绿色和红色 InGaN µLED 表现出宽色域，涵盖 NTSC 的 119.4% 和 Rec. 2020 标准的 89.2%，肯定了蓝色、绿色和红色 InGaN µLED 在全彩色显示器和 WDM-VLC 系统中应用的潜力。

 <https://opg.optica.org/ol/viewmedia.cfm?uri=ol-49-16-4697&seq=0&html=true>

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

## 23.1 Andy Bechtolshelm - 2024 Hotchips：

这是他在2024年8月底Hotchips听说的使用MicroLED的OSPF，而并不是实际应用中使用了MicroLED

![image](/picture/OSFP-MicroLED.png)

视频
<https://www.youtube.com/watch?v=Rnwguy1Af_I>

## 23.2 400G 以太网之路由 Bechtolsheim 的意图铺就

掀起波澜的最佳方式就是引起轰动，而安迪·贝希托尔斯海姆（Andy Bechtolsheim）或许是 IT 基础设施领域最著名的连续创业者，他在这方面就非常擅长。作为 Sun Microsystems 和一系列网络和系统初创公司的联合创始人之一，以及谷歌的第一位投资者，他不仅看到浪潮，而且制造浪潮，然后乘风破浪，一路创建公司和市场。

当时，贝克托尔斯海姆还是斯坦福大学的一名博士生，正在从事一个旨在将网络接口与处理器集成在一起的项目。斯科特·麦克尼利和维诺德·科斯拉邀请贝克托尔斯海姆担任 Sun Microsystems 的第一任首席技术官。Sun 从工作站转向系统，取得了巨大的成功。1995 年，贝克托尔斯海姆带着大量资金离开，创办了一家名为 Granite Systems 的公司，专门生产更便宜的千兆以太网交换机。在成立仅仅一年多一点的时间后，贝克托尔斯海姆将公司出售给了以太网路由巨头思科系统，思科系统凭借其 Catalyst 4000 系列铁板产品，在以太网交换领域奠定了基础。

五年后，随着互联网泡沫的破灭，贝克托尔斯海姆再次回到网络系统接口问题上，并成立了一家名为 Kealia 的公司，该公司生产巨型 InfiniBand 模块化交换机和一系列基于 Opteron 的服务器，这些服务器的设计理念是超级计算机，但针对的是企业。到 2004 年，Sun Microsystems 在服务器领域的日子并不好过，它收购了 Kealia，并让贝克托尔斯海姆重返公司，这些系统的基本架构至今仍存在于 Sun 产品线中，尤其是 Exadata 数据库集群。

解决了这个问题后，贝希托尔斯海姆转向了网络领域的下一个浪潮——10 Gb/秒以太网，他与斯坦福大学教授戴维·切瑞顿共同创立了 Arista Networks。切瑞顿领导着分布式系统小组，是 Granite Systems 的联合创始人，也是 Google 的早期投资者。（谢尔盖·布林和拉里·佩奇是切瑞顿的学生，当贝希托尔斯海姆在切瑞顿家门廊上掏出一张 10 万美元的支票给他们俩创办搜索引擎公司时，切瑞顿随后又拿出了一张 20 万美元的支票。）切瑞顿的另一名学生肯·杜达是 Arista Networks 的联合创始人， 2008 年，当贝希托尔斯海姆不再在 Sun 工作，并承认自己大部分时间都在一家新公司工作时，Arista Networks也退出了低调模式。一年半后，Arista Networks 推出了其首款模块化交换机，该交换机配备 384 个 10 Gb/秒端口以及其上的 Linux 可扩展操作系统 (EOS) 变体，并于 2011 年 3 月推出了基于 Broadcom 的 Trident+ 和 Fulcrum Microsystems 的 Bali 交换机 ASIC 的架顶式交换机。

在谈到 100 Gb/秒以太网及其后续产品时，Bechtolsheim 表示：“从收入增长来看，这无疑是有史以来增长最快的以太网标准。400 Gb/秒以太网将在 2018 年底推出，并在 2019 年至 2020 年逐步普及。它的发展速度不会快于 100 Gb/秒以太网，因为它更昂贵。因此，100 Gb/秒以太网将继续大批量出货，也许会在 2021 年实现普及。”

对于超大规模和云构建者来说，重要的是 400 Gb/秒将直接进入数据中心中当前使用 100 Gb/秒的相同位置，而无需更改机架内、跨行、跨数据中心、跨地区和跨地域当前使用的铜缆和光纤线路 - 这正是微软研究人员所预测的必要条件，当时每个人都在 2013 年在 IEEE 上讨论 400 Gb/秒以太网标准的需求。当时，25G 联盟距离推出还有一年的时间，因此我们将获得的 400 Gb/秒在某些方面与我们在没有超大规模压力的情况下获得的有所不同。

我们注意到，Bechtolsheim 对 200 Gb/秒网络没有太多评论，他更专注于直接跃升至 400 Gb/秒。这恰恰是博通 (Broadcom) 对其“Tomahawk-3”芯片组所做的事情，我们一个月前曾谈到过这一点，这绝非巧合。借助 Tomhawk-3，博通将从使用非零返回 (NRZ) 信令组合四个 25 Gb/秒通道的端口转变为使用四通道脉冲幅度调制 (PAM-4) 信令以 50 Gb/秒运行的八个端口。这一切都很好，除了一件事。Bechtolsheim — — 我们推测至少部分超大规模提供商和云构建者 — — 希望直接转向 100 Gb/秒信令，并减少通道数、散热和成本。 （如果你能想象那个怪物的话，IEEE 400 Gb/秒的规范最初是 16 条通道，以 25 Gb/秒的速度运行。）

Bechtolsheim 在演讲中表示：“唯一真正有意义的做法是直接实现每通道 100 Gb/秒的速度”，并指出，随着超大规模和云构建者的需求，带宽跳跃变得越来越大、越来越快，交换机 ASIC 中每个 SERDES 速度的有效寿命越来越短。

![image](/picture/arista-ethernet-lane-speeds.jpg)

事实上，Bechtolsheim 预测，400 Gb/秒设备中的大多数端口将基于 100 Gb/秒信令，而不是当前的 50 Gb/秒信令，因此我们几乎可以猜测出博通的“Tomahawk-4”芯片可能是什么样子以及何时上市。

其中一些转变耗时很长，从 NRZ 到 PAM-4 信号的转变只是其中之一。“问题在于经济因素，”Bechtolsheim 解释道。“人们迅速转向更便宜、更耗电的产品。我们在从 10 Gb/秒到 25 Gb/秒以及从 40 Gb/秒到 100 Gb/秒的转变中看到了这一点，在不到一年的时间里——大概在六个月到九个月之间——我们的大部分订单都转向了新一代产品，该产品在各个指标上都更胜一筹。”事实上，他补充说，客户接受产品的速度和 Arista Networks 生产产品的速度一样快。

这与以太网交换机市场在其存在后的头几十年所展现出的缓慢、可预测和有条不紊的发展方式截然不同。好消息是，每个 IT 组织都将受益于超大规模企业和云构建者通过 Bechtolsheim 等杰出人物向交换机芯片制造商和制造光互连和电线的下游参与者施加的压力。

最后一点：Bechtolsheim 表示，<font color=red>让 SERDES 的速度超过 100 Gb/秒非常困难</font>。这种快速切换本身就是一种障碍。那么，我们该怎么做才能加快速度呢？提高脉冲幅度调制。通过转向 PAM-8 信号，您可以在四条通道上以 100 Gb/秒的速度将每端口速度翻倍至 800 Gb/秒，而使用 PAM-16 信号，您可以获得高达 1.6 Tb/秒的速度。如果您必须以 100 Gb/秒的速度运行八条通道——虽然没有人认为这是可取的，但这可能是必要的——那么根据我们的估计，这将使您的速度达到 3.2 Tb/秒。这可能是使用这些方法的极限，就像在 300 毫米晶圆上的 3 纳米极紫外 (EUV) 工艺上塞入 48 个到 64 个核心的东西可能是使用近乎当前的芯片制造方法的摩尔定律的实际极限。

和往常一样，十年后一切看起来都会走向衰败。这正是 IT 行业令人兴奋的地方。

<https://www.nextplatform.com/2018/02/21/road-400g-ethernet-paved-bechtolsheims-intentions/>

## 23.3 Andreas “Andy” Bechtolsheim ECOC 2024 演讲

ECOC 2024介绍

Arista Networks 联合创始人兼首席架构师

此前，Andy 是 Sun Microsystems 的联合创始人兼首席系统架构师，负责下一代服务器、存储和网络架构。

作为一名私人风险投资人，安迪参与了包括谷歌、VMware、Mellanox 和 Brocade 在内的多家公司的融资。他曾担任超过 25 家公司的董事会成员，其中大多数公司已上市或被收购。

安迪于 1976 年获得卡内基梅隆大学计算机工程硕士学位，并于 1977 年至 1982 年在斯坦福大学攻读计算机工程博士学位。

他曾获得富布赖特奖学金、Studienstiftung 奖学金、斯坦福年度企业家公司奖、史密森尼创新领导奖，并且是美国国家工程院院士。

互连能否跟上人工智能的步伐？
Can Interconnects Keep Up with AI?
AI 集群的带宽需求对 AI Fabric 互连提出了前所未有的挑战。我将讨论如何改善光学器件的功率、成本和可靠性、铜线和光学器件之间的界限以及封装创新的机会。

<https://www.ecoc2024.org/programme/plenary-speakers/>

## 23.4 20241023 加利福尼亚州硅谷举行的 PECC 峰会

“电力仍然是一个问题”

![](/picture/Arista1.gif)

硅控和光学现状

![](/picture/Arista2.gif)

总结幻灯片

![](/picture/Arista3.gif)

## 23.5 OCP

Sustainable Optics for Scaling AI

![](/picture/Arista-OCP2024_1.png)

![](/picture/Arista-OCP2024_2.png)

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/Sustainable%20Optics%20for%20Scaling%20AI.pdf>

<https://www.opencompute.org/events/past-events/2024-ocp-global-summit>

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

# 27. 复旦 迟楠

## 27.1 硅基氮化镓微型LED，实现高速可见光通信信号探测

第三代半导体氮化镓作为一种宽禁带体材料，其细窄的耗尽区能够实现高载流子浓度，以此诞生的发光二极管（LED）获得了2014年诺贝尔物理学奖。借助LED发展起来的可见光通信，正由于频谱无需授权、高速、节能、无电磁辐射等优点，在6G研究领域成为一种极具潜力的通信技术。

但是，可见光通信作为一种通信系统，发射和接收两端具有相同的重要性。近年来，可见光通信的发展主要依靠着发射器件的突破，包括LED、SLD和LD。而对于接收器件，大部分可见光通信系统在使用红外、近红外的探测器进行信号的接收。这些使用的探测器已经在几十年的发展历程中对红外、近红外通信进行了不断优化，这其中包括铟镓砷探测器、镓砷探测器和硅探测器。它们最小的峰值频率响应也在800 nm波长，然后在可见光波段（400-780 nm）快速下降，这就导致类似可见光通信极具竞争力的水下通信场景（蓝绿光400-570 nm）发展受阻。

将氮化镓LED进行反向偏压能实现可见光波段探测器的功能。传统氮化镓LED在制备过程中往往使用蓝宝石衬底或者氮化镓衬底。蓝宝石衬底一般只能设计横向结构，在高注入电流或者高入射光功率下，会表现出电流拥堵、散热差等问题，以至于芯片性能严重下降或损坏。氮化镓衬底是理论上最理想的衬底，可制备氮化镓衬底过程困难且成本极高，难以满足商用化需求。

为解决上述问题，复旦大学迟楠教授、沈超教授、施剑阳博士研究团队联合南昌大学、国家硅基LED工程技术研究中心江风益院士、张建立教授等人设计了一种硅基垂直结构的氮化镓Micro-LED。将该LED作为探测器，成功实现了10 Gbps的可见光通信。相关研究成果发表于Photonics Research 2022年第10期。

该方案首先设计一个硅基垂直结构的氮化镓Micro-LED图（a），实验中同时设计了10 μm×10 μm、50 μm×50 μm和100 μm×100 μm三个尺寸芯片，其中50 μm的SEM图，如图（b）。随后将设计的芯片以共阴极的方式组成4×4芯片阵列，如图（c），该芯片阵列的光纤显微图像，如图（d）。

![image](/picture/Chinan1.webp)

基于该硅基氮化镓Micro-LED，成功实现了实现峰值频率响应400 nm的可见光探测器，其半波宽达到了72 nm，为可见光的波分复用系统提供了可能。对该器件给予正向偏置电压，可以发射出573 nm左右的可见光，当给予方向偏置电压，该器件可以实现可见光信号的探测。通过加大反向偏置电压，-20 dB带宽最大可以达到822 MHz。利用该探测器，成功实现了传输距离1 m，传输速率10.14 Gbps的可见光通信。

相比于传统蓝宝石衬底的氮化镓Micro-LED，硅衬底的Micro-LED具有高晶体质量、良好导电性和高导热性能等特点，并且与现有硅基基础电路兼容，具备向更加小型化高集成化发展的优势，以此构建的可见光探测器，适合未来对成本、速率敏感的6G可见光通信应用场景。复旦大学与南昌大学团队实现了硅基氮化镓Micro-LED作为高速可见光探测器，后续将进一步开展更高响应灵敏度、更高传输带宽的研究，将该器件推向实用化，最终实现可见光通信收发一体化设计与应用。

<https://mp.weixin.qq.com/s/RO7P-60JWRLwjvJDx2nEgg>

用于超过 10 Gbps 可见光通信的 Si 基板垂直结构 InGaN/GaN 微型 LED 光电探测器

几十年来，光电探测器已针对近红外光谱范围内的光纤通信进行了优化，范围从 O 波段 (1260 nm - 1360 nm) 到 U 波段 (1625-1675 nm)。许多可见光通信 (VLC) 系统和演示都基于这些设备，导致系统性能欠佳。为了改进 VLC 系统，必须开发响应度峰值在 400 nm 左右的新型探测器。本文报告了基于氮化镓 (GaN) 技术的此类设备。

我们知道，如果发光二极管 (LED) 受到负偏压，它们可以用作光电探测器 [S. Schmid、G. Corbellini、S. Mangold 和 TR Gross，“基于软件同步的 LED-LED 可见光通信系统”，2012 IEEE Globecom 研讨会，2012 年，第 1264-1268 页，doi：10.1109/GLOCOMW.2012.6477763]。本文基于这一原理，报道了一种用作光电探测器的新型 GaN 微型 LED。与许多在蓝宝石衬底上生长的微型 LED 不同，出于成本和热管理原因，这种新设备使用硅衬底。结果表明，新设备确实在 400 nm 左右表现出峰值响应度，最大 20 dB 带宽约为 800 MHz。使用正交频分复用 (OFDM) 标准做法以及比特和功率加载，边长为 50 毫米的方形设备在 1 米距离处实现了 10.14 Gbps 的惊人数据速率。要实现 10 Gbps，需要 60 mW 的入射功率。未来的工作必须集中于将灵敏度提高三到四个数量级，以便能够在实际 VLC 系统中使用此类设备。

<https://opg.optica.org/spotlight/summary.cfm?id=507603>

用于超过 10 Gbps 可见光通信的 Si 基板垂直结构 InGaN/GaN 微型 LED 光电探测器

<https://opg.optica.org/ViewMedia.cfm?uri=prj-10-10-2394&seq=0&html=true>

论文pdf

<https://github.com/basteng/Today-I-Learned/blob/main/paper/%E7%94%A8%E4%BA%8E%E8%B6%85%E8%BF%87%2010%20Gbps%20%E5%8F%AF%E8%A7%81%E5%85%89%E9%80%9A%E4%BF%A1%E7%9A%84%20Si%20%E5%9F%BA%E6%9D%BF%E5%9E%82%E7%9B%B4%E7%BB%93%E6%9E%84%20InGaNGaN%20%E5%BE%AE%E5%9E%8B%20LED%20%E5%85%89%E7%94%B5%E6%8E%A2%E6%B5%8B%E5%99%A8.pdf>

### 27.1.1 实验装置

![image](/picture/getimagev2.jpg)

上图是采用基于微型 LED 的 PD 的 1 m VLC 系统的实验装置。

发送端

- 传输的 DMT 信号由离线 MATLAB 程序和 AWG（Agilent M8190A）生成。在整个实验过程中，AWG 的采样率设置为 4.8 至 8.2 GSa/s。
- 采用 2.5 GHz EA（Mini-Circuits ZFL-2500VH+）和 4.2 GHz 偏置器（Mini-Circuits ZFBT-4R2GW-FT+）放大信号并驱动 450 nm LD（OSRAM PL450B）。
- LD 安装在紧凑的光学平台上，可配置为三色 LD 。在整个实验中，我们传输了 0.5 和 1 m 的自由空间。

接收端

- 在接收器端，使用可调中性密度 (ND，大恒光学 GCO-0702M) 滤光片来控制入射到 PD 中的光功率。
- 使用镜头 (Olympus PLN10X/0.25) 来促进光信号耦合到微型 LED 中。基于微型 LED 的 PD 由恒流源 (Keithley 2400) 和 4.2 GHz 偏置器提供的反向偏置电压驱动。
- 输出信号再次由 2.5 GHz EA 放大，然后由示波器 (OSC，Agilent MSO9254A) 采样。OSC 的采样率设置为 5 GSa/s。

## 27.2 基于单个磷光白色 LED 的自适应比特分配 OFDM 的 2.0-Gb/s 可见光链路

本文介绍了一种基于单个商用磷光白色发光二极管 (LED) 的高速可见光通信 (VLC) 系统。该系统使用预均衡电路来扩展调制带宽，并使用差分输出接收器来降低系统噪声。通过自适应比特和功率分配以及正交频分复用 (OFDM)，我们通过实验证明了 1.5 米自由空间传输中 2.0 Gb/s 的可见光链路，BER 低于 3.8×10 -3的预前向纠错限制 。据我们所知，这是使用单个磷光白色 LED 的最高白光 VLC 数据速率。

本文介绍了一种基于单个商用磷光白色 LED 的高速 VLC 系统。在该 VLC 系统中，预均衡电路用于扩展调制带宽，并利用低成本差分输出 PIN 接收器来降低系统噪声。使用自适应比特和功率分配 OFDM，我们成功演示了 1.5 米自由空间传输中的 2.0 Gb/s VLC 链路和 3.0 米传输中的 0.79 Gb/s 数据速率，在预 FEC 限制下的 BER 结果为 3.8 ×10− 3。与我们在[18]和 [19]中所做的工作相比 ，我们分别用磷光白光LED和更宽带宽的PIN接收器替换RGB LED的红色芯片和APD接收器。利用自适应比特和功率分配OFDM，与 [20]中所做的工作相比，数据速率大大提高，传输距离也有所增加。据我们所知，这是迄今为止使用单个磷光白光LED报道的最高的白光VLC数据速率。

图 1 给出了 VLC 系统中使用的幅度均衡器的示意图。幅度均衡器的详细原理见 [19]。Z11 是电阻 R1、电容 C1 和电感 L1 的等效阻抗，Z22 是电阻 R4、电容 C2 和电感 L2 的等效阻抗。R2 和 R3 均等于 RL。均衡器的频率响应 Heq 可以表示为

\[
H_{eq} = \frac{1}{2\left(1 + \frac{R_L}{R_4 + \frac{j\omega L_1}{1 - \omega^2 C_1 L_1}}\right)}
\]

当任意波形发生器（AWG）的输出阻抗ZS和电放大器（EA）的阻抗ZL均等于RL，且L1=L2，C1=C2时，电阻R1和R4的关系为R1∗R4=RL2，参数ω为角频率，等于2π∗f，其中f为频率。

![image](/picture/huang1-2480541-large.gif)

式中，当1−ω2C1L1趋于零时，Heq的最大限度为0.5，当f=1/2πC1L1−−−−√时，Heq取最大值；当ω趋于零，且RL一定时，Heq=1/2(1+RL/R4)，低频响应由R1或R4决定。

**幅度均衡器的详细原理见27.3**

<https://ieeexplore.ieee.org/document/7273821>

原文pdf
<https://github.com/basteng/Today-I-Learned/blob/main/paper/2.0-Gb_s_Visible_Light_Link_Based_on_Adaptive_Bit_Allocation_OFDM_of_a_Single_Phosphorescent_White_LED.pdf>

## 27.3 采用硬件预均衡电路的 Gb/s VLC 传输

在本文中，我们提出了一种用于高速可见光通信 (VLC) 系统的恒电阻对称桥式 T 型幅度均衡器。利用该硬件均衡器，我们成功地演示了基于 RGB LED 在 80 厘米自由空间中实现每秒千兆比特的 VLC 传输。在 1.05 Gb/s 的 64 二次幅度调制 (64QAM) 单载波调制、1.05 Gb/s 的 64QAM 正交频分复用 (OFDM) 以及 1.42 Gb/s 的比特和功率加载 OFDM 调制下测量的信号的比特误码率 (BER) 均低于 7% 前向纠错 (pre-FEC) 限制 3.8 × 10 -3 ，清楚地验证了所提出的均衡器的可行性。与不使用均衡器的系统相比，VLC 系统的 BER 性能可以至少提高 1 个数量级。此外，由于均衡器体积小巧，只需使用无源元件即可轻松安装，因此可以轻松集成到放大器或 LED 中。据我们所知，这是使用预均衡电路的最高数据速率和最长传输距离。

<https://ieeexplore.ieee.org/document/7124419>

## 27.4 利用 GaN 激光器实​​现无处不在的通信 - Compound Semiconductor

虽然科幻小说往往无法描述当前的技术能力，但它仍能让我们一窥未来的潜在进步。一个典型的例子就是漫威漫画的英雄钢铁侠，他的防弹衣自 1962 年首次亮相以来就不断演变。在最近的迭代中，托尼·斯塔克的战衣采用了可以相互通信的纳米级设备。要让科幻小说成为科学事实，这样的防弹衣需要强大的高速数据传输能力。

虽然我们不太可能完全模仿钢铁侠，但随着 6G 无线数据链路技术的快速发展，人们正在转向更多可穿戴设备。在这个基础设施中，可见光通信 (VLC) 有望发挥关键作用。VLC 有望以超高速度和低延迟提供跨太空-空中-地面-水下领域的广泛覆盖通信。未来，光甚至可以用来为 X-things 互联网供电。

什么是 VLC？
“可见光通信”一词相对不言自明。它是一种无线光传输技术，利用可见光在380 nm 至 790 nm 光谱范围内进行数据通信。

与传统无线通信难以应对光谱资源的匮乏形成鲜明对比的是，可见光通信拥有丰富的光谱资源，带宽约为 400 THz。这一巨大潜力等待着人类去探索和创新。VLC 的其他优势包括不受无线电干扰、没有电磁辐射和高度保密性。然而，VLC 最大的优势还是其速度快。当今的实验室数据传输记录超过 20 Gbit/s，如此高的速度使得无线下载一部超高清电影仅需几秒钟。

典型的 VLC 系统由三个主要部分组成：可见光发射器、传输通道和接收器。信息传输始于光发射器中的信号编码、调制和预平衡。然后，光通过自由空间传输到接收器，接收器中会使用pin光电二极管或雪崩光电二极管将光信号转换为电信号。之后，会进行均衡、解调和解码，以恢复原始传输信号。

目前，VLC 系统存在两个重大限制。一个与发射器有关，例如强度调制直接检测系统中的高速蓝色激光器。这种光源的带宽相对较小，成熟度远不及在 1550 nm 左右工作的同类光源。第二个限制是相干调制系统中关键组件（例如外部调制器、放大器和平衡光电探测器）的开发缓慢。

在复旦大学，我们正在努力解决这些限制，首先是开发一种具有更高调制速率的新型 GaN 激光器。

![](/picture/fudan1.jpg)

(a) 激光外延结构。(b) 高速蓝色激光二极管芯片的显微照片。

高速光源
正如中国古语所说：工欲善其事，必先利其器。我们在开发 GaN 基激光器时牢记了这一建议，GaN 基激光器是白光的基本元件，也是水下无线光通信的有前途的光源。目前，发射紫光、蓝光和绿光的 GaN 基激光器主要用于光存储、照明、显示和材料处理等领域，重点关注直流特性，例如输出功率和斜率效率。由于极化效应，在 c 面GaN衬底上制造的蓝色激光器中存在强大的内置电场，研究人员正在利用半极性和非极性 GaN 衬底来消除这种极化场。这可以提高效率和增加调制带宽。然而，具有合适取向的 GaN 衬底供应有限。

我们在开发高速 GaN 基激光器的过程中，既考虑了外延结构的设计（包括有源区和电子阻挡层），也考虑了器件结构（例如脊形波导）。通过对各种外延结构的模拟，我们发现了设计规则，这些规则使我们改善了 InGaN/GaN 量子阱激光器的频率响应，随后通过实验工作验证了这些发现。

我们的高速激光器的测量和特性分析涉及光-电流-电压特性、发射光谱、结温、相对强度噪声、频率响应和数据传输性能的详细分析。我们通过确定光-电流-电压特性获得了激光器的阈值电流和斜率效率。我们进一步提取了激光器的固有参数。-3dB 调制带宽可以通过小信号频率响应测试得出。在这项工作中，我们对设计对性能的影响有了深入的了解，例如，不同波导层结构的影响，发现较厚的波导层结构会导致光场更加发散，从而增加其总体积。p和n波导层的最佳厚度分别为 50 nm 和 150 nm。

![](/picture/fudan2.jpg)

VLC 应用场景。

与 LED 一样，缩小激光二极管的尺寸为提高其高速运行提供了一条有希望的途径。我们发现，由于光场体积较小，较短的腔体可以提高调制性能。然而，这是有代价的，会增加镜面损耗并抑制阻尼效应。尽管存在这些缺点，我们还是展示了一种基于高速蓝色激光的 VLC 系统，其传输速率高达 20.06 Gbit/s，而使用绿色激光的变体传输速率达到 17.73 Gbit/s。

在基于激光的 VLC 技术快速发展的基础上，我们正在改进这项技术，以实现一个连接性更好的世界。我们对 VLC 的愿景包括将照明和通信相结合的室内系统，以及长距离和水下无线光通信。为了将这些想法变成现实，我们的实验室正在追求创新的设计和实践。

用于移动的 VLC……
当激光二极管部署在 VLC 系统中时，它们承诺提供高调制带宽和输出功率，这些属性可以实现高速、长距离通信。然而，由于激光二极管产生的光束较窄，因此在基于激光的光无线链路中需要指向和对准，这限制了通信系统的移动性。具有广泛覆盖范围的发射器和增强的移动性的 VLC 为无线服务提供了根本优势，为用户提供了灵活性和便利性，同时实现了移动连接。因此，我们超越了点对点 VLC 链路，并试图找到一种解决移动通信相关挑战的方法。

利用具有广泛空间覆盖范围的基于激光的光发射器，实现了具有移动接收端的 VLC 系统，取得了进展。使用最简单的调制技术开关键控 (OOK)，在基于激光的白光 VLC 链路中实现了超过 500 Mbit/s 的数据速率。传输在 1 m 和 2 m 的距离下都很稳定，并且当系统以 0.48 m/s 的速度移动时，该系统能够支持 500 Mbit/s 的传输速率。虽然距离和移动性会影响系统的性能，但它能够保持相当程度的可靠性和效率。

![](/picture/fudan3.jpg)

波分复用 VLC 系统的设计，以及相应的物理原型。

…室内照明…
VLC 的一个关键优势是它可以将照明和通信结合起来。为了确保以低碳足迹和与照明系统兼容而降低的运营成本实现这一目标，VLC 可能不会来自增加光源的数量。相反，扩大单个光源的视野是一个好主意。

白光源由蓝色激光阵列、扩散器、平凸透镜和陶瓷荧光板组合而成。基于激光的白光源表现出出色的稳定性，照射范围延伸至 20° 的半角。为了确保高频谱利用率，我们采用了离散多音比特加载调制。通过这种方法，我们将激光器的带宽划分为 256 个子载波，每个子载波都根据其比特误码率匹配调制阶数。在 VLC 系统中使用该发射器，峰值数据传输速率已达到 3.24 Gbit/s，跨度为 1 m 至 5 m。该结果有望展示用于移动网络应用的长距离、广覆盖、高速 VLC 链路，以及利用基于激光的白光发射器进行固态照明的可行性。

… 和卫星互连
在太空中，一个重要的趋势是卫星星座的建设。这对多颗卫星之间的实时数据链路有影响，这些链路需要大容量、低延迟和高可靠性的通信方法。卫星之间通常使用激光通信。目前，由于设备和系统已经成熟，红外波段被选为卫星间和卫星对地通信。展望未来，考虑到 GaN 及其相关合金的抗辐射性能，蓝色激光器可能成为卫星间光无线通信的有用光源，例如涉及低地球轨道卫星以提供互联网接入的通信。

为了通过 VLC 推进卫星间通信，我们专注于增加通信容量和距离。对于前一个目标，我们一直在研究使用波分复用 (WDM) 技术的能力。使用 40 通道 WDM VLC 系统，我们实现了 418.3 Gbit/s 的总传输速率，采用了离散多音比特功率加载和 Levin Campello 算法。在增加通信距离方面，我们将双向储层计算应用于 VLC 波形以进行符号级均衡，这种方法使我们能够在 100 米的自由空间距离内以 11.2 Gbit/s 的速度记录传输。

水下视频流
可见光通信的另一个重要应用是水下无线光通信（UWOC）。由于海水中存在蓝绿传输窗口，在此谱域发射的激光器是实现水下无线数据链路的有吸引力的候选者。

目前，UWOC 面临的主要挑战是普遍存在的时变和复杂的信道特性。典型的基于激光的 UWOC 链路基于高斯光束。当存在气泡、湍流或障碍物等干扰时，到达接收端的光束质量会下降。典型问题包括光强度的降低和光束质心的剧烈漂移运动。因此，在长距离上实现稳定、高速的数据传输具有挑战性。

我们的团队通过引入高效可见光超宽带自聚焦艾里光束超表面来应对这一挑战。在自聚焦区域，小规模障碍物引起的阻碍被旁瓣中携带的能量减弱；在发散区，艾里光束独特的圆形能量分布增强了系统对障碍物的适应性。这种超表面设计在440 nm 至 640 nm 的宽光谱范围内表现出高偏振转换效率，使无线光通信系统的数据传输速率提高了 91%，从而能够使用水下光通信数据链路通过 WDM 实现可靠的 4K 视频传输。展望

未来，基于激光的 VLC 仍有许多挑战需要克服。要将 GaN 基激光二极管的调制带宽提高到几十 GHz，还需要取得很大的进展。当电信界专注于以 100 G bit/s 到 Tbit/s 运行的光链路时，VLC 界的研究人员才刚刚进入这个领域，数据速率为几十 Gbit/s。

![](/picture/fudan4.jpg)

基于超表面的 Airi Light 水下光通信系统。(b) 使用全色超表面系统的水下 4K 视频流。(c) 在不同帧序列下接收带有和不带有全色超表面的视频帧。

此外，当今的 VLC 系统采用强度调制直接检测。这是因为仍然缺少可见光谱中的外部调制器、放大器和其他重要的光通信组件。同时，相干 VLC 系统的开发才刚刚开始，需要引入窄线宽激光器和高速平衡光电探测器。

在推进 VLC 的过程中，我们的团队正在与全球合作伙伴合作开发高性能 III 族氮化物光电器件和可见光光子集成电路技术。我们正与国际合作者一起努力实现一种环保、节能、低成本、高速的基于激光的 VLC 技术，作为 6G 网络的重要组成部分。

FURTHER READING / REFERENCE 
➤ J. Wang et al. "High-speed GaN-based laser diode with modulation bandwidth exceeding 5 GHz for 20 Gbps visible light communication," Photonics Res. 12 1186 (2024) > Y. Hou et al. "Wide field-of-view laser-based white light transmitter for visible light communications," Opt. Lett. 49 2805 (2024) 
➤ J. Hu et al. "A metasurface-based full-color circular auto- focusing Alry beam transmitter for stable high-speed underwater wireless optical communications," Nat. Commun. 15 2944 (2024) 
➤ Z. Lu et al. "11.2 Gbps 100-meter free-space visible light laser communication utilizing bidirectional reservoir computing equalizer," Opt. Express 31 44315 (2023) > J. Wang et al. "Study of equivalent circult of GaN based laser chip and packaged laser," Sci. Rep. 14 11368 (2024) 
➤ Y. Hou et al. "Tutorial on laser-based visible light communications," Chin. Opt. Lett. 22 092502 (2024) 
➤ C. Guan et al. "High-speed InGaN/GaN Green Laser Diode for 17.73 Gbps Visible Light Communication," 2024 30th International Semiconductor Laser Conference (ISLC), IEEE. (accepted) 2024.

<https://compoundsemiconductor.net/article/120606/Targeting_ubiquitous_communication_with_GaN_lasers>

# 28. Nvidia

## 28.1 Nvidia 展示了光学连接的 GPU 系统可能是什么样子

几周前，Nvidia 与 Ayar Labs 签署了研发合作协议，我们坐下来与这家硅光子学初创公司的首席执行官 Charlie Wuischpard 聊了聊，谈论了两家公司将开展哪些合作。Nvidia 参与了 Ayar Labs 今年早些时候进行的 C 轮融资，当时该公司筹集了 1.3 亿美元用于开发其带外激光器和硅光子互连。惠普企业 (Hewlett Packard Enterprise) 也在今年 4 月的那轮融资中投资了该公司，该公司今年 2 月还与 Ayar Labs 签署了一项协议，以研究如何将硅光子学引入 Slingshot 互连。Ayar Labs 也得到了英特尔的早期支持，尽管英特尔希望将激光器嵌入芯片内部，而不是像 Ayar Labs 那样从芯片外部泵入激光信号。 （如果现在有什么是真的，那就是英特尔现在不能犯任何错误。因此，英特尔利用硅光子学来规避风险是件好事。）

下面是 GPU 和 NVSwitch 如何使用光学引擎将电信号转换为光信号以创建 GPU 的 NVSwitch 网络的框图：

![image](/picture/nvidia-dally-optical-engine-interconnect.jpg)

<https://www.nextplatform.com/2022/08/17/nvidia-shows-what-optically-linked-gpu-systems-might-look-like/>

# 29. OELab动态

## 29.1 清华大学罗毅院士团队到北京芯能交流技术 2022.9

9月1日，清华大学罗毅院士团队一行来到北京芯能电子科技有限公司进行技术交流。北京芯能是探路者集团控股子公司，是一家Mini/Micro LED显示驱动IC及解决方案提供商，是目前国内唯一具有主动式直显、背光显示驱动两条产品线的芯片设计公司。

9月1日，清华大学罗毅院士团队一行来到北京芯能电子科技有限公司进行技术交流。北京芯能是探路者集团控股子公司，是一家Mini/Micro LED显示驱动IC及解决方案提供商，是目前国内少数具有主动式直显、背光显示驱动两条产品线的芯片设计公司。

罗毅是中国工程院院士、清华大学教授，目前担任北京信息科学与技术国家研究中心副主任。罗毅院士长期从事半导体光电子器件研究，是我国信息光电子技术的学术带头人之一，他在高速宽带光电子器件、GaN基LED及半导体照明技术方面取得了诸多创新成果，推动了我国信息光电子技术和产业的发展。其团队成员汪莱老师长期从事GaN基LED研究，在LED器件物理、面向显示和通信应用的Micro-LED方面取得了研究成果。同时，他非常注重产学研结合，曾参与编撰《Micro-LED产业技术路线图》，并和国内多家龙头企业开展过合作。

参加会议的人员除罗毅院士、汪莱老师外，还包括探路者集团董事长李明、副总裁杨树、投资部刘凯及芯能科技CEO金镇赫、企划部朱顺京等。

会上首先由探路者集团副总裁杨树介绍了北京芯能产品线和技术路线，并现场展示了Mini-LED全矩阵区域调光落地方案。汪莱老师介绍了团队在Micro-LED材料和芯片上的研究进展，并就芯片尺寸10μm以下的Micro-LED的物理效应和芯能进行了讨论。罗毅院士和汪莱老师回顾了显示技术的发展历程，认为Mini-LED动态背光技术对LCD电视的画质提升明显，对芯能灯驱合一的技术路线高度认可，认为双方可在基于硅基驱动IC的Micro-LED智能显示芯片方向上进行深入探索。此次会议为双方后续合作打下了坚实基础。

<http://bxet-vision.com/#/newsdetail?id=425>

# 30. 光互连的思考

## 30.1 光互连的思考：哪些铜互连将被光互连取代 VPIphotonics

支持光子的云计算 （PECC） 峰会今天刚刚结束，以下是我个人从此次活动中得到的收获：

1.） 很明显，光互连是 AI 数据中心的关键使能技术（但我们都知道，这就是我们在那里的原因）

2.） 多年来，关于线性可插拔光学器件 （LPO）、近封装光学器件 （NPO） 和共封装光学器件 （CPO） 等不同方法的讨论很多。这一事件清楚地表明，这不是一个或另一个的问题，而是每个都有自己的位置。一些应用程序需要 LPO 提供的灵活性，而另一些应用程序需要 CPO 提供的更高性能，因此所有这些解决方案将根据用例共存。

3.） 真正的问题是：哪些铜互连将被光学互连取代？人们认为光学器件可以取代铜用于米级 GPU 到 GPU 连接（如 NVLink），这仍有待证明，但有很多人正在努力。与此同时，铜有望在 GPU 到 HBM3 等较短的毫米级连接中保持主导地位。

4.） 硅光子学正在大规模实施，但我们需要更多的最终用户要求围绕 PDK 和行业测试的标准化，以推动我们达到一个新的成熟水平并推动更广泛的采用。

VPIphotonics 通过提供仿真工具来帮助解决这些挑战，这些工具允许您在单个接口中对完整光传输系统中的光子集成电路 （PIC） 进行建模和仿真。然后，您可以使用我们与 Keysight Technologies ADS 的联合解决方案扩展该解决方案以模拟整个电-光-电 （EOE） 链路，从而实现电-光协同设计和完整的端到端链路验证。

在此处查看我们的 EOE 解决方案的简短演示：https://lnkd.in/ePBw9aiy

Linkedin: Chris MaloneyChris Maloney

## 30.2 信息图 Tuesday （IT）：光互连将以 5 比 1 甚至 10 比 1 的比率增长比 XPU 更快 Marvell

“光纤 [互连] 是唯一可以为您提供连接整个数据中心数万台服务器所需的带宽和覆盖范围的技术...虽然铜仍然是芯片到芯片和其他短距离连接的可行技术，但光学是 AI 的主要介质......随着速度的提高和距离的扩大，互连的数量将急剧增加......光互连的增长速度将比 AI 集群中的加速器 [或 XPU] 增长更快。

![](/picture/optical_interconnects.jpg)

<https://www.linkedin.com/posts/mingliangliu_semiconductorindustry-semiconductor-semiconductors-activity-7257047321077571585-0uo9?utm_source=share&utm_medium=member_desktop>

补充阅读：
🏷️扩展 AI 意味着扩展互连：<https://www.marvell.com/blogs/scaling-ai-means-scaling-interconnects.html>

🏷️数据中心内链接：<https://www.linkedin.com/posts/mingliangliu_ai-hpc-semiconductor-activity-7217311426044993537-Chdc/>

数据中心内互连 （DCI） 市场正在经历一场重大变革。与 Inter-DCI 市场相比，Intra-DCI 市场需要更大的端口/链路/电缆运输量和对数据传输 （I/O） 能效、信号延迟、通道速率或信道速度（每个波长）、带宽（海岸线）密度和系统可扩展性的更严格要求，再加上人工智能 （话题标签#AI ） 和高性能计算 （话题标签#HPC ） 应用的天文数字增长。 📈
 
2024 年是数据中心部署共封装光学器件 （CPO） 的“年⃣”1️吗？
💡与其现在匆忙下结论，不如让我们在一两年后回过头来。

![](/picture/Intra-Datacenter.jpg)

<https://www.linkedin.com/posts/mingliangliu_ai-hpc-semiconductor-activity-7217311426044993537-Chdc?utm_source=share&utm_medium=member_desktop>

补充阅读：
🏷️英特尔 的光计算互连 （OCI） 技术： https://lnkd.in/gWfrDceC
🏷️ 台积公司 的“COUPE”：https://lnkd.in/gkyKm_HD
🏷️ GlobalFoundries 的“Fotonix”：https://lnkd.in/gKHwSfDR
🏷️ 诺基亚 已购买 Infinera ： https://lnkd.in/gZJdvnVi
🏷️CPO 示例 （V）：https://lnkd.in/gAGh_nwK
🏷️CPO 示例 （VI）：https://lnkd.in/gbajACdV



# 31. 新型深紫外微型 LED 阵列推动无掩模光刻技术发展 - 中科大

![](/picture/new-duv-micro-led-arra.jpg)

中国科学技术大学孙海鼎教授团队研发出垂直集成微尺度发光二极管（micro-LED）阵列，并首次应用于深紫外（DUV）无掩模光刻系统。该项研究成果发表在《激光与光子学评论》上。

光刻技术在集成电路芯片制造中发挥着至关重要的作用，是半导体和微电子工业的关键核心技术之一。自20世纪90年代以来，低成本、高分辨率无掩模光刻系统成为先进光刻技术研究的热点。然而，该项前沿技术的专利主要掌握在欧洲、美国、日本和韩国手中，技术壁垒较高。

在此背景下，孙教授带领的iGaN团队多年来对深紫外微LED进行了深入研究，创新性地提出了以深紫外微LED阵列为光源的无掩模光刻系统。

他们系统地设计和优化了深紫外微型 LED 的外延结构、器件尺寸、侧壁轮廓和几何形状，大大提高了其功率效率、调制带宽以及在紫外光检测、成像和传感方面的多功能性。在此基础上，该团队成功开发了基于这些深紫外微型 LED 的阵列系统。

在本项工作中，该团队进一步提出并制作了一种深紫外显示集成芯片，充分利用了深紫外微LED超小尺寸和超高亮度的优势，提出了一种三维垂直集成器件架构，其中AlGaN基深紫外微LED阵列与氧化锌（ZnO）基光电探测器（PD）通过透明蓝宝石衬底并排。

在这种架构下，从 DUV 微型 LED 阵列发射的紫外光子可以穿透透明蓝宝石基板，并被基板背面的 PD 捕获，从而实现高效的光信号传输。

此外，团队还基于垂直集成器件开发了闭环反馈控制的自稳定发光系统，该系统不仅可以监测Micro-LED阵列输出光强的波动，还可以提供持续的反馈，以保证输出功率的稳定。

测试结果表明，具有自稳定系统的装置能保持较高的光强和长期稳定性，而无反馈系统的装置光强随着时间的推移逐渐下降。

利用该反馈系统，该团队演示了像素密度高达 564 像素/英寸 (PPI) 的 DUV 微型 LED 阵列，并在无掩模 DUV 光刻后成功在硅片上显示出清晰的图案，表明高分辨率光刻技术具有潜力。这是基于 DUV 微型 LED 有源矩阵的 DUV 无掩模光刻的首次演示。

该研究开发了一种新型深紫外微型LED阵列与PD相结合的集成器件，为未来无掩模光刻系统展示了巨大的应用前景，也为未来发展高集成、多功能的三维光电集成系统奠定了基础。

下一阶段，团队将致力于进一步缩小单个Micro-LED和PD的尺寸，从而提高单位面积阵列的密度和集成度，并优化单个器件的性能和大晶圆的均匀性，为无掩模光刻技术的更高精度奠定基础。

<https://phys.org/news/2024-10-deep-ultraviolet-micro-array-advances.html>

# 32. 用于传感、生产和通信的紫外线微型 LED - 柏林费迪南德-布劳恩研究所 (FBH) 

柏林费迪南德-布劳恩研究所 (FBH) 的研究人员已成功生产出首批发射紫外线光谱范围 (UVB) 的微型 LED 原型。发射波长为 310 纳米 (nm) 的微型 LED 的发射区域尺寸很小，直径小至 1.5 微米 (µm)。这比传统的 UV LED 小数百到数千倍。微型 LED 可以紧密排列，间距小至 2 µm，在芯片上形成二维阵列，从而产生高分辨率的 UVB 发射区域。

UV 微型 LED 既可以用作单个发射器，也可以排列成高密度阵列，可用于各种应用。这包括传感技术、聚合物和树脂固化、半导体芯片生产和光通信。在 FBH 目前的芯片上，阵列中的所有 UV 微型 LED 都是同时运行的。下一步，LED 像素将通过控制芯片单独寻址。这将使它们能够生成并快速调制单个照明图案，例如实现无掩模光刻。因此，可以轻松、快速且经济高效地在半导体晶圆上创建单个结构。

高分辨率紫外线照射模式的能力还为快速成型和荧光分析领域开辟了新的应用。与此同时，FBH 科学家已经将这项技术转移到 UVC LED，包括发射波长极短（约 230 nm）的远 UVC LED。现在，FBH 正在寻找打算在其应用中使用 UV 微型 LED 的合作伙伴，旨在共同推进该技术并充分发挥设备的潜力。

![](/picture/uv-micro-leds-for-sens-1.jpg)

通过金属有机气相外延沉积在紫外线光谱范围内发光的半导体层结构，然后使用光刻工艺、等离子蚀刻和沉积方法进行图案化。制造直径在 1.5 至 50 µm 之间、间距在 2 至 60 µm 之间的小 UV 微型 LED 需要很高的对准精度、制造精度和材料完美性。

这只能通过使用专为此应用设计的最先进的光刻工艺来实现。需要将不同的工艺层精确对准（叠加控制），精度要优于 20 nm，覆盖 2 英寸 LED 晶圆。由于制造的 UV 微型 LED 尺寸很小（例如蚀刻结构的直径、形状和倾斜角），因此其特性通过电子显微镜进行控制。

https://techxplore.com/news/2022-07-uv-micro-leds-production.html

# 33. Introduction and Research Trends on Micro LED Technology

Abstract Currently, micro LEDs (Light Emitting Diode) are attracting attention in the lighting field along with next-generation displays and have advantages such as high luminance, operating speed, energy efficiency, and long-term driving. It is predicted to bring new innovations in smartphones, televisions, and wearable electronic devices. These micro displays are self-luminous displays that emit light by themselves by being implemented as pixels composed of micrometer-sized LED …
•	Cites: Influence of dislocation density on internal quantum efficiency of …

new citation to articles by Lai Wang

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Introduction%20and%20Research%20Trends%20on%20Micro%20LED%20Technology.pdf>

# 34. Influence of dislocation density on internal quantum efficiency of GaN-based semiconductors - 余佳东

<https://pubs.aip.org/aip/adv/article-pdf/doi/10.1063/1.4979504/8465403/035321_1_online.pdf>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/035321_1_online.pdf>

# 35. InGaN quantum dots for micro-LEDs - 汪莱

综述

引文52，53是W.B.Lv文章

<https://pubs.aip.org/aip/app/article/9/10/100904/3317660>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/InGaN%20quantum%20dots%20for%20micro-LEDs.pdf>

# 36. 基于等效电路模型的GaN基Micro-LED调制带宽分析 - 厦门大学/复旦 田鹏飞

我们建立了基于 GaN 的 Micro-LED 系统的等效电路模型，其中融入了印刷电路板和键合线的寄生参数。我们的深入分析表明，本征 Micro-LED 的参数显著影响 Micro-LED 的调制带宽。随着 Micro-LED 的电阻和电容的增加，Micro-LED 的带宽急剧下降。为了解决这个关键问题，我们基于等效电路模型的分析提出了几种可行的策略。特别是，我们开发了深蚀刻技术来提高 Micro-LED 系统的带宽。通过拟合浅蚀刻和深蚀刻 Micro-LED 等效电路模型的阻抗参数，深蚀刻器件的电极电容与浅蚀刻器件相比降低了 24.9 pF。这使得在 4 kA/cm 2的低电流密度下调制带宽从 203 MHz 显着提高到 249.8 MHz 。拟合参数模拟带宽的高度一致性证明了我们提出的等效电路模型的有效性和可靠性。

<https://opg.optica.org/oe/fulltext.cfm?uri=oe-32-22-39974&id=561574>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Modulation%20bandwidth%20analysis%20of%20GaN-based%20micro-LED%20deduced%20by%20an%20equivalent%20circuit%20model.pdf>

# 37. 使用网络分析仪测量确定 LED 等效电路

我们对一些偏置为 1 至 10 mA 的预生产 DH LED 进行了测量，对于每种情况，我们都获得了宽带输入阻抗图，该图给出了幅度和相位随频率的变化。我们从这些图中推导出每个二极管的载流子寿命、差分二极管电阻、扩散电容、寄生电阻和理想因子。然后在等效电路中使用这些参数来计算设备的模型输入阻抗，然后将其与测量结果进行比较。在很宽的频率范围内，至少在频率等于 1/（载流子寿命）时，一致性很好。我们的模型充分考虑了之前在单端口激光测量中注意到的最大相位滞后的存在。

<https://ieeexplore.ieee.org/document/791628>

# 38. 关于铜在计算领域的未来，需要记住的九件事 Marvell

作者：Michael Kanellos，Marvell 网红关系主管；Vienna Alexander，Marvell 营销内容实习生

铜死了吗？

远非如此。然而，铜技术将在未来几年发生巨大转变。以下是指南。

1. 铜是最适合居住的金属

自 Colossus 和 ENIAC 时代以来，铜一直是互连的主要材料。它是一种优质的导体，成本远低于金或银，并且电阻相对较低。20世纪 90 年代末，铜还取代了铝，用于连接芯片内的晶体管，因为其电阻降低了 40%，性能提高了 15% 1。

铜线也简单、可靠且耐用。互连本质上是电线。相比之下，光互连需要大量组件，例如光学 DSP、跨阻放大器和激光器。

Marvell 光学技术执行副总裁 Loi Nguyen 博士表示：“光学技术的第一条规则是‘凡是能用铜做的事情，就用铜做’。”

2. 但它仍然是一种金属

尽管如此，电阻仍然存在。随着带宽和网络速度的增加，热量和功耗也会增加。此外，增加带宽会减少覆盖范围，因此将数据速率加倍会使距离缩短约 30-50%  （见下文）。

因此，光学技术已经取代了数据中心和电信网络中五米或更长的互连线中的铜。 

![](/picture/where-are-copper-interconnects-used.jpg)

来源：Marvell

3. 200G标志着一个转折点

SerDes 是网络的基本单元，是最终决定网络其他组成部件性能的基本输入输出结构。当前的 12.8T 网络由数百万个 50G 铜线和光纤 SerDes 组成。一条 400G 电缆或模块将包含八个 SerDes，而 32 条 400G 电缆将插入单个交换机。未来几年将实施的 51.2T 网络将主要依赖 100G SerDes。依赖 200G SerDes 的网络将在 2027 年腾飞。然而，更高的带宽意味着更短的覆盖范围。 

![](/picture/serdes-shipment.jpg)

来源：Marvell

4. 更高的带宽/更短的距离会影响系统之间和系统内部的连接

五米及以下的铜缆连接大致可分为两类：电缆和电线。连接同一机架内的服务器和交换机的铜缆基于无处不在的以太网协议。传统的以太网直连铜缆 (DAC) 可以在 5G 下传输三米信号——足以满足当今机架的需求——但在 200G 下只能传输大约一米。数据中心机架通常高七英尺；因此，即使将交换机放在中间，200G 以太网电缆也不足以将机架中的所有系统连接在一起，除非使用非自然的工程技巧。

相比之下，同一块主板或同一系统内的芯片则依靠利用 PCIe 的有线连接。数据速率和距离要低得多：PCIe Gen 4 连接每通道可传输高达 16GB 的数据，传输距离可达 8 英寸。热量和功率限制要求更高，物理连接本身要薄得多，而且 PCIe 连接通常需要更低的延迟和更高的数据包传输可靠性：应用差异是传输速度差异的很大一部分原因。

但是，与以太网一样，PCIe 也面临距离挑战。PCIe Gen 6 设备（64 GB/通道）只能在两英寸内发送数据，否则数据可能会损坏。由于云服务提供商需要更大的服务器，并想方设法将服务器组件分布在相邻的主板和服务器上，因此这还远远不够。PCIe Gen 6 将开始出现在与基于 200G 的以太网同一代的系统中。

铜线也是企业和小型企业网络的主流，因为带宽需求在 1-10G 范围内。因此，目前更长的覆盖范围并不是一个大问题。

5. 以太网的解决方案？将光学元件引入铜线

有源电缆 (AEC) 有效地在铜缆终端添加了光学 DSP，以放大和微调信号。例如，今年早些时候推出的用于 AEC 的 Marvell® Alaska® A 1.6T PAM4 DSP 是业界首款用于此应用的 1.6 Tbps 设备。虽然在电缆中添加半导体会增加成本和总功耗，但它在 200G 时将距离延长了三倍，在 50G 时将距离延长了七米。在这些距离下，铜成为服务器到交换机和服务器到服务器连接以及 AI 集群中系统链接的可行介质。

![](/picture/dac-and-aec-cables.jpg)

来源：Marvell

可以通过增加电缆的规格来延长 DAC 电缆的长度。但不幸的是，由此产生的额外厚度使电缆变得僵硬且难以操作，这对设施管理人员来说是一个很大的麻烦，也是环境热量的来源。

电缆终端的 DSP 安装在熟悉的标准模块中，便于实施。TE Con​​nectivity、Molex 和 Amphenol 等公司正在开发采用 Alaska A 1.6T PAM4 DSP 的布线解决方案。  

![](/picture/marvell-alaska-dsp-extends-copper-reach.jpg)

来源：Marvell

同时，有源光缆还包括带有光学 DSP 的跨阻放大器和驱动器。AOC 电缆能够传输长达 30 米的数据，以适应更大的 AI 集群和分解系统。

6. 对于 PCIe，光学技术得到集成

与 AEC 和 AOC DSP 一样，PCIe 重定时器代表了一类可延长铜互连长度的新型设备。两者的区别在于标准、用例和借鉴自光学领域的技术。

今年早些时候发布的单个1.6T Marvell Alaska P 重定时器可用于将 Gen 4 PCIe 链路从 8 英寸扩展到 20 英寸以上，而 Gen 6 PCIe 链路则从 2.5 英寸扩展到大约 17 英寸。更长的链路为物理上更大的系统和分解系统打开了大门，这些系统可以提供更好的性能，同时减少热点。

PCIe 重定时器不会将光学 DSP 或完整组件集成到自己的设计中。相反，它们会改造光学技术和概念。例如，5nm Alaska P 是围绕等效 DSP 内部使用的相同 SerDes 构建的。该设备还使用 PAM4 调制方案，使数据速率翻倍。当前的 PCIe 设备使用较旧的 NRZ 调制方案。

![](/picture/pam4-modulation-for-higher-pcie-speeds.jpg)

来源：Marvell

而且，如上所述，PCIe 重定时器用于连接同一系统的组件。Alaska P 可用于将 AI 处理器相互连接或连接到 CPU。这些设备还可用于将 GPU 相互连接。此外，PCIe 重定时器可能会与 CXL 控制器一起部署，以将处理器连接到内存。

单位数量也可能非常可观。根据 650 Group 的数据，两年内出货的 75% 的云和 AI 服务器将依赖 PCIe 重定时器，并且通常包含多个设备。该公司补充说，一台 8 GPU 服务器可能包含 16 个 PCIe 重定时器。 

![](/picture/waldo-the-pcie-retimer.jpg)

来源：Marvell

7.更多芯片意味着更多系统智能

与 AEC 和 AOC 设备一样，PCIe 重定时器可以收集遥测数据，以提高系统性能和预测性维护。

8.人工智能将推动 PCIe 速度更快

本月初， PCIe Gen 7 SerDes 在 OCP 上亮相，其运行速度可达 128GT/秒。这是一张照片。

![](/picture/pcie-gen7-serdes.jpg)

来源：Marvell

9. 下一步：芯片内部的光学

几十年来，未来学家一直在讨论将光学接口引入芯片的好处。现在，多种力量的汇聚正在铺平道路。芯片设计和先进封装为将光学互连集成到半导体设计中提供了框架。研发工作稳步推进，功率也日益成为瓶颈。

台积电最近表示，它正在加快硅光子解决方案的开发，以便在三到五年内使该技术投入生产。到 2028 年，光学芯片可能形成一个价值5 亿美元的市场3。

Marvell 光学和云连接高级副总裁兼首席技术官 Radha Nagarajan 表示，光学可以降低 30% 或更多的功耗3。不过，AI 芯片必须重新设计才能适应这些接口。

参考资料：

1.IBM ，2018年 
<https://www.ibm.com/history/copper-interconnects>

2.. 650 Group， 2024 年第二季度商用硅片报告。行业估计
<https://650group.com/reports/data-center-ethernet-switch-semiconductors-2/>

3.日经商业科技，2024 年 9 月。
<https://asia.nikkei.com/Business/Technology/TSMC-aims-to-ready-next-gen-silicon-photonics-for-AI-in-5-years>

<https://www.marvell.com/blogs/nine-things-to-remember-about-the-future-of-copper-in-computing.html?utm_source=li&utm_medium=blog&utm_campaign=copper-tech>

# 39. GaAs-AlGaAs 高亮度 LED 用于光通信系统的功率和调制带宽

提示词：详细整理这篇文档，输出格式清晰的总结

## 39.1 Google给出的总结

GaAs-AlGaAs 高亮度 LED 用于光通信系统的功率和调制带宽
**摘要：**本文介绍了一种针对 GaAs-AlGaAs 双异质结高亮度 LED 的分析模型，该模型旨在用于光通信系统。该模型考虑了所有重要的器件和材料参数，如自吸收、异质界面复合、掺杂浓度、有源层厚度、注入载流子密度以及载流子限制。本文讨论了这些参数对 LED 输出功率和调制带宽的影响，并给出了与模型一致的实验结果。最佳高输出 50 µm LED（偏置在接近饱和状态）向空气发射 15 mW，辐射强度为 200 W/cm² sr（迄今为止报道的表面发射 LED 中最高的辐射强度），调制带宽为 17 MHz；获得的最高带宽是在 2 mW 输出时为 170 MHz。

关键词： LED，GaAs-AlGaAs，双异质结，光通信，功率，调制带宽，自吸收，异质界面复合。

一、引言

自 1971 年 Burrus 和 Miller 首次报道 GaAs-AlGaAs 高亮度 LED 以来，这些器件作为光波通信潜在光源的应用前景越来越受到关注。对于这种小面积器件来说，在光波通信应用中需要考虑最重要的特性是输出功率（或效率）和调制带宽。本文将讨论一些与 LED 性能相关的器件参数，重点关注与通信光源相关的参数。这些参数包括自吸收、异质界面复合、掺杂浓度、有源层厚度、注入载流子密度以及载流子限制。最近的一些出版物已经讨论了这些参数的某些方面：Harth 和 Heinen 研究了单异质结 LED 中吸收和表面复合的影响以及这些器件的频率响应；King、SpringThorpe 和 Szentesi 展示了双异质结（DH）LED 效率和上升时间的实验结果，这些结果是作为有源区空穴浓度的函数，但没有给出分析；Ettenberg 和 Kressel 研究了 AlGaAs-GaAs 异质结的界面复合；Ettenberg、Kressel 和 Gilbert，以及 Casey、Miller 和 Pinkas，以及 Zucker、Laner 和 Schlafer 测量了载流子浓度随载流子浓度变化的关系；Lee 分析了 Burrus 型 LED 频率响应的寄生效应，并由 Burrus、Lee 和 Holden 进行了报道；King 等人报道了 LED 的高功率性能，而 Lockwood、Wittke 和 Ettenberg 报道了 LED 的高频性能。

二、内部量子效率和有效载流子寿命

已有文献表明 [13] 自吸收在一些类型的光发射二极管设计中起着重要作用。在像 GaAs 这样的直接带隙材料中，由于发射峰在重掺杂 n 型材料中向带隙边缘的高能侧移动，而在重掺杂 p 型材料中向带隙边缘的低能侧移动，因此发射峰的位置会发生偏移。由于光产生区域通常延伸到几个扩散长度，因此自吸收变得明显。在双异质结 LED 中观察到的更高外部效率（相对于扩散型同质结 LED）的一个明显原因是能够产生薄有源区，从而减少了自吸收。

三、调制带宽和功率带宽积

通过直接调制注入电流可以实现光输出的强度调制，前提是电流变化速率要比注入电子和空穴的复合速率慢。寄生元件（如空间电荷电容）会导致载流子注入结的延迟，从而导致光输出的延迟。如果保持恒定的正向偏置，则这种延迟可以忽略不计，因此 LED 的调制带宽仅受载流子复合时间的限制。如果电流以角频率 ω 调制，则光输出强度会随 ω 变化。

四、载流子限制

在前面的部分中，我们假设限制作用层中 AlGa1-xAs 的带隙足够大，以至于注入的载流子能够很好地限制在有源区。然而，当有源层非常薄或结温升高时，注入的载流子可能会获得足够的能量来越过异质结势垒。在本节中，我们将考虑异质结势垒的高度，以确定在不同温度下，以及在不同有源层厚度下，将注入载流子限制在 50 µm 直径发射区的实际二极管中所需的带隙差。

五、实验

六、结论

本文讨论了与 AlGaAs-GaAs 双异质结 DH LED 的效率和调制带宽相关的器件参数。这些参数是自吸收、异质界面复合速度、掺杂浓度、有源层厚度、注入电流密度以及载流子限制。其中一些参数是相互关联的。与扩散型同质结器件相比，DH LED 能够获得更高的功率，这是因为：首先，良好的异质结界面质量降低了非辐射复合；其次，可以在薄有源层中限制电子，这会提高注入载流子的密度；第三，由于注入载流子密度的增加，辐射复合速率提高，载流子寿命缩短。因此，功率带宽积得到了改进。将注入的载流子限制在 8 × 1018 cm-3 需要对于大于 1 µm 的有源层厚度来说，铝砷化物摩尔分数差 Ax ≥ 0.2，对于小于 0.5 µm 的有源层厚度来说，Ax ≥ 0.3。对于 w > 1 µm，界面复合速度 s = 2 × 103 cm/s，对于 w < 1 µm，s 则更小 [5]。分析中没有考虑的效应是高载流子密度下的横向扩散。横向扩散会降低有效电流密度，从而降低效率和带宽。输出功率的饱和主要是由于热效应，尽管其他因素如载流子泄漏和横向扩散也可能很重要。

致谢

作者感谢 C. A. Burrus 的许多有益的讨论，M. A. Pollack 的霍尔测量，D. L. Rode 提供了计算费米能级的程序，W. S. Holden 和 F. Favire 制作二极管，以及 H. E. Kehlenbeck 对器件的评估。

## 39.2 豆包给出的总结

GaAs - AlGaAs高辐射LED用于光通信系统的功率和调制带宽研究

**作者**：TIEN PEI LEE、ANDREW G. DENTAI
**发表刊物**：IEEE JOURNAL OF QUANTUM ELECTRONICS, VOL. QE - 14, NO. 3, MARCH 1978
**研究内容**：分析用于光通信系统的GaAs - AlGaAs双异质结构高辐射LED，考虑自吸收、异质界面复合、掺杂浓度、有源层宽度、注入载流子密度和载流子限制等参数对LED输出功率和调制带宽的影响，并给出实验结果。
1. **引言**
    - GaAs - AlGaAs高辐射LED作为光波通信系统光源受关注，其输出功率和调制带宽是重要特性。
    - 前人研究涉及多种相关因素，本文在此基础上进一步探讨影响LED性能的器件参数。
    - 本文先提出基本模型，再讨论调制带宽，考虑异质结构势垒高度对载流子限制的影响，最后给出实验结果支持模型适用性。
2. **内部量子效率和有效载流子寿命**
    - **模型建立**
        - 假设一维模型，适用于大活性面积与厚度比的LED（如Burrus型）。
        - 考虑电子扩散电流主导结电流，稳态连续性方程为\(D\frac{d^{2}n}{dx^{2}}-\frac{n}{\tau}=0\)，边界条件与异质界面表面复合速度\(s\)有关。
    - **电子密度与寿命**
        - 解得电子密度\(n(x)\)，进而得平均电子密度\(\vec{n}\)和平均有效载流子寿命\(\tau_{eff}\)。
        - 当\(Ls/D\ll1\)时，\(\frac{1}{\tau_{eff}}=\frac{1}{\tau}+\frac{2s}{w}\)，表明表面复合会降低载流子寿命。
    - **光强与效率**
        - 考虑自吸收后，\(p - n\)异质结处峰值光强\(P = (\frac{h\nu}{e})\eta_{i}J = (\frac{h\nu}{e})\eta_{0}\eta_{DH}^{n}J\)。
        - 得到双异质结构（DH）和单异质结构（SH）从不同层提取光时的内部量子效率降低因子\(\eta_{DH}^{n}\)、\(\eta_{SH}^{n}\)、\(\eta_{DH}^{p}\)、\(\eta_{SH}^{p}\)。
    - **参数影响分析**
        - 通过\(\eta_{DH}^{n}\)与\(w/L\)关系图分析，表面复合影响效率和寿命，自吸收在轻掺杂时重要，\(s = 10^{4}cm/s\)时有最佳有源区厚度，光从\(p\)侧提取时效率在大\(w/L\)时降低。
3. **调制带宽和功率带宽积**
    - **调制带宽**
        - 电流调制频率\(\omega\)时，光强随\(\omega\)变化，调制带宽\(\Delta f=\frac{1}{2\pi\tau_{eff}}\)。
        - 假设界面复合为主导非辐射复合过程，可得\(\frac{1}{\tau_{eff}}=\frac{1}{\tau_{r}}+\frac{2s}{w}\)，\(\tau_{r}\)与平衡载流子浓度和注入载流子有关，在低注入水平时带宽与掺杂浓度有关，高注入水平时带宽为\((JB/ew)^{1/2}/2\pi\)。
    - **功率带宽积**
        - \(\Delta f\cdot P\)在界面复合和自吸收可忽略时，低注入与\((JN_{A})\)成正比，高注入与\((J^{3/2}/w^{1/2})\)成正比，重注入可提高功率带宽积。
4. **载流子限制**
    - **势垒高度与载流子泄漏**
        - 考虑有源层薄或结温升高时载流子可能泄漏，需确定异质结构势垒高度以限制载流子。
        - 前人估计激光二极管阈值过电流的方法存在问题，本文考虑\(\Gamma\)导带谷电子和价带空穴，计算准费米能级确定过剩载流子浓度。
    - **计算与结果**
        - 计算注入电子密度，给出不同注入水平下的过剩电子电流密度\(J_{n}'\)和过剩空穴电流密度\(J_{p}'\)，总过剩电流密度\(J'\)。
        - 定义“限制因子”\(C=\frac{1}{1+(J'/J)}\)，计算表明\(w>1\mu m\)且\(\Delta x\geq0.2\)或\(0.1<w<0.5\mu m\)且\(\Delta x\geq0.3\)时可实现良好载流子限制。
5. **实验**
    - **晶片生长与二极管制造**
        - DH晶片用液相外延（LPE）生长，介绍各层材料、掺杂浓度和厚度。
        - 制造Burrus型结构二极管，在\(n - Al_{0.33}Ga_{0.67}As\)层开“井”。
    - **测量**
        - 用大面积校准光电二极管测总光功率，在300mA直流电流附近获最大功率输出。
        - 用RF电流调制LED，通过小面积快速\(p - i - n\)光电二极管检测光输出，用频谱分析仪显示，根据调制带宽测量评估载流子寿命。
    - **结果**
        - **功率输出相关因素**
            - 给出不同有源层厚度、掺杂浓度和\(\Delta x\)的实验结果，包括功率输出、发射波长等。
            - 分析功率输出与有源层厚度关系，得出界面复合速度\(s = 2×10^{3}cm/s\)，量子效率约70%，外部量子效率4 - 5%。
        - **调制带宽与载流子寿命**
            - 绘出不同掺杂浓度下带宽与\((J/w)\)关系，实验结果与计算吻合。
            - 表明低掺杂浓度下重注入可提高效率和调制速度，为获更高调制带宽可减小有源层厚度或增加掺杂浓度。
        - **最大输出功率与带宽**
            - 给出不同掺杂浓度和厚度二极管的最大输出功率与调制带宽关系，低掺杂密度时获高功率低带宽，高掺杂时带宽增加但功率降低，热加热使输出饱和。
            - 与同质结LED对比，DH LED轻掺杂活性区可获更高功率。
        - **光谱宽度**
            - 光谱宽度随掺杂浓度增加而增大，高调制率能力受光纤材料色散限制，可通过使用长波长LED克服。
6. **讨论与结论**
    - DH LED轻掺杂活性区可获更高功率，原因包括异质界面质量好、载流子可在薄有源层受限、辐射复合率提高。
    - 载流子限制要求特定\(\Delta x\)，实验二极管获一定输出功率和调制带宽，增加掺杂可提高调制带宽但降低功率并增宽光谱，输出功率饱和主要因热加热，未考虑高载流子密度下载流子横向扩散影响。

文档中的公式整理成 Markdown 格式

1. 稳态连续性方程：\(D\frac{d^{2}n}{dx^{2}}-\frac{n}{\tau}=0\)，其中\(n\)是电子密度（\(cm^{-3}\)），\(D\)是电子扩散常数（\(cm^{2}/s\)），\(\tau\)是体复合寿命（秒）。
2. 边界条件：
   - \(-\left.\frac{d n}{d x}\right|_{x = 0}=\frac{J}{e D}-\frac{s}{D}n(0)\)
   - \(\left.\frac{d n}{d x}\right|_{x = w}=-\frac{s}{D}n(w)\)，其中\(J\)是\(p - n\)异质结处的注入电流密度，\(e\)是电子电荷，\(s\)是表面复合速度（\(cm/s\)），\(w\)是有源层宽度。
3. 电子密度表达式：\(n(x)=\frac{J L}{e D}\left\{\frac{\cosh \left(\frac{w - x}{L}\right)+\frac{L s}{D}\sinh \left(\frac{w - x}{L}\right)}{\left[\left(\frac{L s}{D}\right)^{2}+1\right]\sinh \frac{w}{L}+\frac{2 L s}{D}\cosh \frac{w}{L}}\right\}\)，其中\(L\)是电子扩散长度（\(L=\sqrt{D\tau}\)，厘米）。
4. 平均电子密度：\(\vec{n}=\frac{1}{w}\int_{0}^{w}n(x)dx=\frac{J}{e}\frac{\tau_{eff}}{w}\)。
5. 平均有效载流子寿命：\(\tau_{eff}=\tau\left\{\frac{\sinh \frac{w}{L}+\frac{L s}{D}\left(\cosh \frac{w}{L}-1\right)}{\left[\left(\frac{L s}{D}\right)^{2}+1\right]\sinh \frac{w}{L}+\frac{2 L s}{D}\cosh \frac{w}{L}}\right\}\)，当\(Ls/D\ll1\)时，\(\frac{1}{\tau_{eff}}=\frac{1}{\tau}+\frac{2s}{w}\)。
6. 峰值光强表达式：\(P=\frac{h\nu}{\tau_{r}}\int_{0}^{w}n(x)e^{-\alpha x}dx\)，其中\(\tau_{r}\)是辐射复合寿命，\(\alpha\)是发射峰波长处的吸收系数。
7. 光强与电流关系：\(P = (\frac{h\nu}{e})\eta_{i}J = (\frac{h\nu}{e})\eta_{0}\eta_{DH}^{n}J\)，其中\(\eta_{0}=\tau /\tau_{r}\)（当\(s = 0\)，\(\alpha = 0\)时的内部量子效率），\(\eta_{i}\)是考虑界面复合和自吸收时的内部量子效率，\(\eta_{DH}^{n}=\eta_{i}/\eta_{0}\)（DH结构从\(n\)侧被动层提取光时的内部量子效率降低因子）。
8. 双异质结构（DH）从\(n\)侧提取光时的内部量子效率降低因子：\(\eta_{DH}^{n}=\frac{1}{2\left[\left(S^{2}+1\right)\sinh \frac{w}{L}+2 S\cosh \frac{w}{L}\right]}\cdot\left\{\frac{1 + S}{1+\alpha L}\left(1 - e^{-w(1+\alpha L)/L}\right)e^{w/L}-\frac{1 - S}{1-\alpha L}\left(1 - e^{w(1-\alpha L)/L}\right)e^{-w/L}\right\}\)，其中\(S = Ls/D\)（界面复合速度的归一化形式）。
9. 单异质结构（SH）从\(n\)侧提取光时的内部量子效率降低因子：\(\eta_{SH}^{n}=\frac{1}{2\left(\sinh \frac{w}{L}+S\cosh \frac{w}{L}\right)}\cdot\left\{\frac{1 + S}{1+\alpha L}\left(1 - e^{-w(1+\alpha L)/L}\right)e^{w/L}-\frac{1 - S}{1-\alpha L}\left(1 - e^{w(1-\alpha L)/L}\right)e^{-w/L}\right\}\)。
10. 双异质结构（DH）从\(p\)侧提取光时的内部量子效率降低因子：\(\eta_{DH}^{p}=\frac{1}{2\left[\left(S^{2}+1\right)\sinh \frac{w}{L}+2 S\cosh \frac{w}{L}\right]}\cdot\left\{\frac{1 - S}{1+\alpha L}\left(1 - e^{-w(1+\alpha L)/L}\right)-\frac{1 + S}{1-\alpha L}\left(1 - e^{w(1-\alpha L)/L}\right)\right\}\)。
11. 单异质结构（SH）从\(p\)侧提取光时的内部量子效率降低因子：\(\eta_{SH}^{p}=\frac{1}{2\left(\sinh \frac{w}{L}+S\cosh \frac{w}{L}\right)}\cdot\left\{\frac{1 - S}{1+\alpha L}\left(1 - e^{-w(1+\alpha L)/L}\right)-\frac{1 + S}{1-\alpha L}\left(1 - e^{w(1-\alpha L)/L}\right)\right\}\)。
12. 调制带宽相关公式：
    - 光强随调制频率变化：\(|I(\omega)|=\frac{I(0)}{\sqrt{1 + (\omega\tau_{eff})^{2}}}\)，其中\(I(0)\)是零调制频率时的光强度，\(\omega\)是角频率，\(\tau_{eff}\)是有效载流子寿命。
    - 调制带宽定义：\(\Delta f=\frac{\Delta\omega}{2\pi}=\frac{1}{2\pi\tau_{eff}}\)。
    - 假设界面复合为主导非辐射复合过程时的\(\tau_{eff}\)：\(\frac{1}{\tau_{eff}}=\frac{1}{\tau_{r}}+\frac{2s}{w}\)。
    - 辐射复合时间\(\tau_{r}\)：\(\tau_{r}=\frac{\left[\left(n_{0}+p_{0}\right)^{2}+4J/Be w\right]^{1/2}-\left(n_{0}+p_{0}\right)}{2J/ew}\)，其中\((n_{0}+p_{0})\)是热平衡时的电子和空穴浓度，\(J\)是注入电流密度，\(B\)是复合概率。
13. 功率带宽积相关公式：
    - 当界面复合和自吸收可忽略时：\(\Delta f\cdot P=\left|\frac{h\nu}{2\pi e}\right|J\cdot\frac{1}{\tau_{r}}\)，在低注入时\(\Delta f\cdot P=\left|\frac{h\nu B}{2\pi e}\right|J\left(n_{0}+p_{0}\right)\)，高注入时\(\Delta f\cdot P=\left|\frac{h\nu B}{2\pi e}\right|J\left(\frac{J}{ewB}\right)^{1/2}\)。
14. 注入电子密度公式（双注入情况）：\(\Delta n=\left(\frac{J}{ewB}\right)^{1/2}\)。
15. 过剩电子电流密度公式：\(J_{n}'=q u_{n}E N'+q D_{n}\frac{d N'}{d x}\)，其中电子迁移率\(\mu_{n}=3500cm^{2}/V\cdot s\)，\(D_{n}=\mu_{n}(kT/e)\)，电场\(E=\rho_{P}J\)，\(\rho_{P}\)是\(p\)型被动层电阻率，\(N'\)是过剩电子浓度。
16. 过剩空穴电流密度公式（计算方式与过剩电子电流密度类似，将相关参数替换为对应空穴参数）：\(J_{p}'\)（计算过程中假设空穴迁移率\(\mu_{p}=250cm^{2}/V\cdot s\)，电场\(E=\rho_{N}J\)，\(\rho_{N}\)是\(n\)型被动层电阻率）。
17. 总过剩电流密度公式：\(J'=J_{n}'+J_{p}'\)。
18. 限制因子公式：\(C=\frac{1}{1+(J'/J)}\)。

<https://github.com/basteng/Today-I-Learned/blob/main/paper/Power_and_modulation_bandwidth_of_gaAs-AlGaAs_high-radiance_LEDs_for_optical_communication_systems.pdf>

# 40. Ethernet over POF 塑料光纤以太网（Ethernet over POF）技术概述

## 一、塑料光纤（POF）的特点与应用
### （一）特点
1. **优势特性**
   - **物理特性**
     - 重量轻、坚固耐用、成本低且易于安装。
     - 可使用简单刀片切割，无需后续抛光处理。
   - **安全特性**
     - 采用650nm红光（LED），对人体完全安全。
     - 便于安装人员肉眼检测链路是否良好。
   - **抗干扰特性**
     - 完全不受电磁噪声影响，自身也不发射辐射。
     - 对视频和语音流等应用极为重要，可利用现有电源线管道布线，简化安装。
2. **与玻璃光纤的区别**
   - **材料与结构**
     - POF的芯层通常为聚甲基丙烯酸甲酯（PMMA），包层为含氟聚合物；玻璃光纤的芯层和包层为石英玻璃，且通过在芯层添加杂质来控制折射率。
     - POF芯层直径（980um）远大于单模光纤（9um）和多模光纤（50um），包层直径为1000um。
   - **性能表现**
     - POF数据速率较低（最高数百Mbps），传输距离较短（相比单模光纤和多模光纤）。
     - 成本优势明显，更耐弯折。

### （二）应用
1. **汽车领域**
   - 汽车制造商积极采用POF连接汽车信息娱乐系统及一些安全关键应用（如安全气囊）。
   - 高端汽车处理器密集，支持多种设备。
   - 90年代末制定了面向媒体的系统传输（MOST）总线协议，MOST25提供25Mbps带宽，MOST50使用POF作为物理介质，带宽可达50Mbps。
2. **家庭与办公领域**
   - POF在一些特定应用中发挥作用。
   - 在家庭网络中，其“家庭友好”特性（如可沿踢脚线和门框铺设、易切割和安全自终止）为有线连接提供理想解决方案。
   - 适用于在无线信号复杂环境下保障视频和语音服务质量。

## 二、POF与以太网
### （一）POF支持以太网的必要性
   - 以太网在办公网络下层广泛应用，且在工厂和家庭网络中逐渐占据主导地位。
   - POF若要成为铜缆网络的有力替代方案，必须支持以太网。
   - 可借助以太网的低成本、已证实的开放标准、带宽能力和服务质量（QoS）来支持三重播放（语音、视频和数据）服务，而无需重新设计独特的应用特定协议。

### （二）POF以太网实现方式
   - 市场上有多种用于在POF上提供快速以太网（100Mbps）的光纤收发器（FOT），但缺乏电气和物理接口标准。
   - 以Micrel半导体为例，其以太网多端口交换机和物理层（PHY）产品系列可与POF收发器良好适配，因其输入规格（50mV峰峰值至Vdd）范围宽，可与“任何”差分输入接口。
   - 如通过特定电路设计（AC耦合、使用可调电压基准LM4041等），可实现Micrel以太网设备与Firecomms POF收发器的接口连接，提供典型100米传输距离的快速以太网链路，与标准CAT5解决方案相当。

## 三、总结
   - POF技术在工业、办公、家庭和汽车网络中是传统玻璃光纤和铜缆的有吸引力的替代方案。
   - 具有低成本、重量轻、安装简便安全和抗电磁干扰等优点。
   - 尽管目前POF缺乏标准，但将其与以太网接口连接并非难事。
   - Micrel半导体提供多种媒体转换器以太网解决方案，支持100Base - FX网络以及传统的10Base - FL或100Base - SX应用。

# 41. MicroLED Displays Industry status and Roadmap

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/MicroLED%20Displays%20Industry%20status%20and%20Roadmap.pdf>

# 42. MicroLED 展现出神经形态计算的潜力

德国布伦瑞克，2024 年 12 月 2 日 — LED 以其节能而闻名，它还为照明以外的应用开辟了全新的可能性。布伦瑞克工业大学 (TU Braunschweig) 氮化物技术中心 (NTC) 的一个研究小组利用微型 LED 的神经元网络来实现未来的人工智能，旨在让未来的计算机更强大、更节能。

小型化、可扩展性和能源效率对于开发更强大的人工智能应用硬件至关重要。布伦瑞克工业大学的 NTC 研究小组与来自奥斯特法利亚应用科学大学和 ams OSRAM 的合作者一起，采用不同的方法使用微型 LED 技术构建计算机。研究人员正在对节能的微型 LED 进行小型化和扩展，以使神经形态计算机成为可能。

布伦瑞克工业大学半导体技术研究所的 Andreas Waag 教授表示：“我们的光学神经形态计算通过使用电子电路或光子元件模拟了生物神经网络（如人类大脑中的神经网络）的功能。”

奥斯特法利亚应用科学大学的 Christian Werner 教授表示：“这避免了传统数字计算机技术的弱点，这些弱点导致人工智能应用在大规模并行信息处理中需要大量能源。”

预计 10 年后，全球约三分之一的电能将用于超级计算机及其冷却。

氮化镓 (GaN) 是 microLED 技术的首选半导体。这种半导体在电力电子领域的应用越来越广泛，因为它比传统的硅半导体具有更高的功率密度和更好的效率。然而，与硅不同，GaN 具有光学活性，使其成为蓝色 LED 的基本构造块。布伦瑞克工业大学的氮化物技术中心 (NTC) 正在推动氮化物半导体技术的发展，将其作为微电子的第二大支柱。

研究人员将 GaN 组件与传统的硅微电子技术相结合，开辟了全新的应用领域——例如具有数十万个 microLED 的高度集成阵列，这些阵列也在 QuantumFrontiers 卓越集群和下萨克森州量子谷中使用。

“氮化镓的特殊性质非常适合尺寸为 1 微米及更小的 microLED，”Waag 说。

该研究小组还看到了基于 GaN 的 microLED 技术的巨大潜力，可以将 AI 系统造成的功耗降低 10,000 倍。microLED 执行了原本由硅晶体管执行的任务。并行内存处理与高效光子生成和检测相结合，可创建一种硬件，该硬件可物理映射不同级别的神经网络并实现并行信息流。

研究人员表示，在基于该技术的“人工大脑”成为现实之前，还需要进行大量研究，但它有望节省大量能源。NTC 研究小组已经开发出一种具有 1000 个神经元的宏观光学微型 LED 演示器。该演示器已经通过了标准的 AI 模式识别测试：它可以识别以混乱方式书写的从 0 到 9 的数字，其中一些数字人类很难辨认。

这项研究发表在《物理光子学杂志》（www.doi.org/10.1088/2515-7647/ad8615）上。

<https://iopscience.iop.org/article/10.1088/2515-7647/ad8615#fnref-jpphotonad8615bib6>

# 43. 850nm超结构单横模VCSEL芯片，助力短距离高速光通信 - 常瑞华团队

人工智能大模型的基础设施建设迫切需要单通道100Gbps及更高传输速率的数据互联技术。传统的多模VCSEL+多模光纤技术，凭借低功耗和高性价比，已广泛应用于数据中心和智算中心的短距离光互连，但其受限于激光器的色度色散和光纤中的模式色散，该方案存在信道的速率和传输距离的瓶颈问题。相比之下，单横模VCSEL与单模光纤的组合可以从根本上解决传输瓶颈问题，是更高效且更具成本优势的传输方案。近日，清华大学常瑞华院士团队提出一种基于啁啾高对比度超结构（chirped High-Contrast Metastructure, chirped HCM）的850nm单横模垂直腔面发射激光器（VCSEL）芯片，实现了106 Gbps PAM4传输速率。该设计提出chirped HCM作为VCSEL的顶部反射镜（图1），通过在chirped HCM反射镜中引入了横向渐变的反射率，使其能够与激光的基模强度分布更好地匹配，从而有效抑制高阶模式，最终实现高质量、稳定的单横模激光输出。这一设计与传统多层分布式布拉格反射镜（DBR）相比，不仅具备优异性能，而且简化了制造工艺，非常适合量产。

表 1将我们的啁啾 HCM VCSEL 与近年来报道的其他 850 nm 单模 VCSEL 进行了比较。我们的设计具有几个明显的优势。首先，我们的 VCSEL 具有更大的 6 µm 光学孔径 (OA)，可确保更高的可靠性，因为较小的 OA 容易出现诸如静电放电 (ESD) 电阻降低和长期稳定性降低等问题。此外，我们的设备实现了更高的数据速率，在 PAM4 调制下达到 106 Gbps，优于其他方法。此外，与其他一些实现单模操作的方法相比，我们的制造工艺要简单得多。光刻定义的啁啾 HCM 可实现高效的大规模生产，使其非常适合工业实施和批量生产，而无需复杂的再生长或额外的处理步骤。

![](/picture/850nmVCSEL_compare.png)

<https://mp.weixin.qq.com/s/Xk4kGUyjGVuaCo_MGsQVeg>

论文链接

<https://opg.optica.org/optica/fulltext.cfm?uri=optica-11-11-1567&id=563444>

<https://github.com/basteng/Today-I-Learned/blob/main/paper/optica-11-11-1567.pdf>

# 44. 片间光互连发展态势分析 - 信通院 刘璐团队

本文通过对数据中心和计算中心场景下片间光互连技术的研究，展示了 CPO 和 OIO 技术的发展情况，包括技术优势、产业现状和标准建立等方面。强调了片间光互连虽有进展，但面临挑战，需技术、产业和标准协同发展，以满足高带宽、低延迟和高能效的要求，推动其在多领域的应用。

<https://mp.weixin.qq.com/s/gmio2UcQUwfsTxmMSxQ14g>

光通信研究

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/Analysis%20of%20the%20Development%20Trend%20of%20Inter-Chip%20Optical%20Interconnection.pdf>

片上与片间光互连技术与产业分析 - 通信世界

随着各行业数字化转型进度加快，5G、人工智能等新技术迅速普及应用，算力需求快速增长。一年来，ChatGPT为代表的大模型开发和应用取得巨大进展，带动算力需求进一步提升。在数据中心与高性能计算中心高速发展的同时，互连技术也需要随之升级演进，以满足数据传输的大带宽、低时延、低能耗等要求。相比于电信号，光信号具有传输带宽大、传输损耗小、抗干扰能力强、可高速无串扰并行传输等诸多优势，因此光互连成为通信发展的重要技术方向，如何发展片上与片间光互连以突破传统电互连瓶颈，成为当前的研究热点之一。

  片上光互连

  大规模集成易引发信号传输瓶颈问题，其解决思路之一是使用片上光互连代替电互连，数据传输由芯片上的光波导链路实现。相较于电，光传输损耗小、带宽大，片上光互连可以支撑实现大量长距离通道，若扩展到整个晶圆，则可实现晶圆级光互连网络。

  片上光互连的核心是光电子集成芯片

  光电子集成芯片由集成在同一块衬底上多种不同功能的有源器件和无源器件构成，通过光波导进行互连通信，进而实现具有特定功能的片上光学互连处理。激光器、调制器和探测器是光互连系统的核心集成器件，可分别采用波分复用、偏振复用及模分复用技术提高片上光互连的传输容量。目前，针对单一物理维度光信号的复用、解复用器件已经较为成熟。而多种复用方式的综合运用，如波长-偏振-模式混合复用等，可进一步提高片上光互连系统的通道数量和传输容量，这也是片上光互连的重要发展趋势。此外，选择和设计合适的片上拓扑结构对性能提升也具有重要意义。片上光互连架构不仅决定着片上网络中不同节点的互连方式，同时也影响路由器的端口和网络链路数量，进而影响网络的时延、功耗和可靠性等性能。

  片上光互连尚处于研究阶段

  美国加州伯克利大学于2015年制造出一种片上微处理器，使用光实现处理单元与存储单元之间的双向互连通信，每个方向可提供2.5Gbit/s带宽，这一成果具有重要意义。Intel也进行了针对性研究，并在2020年研究院活动上展示了其在微环调制器、全硅探测器、集成半导体光放大器、集成多波长激光器等光互连核心器件方面的重要进展。曦智科技于2022年在“第二届高性能芯粒与互连架构国际研讨会”上，介绍其实现了硅光芯片和CMOS电芯片的垂直封装，由光波导替代铜导线，形成片上光网络进行数据传输。该系统的通道数为512，单通道频率4GHz，片上总带宽2Tbit/s。实测数据显示，该计算系统能在1ns内完成多个计算核之间“All-to-All”的数据广播，这将大幅提高每个计算核的算力利用率。

  片间光互连通

  常情况下，光电合封（C P O，C o-p a c k a g e d Op tics）面向大型以太网网络交换机，交换芯片与光芯片封装在一起，与外部其他芯片之间形成光互连；而光I/O（Optical I/O）面向分布式计算系统，计算芯片与光芯片封装在一起，与外部其他芯片之间形成光互连。本文将这两种形态统称为片间光互连。

  CPO：解决数据中心网络中交换芯片与光芯片之间的互连问题

  CPO通过将光引擎放置在靠近主机ASIC的位置，最大程度地减少高速电通道损耗和阻抗不连续性，从而实现更高速度、更低功耗的I/O驱动。CPO相较于可插拔光模块，带宽密度提升一个数量级，能量效率优化40%以上。

  目前报导的CPO光引擎技术方案主要为VCSEL阵列方案和硅光集成方案。然而，伴随着VCSEL调制速率的提升，芯片可靠性下降，在56GBaud速率尚没有稳定可靠的大规模集成VCSEL阵列，因此基于VCSEL阵列方案的多路并行光互连研究大幅减少。硅光集成技术在近年来成为CPO光引擎的主要方案。硅光不需要气密封装，CMOS兼容更易与电芯片集成，且硅光调制器和探测器均可支持56GBaud以上速率。

  当前CPO技术主要由交换机与光模块公司在推进，C P O样机在近三年相继发布。在“O F C 2 0 2 0”会议上，In tel推出首款CPO样机，由1.6Tbi t/s的硅光引擎与12.8Tbi t/s的可编程以太网交换机集成。在“OFC 2021会议”上，Ranovus发布了Odin品牌模拟驱动CPO 2.0架构。在“OFC 2022会议”上，Mar vell展示了其首款CPO样机，带宽为1.6Tbit/s；Ranovus基于AMD的Xilinx计算加速平台进行CPO 2.0的联合展示。在“OFC 2023”上，Broadcom和Marvell分别发布了51.2Tbit/s的交换芯片。总体来看，终端用户、设备制造商以及光器件供应商均涉足其中，形成了初步的产业生态。

  据Yole预测，CPO市场将从2022年的600万美元增长到2033年的2.87亿美元。CPO数据中心市场于2022年正式起步，出货将以800Gbit/s和1.6Tbit/s端口为主，到2027年CPO端口将占近30%。CPO需要高度集成的光学以及硅芯片技术，难度较大，从可插拔到CPO的转换对企业研发实力提出较高要求，当前CPO产业链包含设计、光引擎供应商、激光器供应商、交换机厂商、硅光代工厂、设备商等。

  2020年，业界开始对发展CPO标准形成共识。标准进展与技术和产业进展密切相关，美国、中国及欧盟率先开展标准化工作。光互连论坛（OIF）、板载光学联盟（COBO）、联合开发基金会（JDF）、国际光电委员会（IPEC）、中国计算机互连技术联盟（CCITA）等标准组织均针对CPO作出了一系列部署。

  光I/O：解决计算芯片CPU、GPU、XPU等之间的互连问题

  光I/O利用光具有的低功耗、高带宽、低延迟等优势，取代传统的电I/O方案，芯片输入输出的为光信号，进而构建分布式计算网络。在相同能效情况下，光I/O的边带宽密度与UCle、NVlink、PCIe等电互连相当，但传输距离远超电互连。

  光I/O需要物理层和互连协议多重创新。在物理层方面，对于CPU而言，通用的对外通信通过PCIe协议实现。目前，数据中心内的光互连解决方案绝大部分针对以太网设计，基于PCIe的光互连解决方案几乎处于空白状态。相比于以太网，<font color=red>PCIe信号的通道数较多，单通道带宽较小，调制方法不同，对延迟的容忍度相对较小</font>。因此，基于以太网的光互连方案无法直接套用到PCIe应用场景，需要重新定义和设计。PCI-SIG于2023年8月宣布成立PCIe光学工作组，其职责是致力于通过光学接口实现PCIe。

  在协议层方面，当前主流的分布式计算主要使用基于以太网的软硬件生态系统，而这一系统存在诸多的提升空间。目前基于以太网的方案需要使用内存屏障甚至软件设定临界区，导致性能开销大、延迟长，在复杂的控制流程之下甚至会出现“死锁”。相比以太网协议，CXL（Compute Express Link）协议提供了高效的数据同步，可大大降低软件管理的复杂度，降低CPU处理网络功能开销。

  目前各大芯片巨头均已在光I/O领域进行布局，其中包括Intel、AMD、NVIDIA等。Intel已经与Ayar Labs合作多年，多次在OFC上展示其FPGA芯片间通过光I/O实现信号互连的阶段性进展。AMD通过收购Xilinx，整合了其硅光团队，在“ISSCC 2023”展示了其初步的进展。NVIDIA与Ayar Labs展开合作，其内部也有自己的硅光团队开发相关技术。Ayar Labs在光I/O方面具有较强实力，与多位伙伴积极合作，其在“OFC 2023”上展示的TeraPHY可以实现双向4.096Tbit/s数据传输。据Yole预测，光I/O市场将从2022年的500万美元增长到2033年的23亿美元。

  由于面向不同应用场景，两种片间光互连的性能存在较大差异。从带宽和能效角度来看，根据Intel数据，单个CPO模块的带宽为1.6~3.2Tbi t/s，带宽密度为50~200Gbi t/(s·mm)，能效为15pJ/bit；而光I/O的总带宽为40Tbit/s，带宽密度为5Tbit/(s·mm)，能效为3pJ/bit。Ayar Labs数据显示，同样能效情况下，光I/O的边带宽密度比CPO的大一个数量级。从延迟角度来看，根据Ayar Labs数据，光I/O的延迟在5ns左右，对应的误码率为1e-15，而CPO为了达到相同的误码率，需要使用FEC技术，其延迟在100~150ns。整体上看，光I/O比CPO的性能要求更高。

  总结展望

  片上光互连的核心是光电子集成芯片，当前处于研究阶段。CPO的研究聚焦51.2Tbit/s交换机，产业化与标准化进程已经启动。光I/O特别适用于计算结构，当前已有产品小批量出货，未来仍需物理层和互连协议进一步创新。无论片上还是片间光互连仍有许多亟待解决的关键问题，如生态尚不成熟、功能选择较少、编程模型缺乏业界共识、可靠性存挑战，以及面临相干、线性驱动可插拔等其他技术挤压等，需要业界的积极探索与合作，共建完善的技术、产业与标准生态。

<http://www.iccsz.com/site/cn/News/2023/10/29/20231029140847063209.htm>

# 45. 微软：基于Micro-LED＋CIS的模拟光学计算实现加速计算

  微软剑桥研究院在今年8月底的一个视频及讲了他们新一代的模拟光学计算机，感觉还挺巧妙的，采用了MicroLED阵列＋投影芯片＋标准的CMOS图像传感器，实现了机器学习推理和复杂优化问题的加速计算(视频：https://youtu.be/gdJYMoZMKIY?si=Zil0EMYvVitWMTyw)。

◆研究背景

      人工智能的可持续性是最重要的问题之一。不幸的是，这个问题出现的时机再糟糕不过了。就在计算机需求急剧增长的时候，数字计算的未来趋势却不容乐观，摩尔定律正在放缓。这并非只是微软的看法，而是整个行业广泛担忧的问题。
      在过去的五六年里，这已经引发了大量的研究与开发工作。许多公司以及初创企业都已经利用模拟技术这一广泛的技术类别制造出了非传统计算机。在这样的背景下，微软也在几年前开始了模拟光学计算的研究之旅。

◆ 模拟光学计算(AOC)      

首先微软团队指出，他们所开发的模拟光学计算机并不是针对通用计算，而且主要用于它加速两类不同但应用范围很广的任务：机器学习推理以及复杂优化问题。      在机器学习推理方面，已经能够展示利用这台计算机加速扩散模型的潜力，扩散模型可用于生成图像及其他内容。实际上，有一些新兴的机器学习形式能够真正利用它所提供的强大计算能力，并实现高级特性，比如对分布外数据有更好的泛化能力。      其次，同一台计算机还能够解决硬优化或组合优化等复杂问题。目前已经从众多行业领域，比如医疗保健、金融、化学工程以及机器人技术领域，确定了一些现实世界中的问题，这些问题都可以通过这台计算机来加速解决。正是同一台计算机，能够支持各种各样的应用。      去年，微软团队研制出了第一代计算机。它是采用较为笨重的技术制造的，但已经能够解决巴克莱银行提出的一个现实世界金融问题的简化版本，并且表现优于量子计算机。

这促成了团队与巴克莱银行的进一步深度研究合作，以及与微软健康未来团队的合作关系。目前团队已经完成了第二代计算机的研制。它的物理尺寸要小得多，而且在世界上首次展示了同一台计算机能够同时解决复杂优化问题并加速机器学习推理。

展望未来，研究者预计在大规模应用的情况下，这台计算机能够实现450 TOPS/Watt(Int8精度)的算力/能效，相较于最先进的GPU，这是100倍的性能提升。

◆ 原理：基于MicroLED＋滤光片＋CIS的模拟光学计算机

      利用光与物质的相互作用实现乘法和加法等基本运算。光通过部分滤光片可等效于 0 到 1 之间权重的乘法（成千上万个光束能以无源无功耗的方式大规模并行乘法），CMOS相机中多束光落在同一个像素上可等效于实现大规模并行加法。基于此可实现向量矩阵乘法器，利用光学固有的并行性构建大规模并行脉动向量矩阵乘法器，其输入向量采用micro LED（显示领域的新兴技术），中间矩阵采用数字投影仪中的芯片，输出向量采用智能手机相机中的标准 CMOS 传感器，并且通过 CMOS 芯片实现非线性、归一化等功能，这种将光学与模拟电子学结合的方式被称为“模拟光学计算”（AOC）。

◆ 基础演示 

1. 机器学习推理      

以 MNIST 分类为例，先在 GPU 上训练模型，再编码到投影仪上，可以看到计算机能够实时且以非常高的准确率对这些数字进行分类。但这里更重要的是，计算机的运算结果与仿真平台（数字孪生）所预测的完全一致。

2. 复杂优化问题      
   
同一台计算机也能够成功解决硬优化问题。举第二个例子，首先将一个优化问题编码到了同一台投影仪上。在这些图表中，100%的成功率意味着每次都能正确地解决问题。当把手放在其中一台投影仪前面挡住了光路，计算机就失去了对要解决问题的追踪。结果就是，它会尝试随机地去解决问题，成功率就降到了零。一旦我把手移开，计算机就重新理解了它正在解决的问题，然后成功率又恢复到了100%。

◆ 应用场景展望      

展望未来，在构建未来大规模版本的计算机时，与应用协同设计是至关重要的，这样才能真正发挥计算机的优势，并弥补它的不足。例如，噪声一直以来都是模拟计算机面临的主要历史性挑战。幸运的是，机器学习模型相对来说更能适应有噪声的计算机。对于一些模型，比如扩散模型，噪声实际上可以成为朋友而非敌人。      

像Bing和Copilot中使用的扩散模型，其工作原理如下：首先有训练图像，然后随着时间推移，不断向它们添加噪声，直到最后只剩下完全的噪声。在推理阶段，运行反向去噪过程，从完全的噪声开始，然后最终生成一幅看起来干净的图像，比如这里生成了一只狗的图像。重要的是，这个反向过程本质上是迭代的。它在计算上很耗费资源，并且需要去噪。所有这些要求都与我们的计算机完美契合。

微软团队已经利用数字孪生实现了一个非常小版本的此类模型，用于生成MNIST数字图像，而且打算很快就在计算机上运行它。随着后续增大模型的规模，就能够生成更高级的图像，比如时尚MNIST图像、密码图像等等。

      值得一提的是，扩散模型只是具有这种反馈特性、适合模拟计算的更广泛的机器学习模型类别中的一个例子。其他的还包括深度平衡模型、神经常微分方程（Neural ODEs），甚至一些最新的模型，比如流匹配（flow matching）和状态空间模型（state space model），似乎也适用于模拟计算机。
      同样的协同设计理念对于优化问题来说也很关键。以医疗保健领域的核磁共振（MRI）扫描为例。如果能把MRI扫描时间从20到40分钟减少到不到5分钟，这对于患者的体验以及治疗方式会产生非常大的影响。

      这里涉及的数学原理其实已经有15年历史了，叫做压缩感知。其原理是，当患者在扫描仪内时，对图像进行欠采样——或者更准确地说，是对自由空间中的扫描进行欠采样——然后通过求解一个硬优化问题来实现高保真度恢复图像。由于这个问题在计算上很困难，所以一直没能得到应用，但微软团队已经能够将这个优化问题映射到他们计算机的运算模式中，他们认为能够将MRI扫描的速度提高4到8倍，同时实现高保真重建，有可能将扫描时间减少到仅仅5分钟。       

(个人总结：模拟光学计算现在好火，换汤不换药的论文很多。硬件技术路线分成空间光和集成光两条。集成光路线的损耗/运算规模是一个比较大的问题，但未来也可以通过先进工艺和异质集成不断优化(台积电的集成光计算芯片)。而微软包括一些初创企业比如Lumai等走的是自由空间的路线，微软的特色在于用了低成本的microLED和CIS来搭建系统，在并行度规模、成本、功耗上相比通信波段的激光器/PD阵列都还是有优势的，速度是劣势。另外一点就是微软提到的需要找到特定的场景应用(噪声、计算精度不敏感)以及专用算法，进行协同设计优化，才能够在这个特定场景下发挥光计算的价值)

<https://mp.weixin.qq.com/s/ciTpYIaff8_LVrsLmzwruA>

## 45.1 arXiv上的论文

Analog Iterative Machine (AIM): using light to solve quadratic optimization problems with mixed variables










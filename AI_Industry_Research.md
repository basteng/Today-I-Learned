- [1. 半导体技术不断发展以满足生成式人工智能的需求](#1-半导体技术不断发展以满足生成式人工智能的需求)
  - [1.1 HBM4 将如何发展？](#11-hbm4-将如何发展)
  - [1.2 封装趋势转向玻璃基板和小芯片](#12-封装趋势转向玻璃基板和小芯片)
- [2. AI市场格局](#2-ai市场格局)
  - [2.1 生成式AI头部企业市场份额](#21-生成式ai头部企业市场份额)
- [3. 数据中心AI芯片路线图](#3-数据中心ai芯片路线图)
- [4. Marvell](#4-marvell)
  - [4.1 Accelerated Infrastructure for the AI Era 2024.04](#41-accelerated-infrastructure-for-the-ai-era-202404)
- [5. 高盛：AI未来的四大巨头](#5-高盛ai未来的四大巨头)
- [6. AI数据中心价值链](#6-ai数据中心价值链)
- [7. AI芯片供应链](#7-ai芯片供应链)
- [8. Nvidia](#8-nvidia)
  - [8.1 NVLink](#81-nvlink)

<div STYLE="page-break-after: always;"></div>

# 1. 半导体技术不断发展以满足生成式人工智能的需求

## 1.1 HBM4 将如何发展？   
生成式人工智能和高性能计算 (HPC) 正在推动数据中心动态随机存取存储器 (DRAM) 需求的增长。

![image1](/picture/img_gen-ai-hbm-product-development_yint_july-2024-1-1024x662.jpg)

Yole Group 预测，2023 年至 2029 年间，高带宽存储器 (HBM) 的出货量将增长约 48%，HBM 在 DRAM 市场的份额将从 2023 年的 2% 左右上升至 6% 以上。

Yole Group 的拆解显示，NVIDIA 在其 Hopper Tensor Core H100 GPU 中引入了一种创新设计，该设计使用 HBM3，提供比其前身 A100 多两倍的 DRAM 带宽。该 GPU 与 Grace CPU 配对，使用 NVIDIA 的超高速芯片间互连，提供 900GB/s 的带宽，为 HPC、AI 和游戏市场运行 TB 级数据的应用程序提供高达 10 倍的性能。

HBM 目前掌握在三家主要厂商手中——SK 海力士、三星和美光。SK 海力士很可能在 2026 年率先推出 HBM4，但是否会使用混合键合仍有待观察。下一代混合键合可使用更小的连接来实现更密集的堆栈。

## 1.2 封装趋势转向玻璃基板和小芯片
目前AI加速器的平均基板尺寸约为70*70mm²，下一代产品有望向更大的尺寸发展，但当尺寸达到100*100mm²时，这一趋势就开始受到限制，超过这个限制，良率就会急剧下降。

并非所有当前的 AI 加速器都使用最大层数，但下一代产品预计将迅速采用更高的层数，以应对信号布线和电力传输挑战以及增大的尺寸。
![image2](/picture/img_high_end_performance_packaging_all-platforms_yg_july2024-1-1024x662.jpg)


提高可扩展性的一种方法是采用玻璃作为新的核心材料，将先进基板提升到一个新的水平。玻璃芯基板可以提供更小的 L/S、更少的层数和卓越的热导率，使其成为解决热管理问题的有希望的候选者。

![image3](/picture/img-status-of-the-advanced-ic-substrates-industry_option-for-datacenters_yint_july2024-1-1024x662.jpg)

Yole Group 预计，随着制造商寻求优化成本和性能，芯片组方法将在未来占据主导地位。芯片组支持分解，因此片上系统 (SoC) 单片芯片被划分为具有不同功能的较小芯片，然后在同一封装中互连。芯片组还允许复制，因此两个或多个 SoC 单片芯片可以在同一封装中互连以形成更大的 SoC。

<https://www.yolegroup.com/strategy-insights/semiconductor-technologies-evolving-to-meet-generative-ai-demand/>

# 2. AI市场格局

## 2.1 生成式AI头部企业市场份额

![image](picture/AI-market%202023.png)

<https://seekingalpha.com/article/4714331-intel-stock-debt-burden-far-from-competitive-sell>

# 3. 数据中心AI芯片路线图

这份 话题标签#datacenter 话题标签#AI 话题标签#chip 路线图显示，英伟达 将在 2027 年及以后💡占据主导地位。该数据中心 AI 芯片路线图显示，NVIDIA 在 AI 话题标签#GPU 业务中占据主导地位：直到 2027 年配备 576GB 话题标签#HBM4 内存的 Rubin Ultra AI GPU！

在最近分享的数据中心 AI 芯片路线图中 X 上发布，TweakTown 很好地了解了公司已经在市场上拥有的产品，以及到 2027 年的 AI 芯片管道中有哪些。看看吧：

该名单包括 话题标签#NVIDIA 、AMD 、英特尔 、谷歌 、亚马逊 、微软 、Meta 、字节跳动 和 华为 的芯片制造商。您可以查看 NVIDIA AI GPU 列表，包括 Ampere A100 到 Hopper H100、GH200、H200 AI GPU，以及 Blackwell B200A、B200 Ultra、GB200 Ultra 和 GB200A。但在那之后 - 我们都知道即将到来 - 是 Rubin 和 Rubin Ultra，两者都是下一代 HBM4 话题标签#memory 。

非常感谢 Anthony Garreffa 和 TweakTown 通过下面的💡🙏👇链接提供完整文章，其中包含更多背景和见解
<https://www.tweaktown.com/news/100151/this-data-center-ai-chip-roadmap-shows-nvidia-will-dominate-far-into-2027-and-beyond/index.html>

![image](/picture/AI%20datacenter.jpg)

# 4. Marvell

## 4.1 Accelerated Infrastructure for the AI Era 2024.04

<https://www.marvell.com/company/events/ai-era-event.html>

<https://github.com/basteng/Today-I-Learned/blob/main/Research%20Report/marvell-accelerated-infrastructure-for-the-ai-era-event.pdf>

# 5. 高盛：AI未来的四大巨头

**听起来你是说这是一个赢家通吃的市场。这是否像互联网的发展一样，会有一个主导者，就像我们在搜索或电子邮件平台中看到的那样？**

**布鲁克·戴恩**： 这又是一个大话题。

**Sung Cho**： 我们知道不会超过四家。没有其他公司可以与之竞争。唯一能进行这种程度投资的公司是 **<font color=red>Meta、Google、OpenAI 和 Anthropic</font>**。

**Brook Dane**： 但我们目前还不知道的是：随着这些模型逐渐成熟，随着阶梯式增长的现象在某个时候出现，三年后最好的模型是否会比其他模型好很多，从而占据 80% 的市场份额？或者我们有四个非常好的模型，人们会将它们用于不同的用例、不同的领域和不同的方式？我们会有四个大规模的模型吗？

如果有四种同样强大的模型，你会认为它们很快就会商品化。而如果其中一种成为明显的主导者，那么它将产生令人难以置信的经济效益。我们还不知道答案。

但我们确实知道，这四家公司都不能放慢创新的步伐。因为如果你放慢了创新的步伐，如果你的智力停留在大学一年级学生的水平，而其他人的智力都达到博士水平，如果他们比你优秀很多，而且他们的效率和成本曲线下降得比你快，那么你可能很难获得市场。

**Sung Cho**： 我认为随着时间的推移，将会出现垂直专家。因此，我认为除了速度和智力之外，竞争还在于：我们如何才能为特定子行业和用例构建更高效的模型？

**高盛研究部的同事曾表示，人工智能有利于 大型科技公司。今天我也听到了您同样的说法。您认为有什么可以挑战这一说法的吗？** 

**Sung Cho**： <font color=red>从基础设施的角度来看，竞赛基本已经结束</font>。

<font color=red>但在构建垂直和行业特定的 LLM 和模型以及许多边缘用例方面，我认为这还没有解决，而且我认为许多创新将会在这里出现</font>。

**布鲁克·丹恩**： 我想补充的是，我认为这个市场不仅仅是少数几家超级大盘股赢家。本质上，除了模型训练部分之外，最重要的是：你拥有哪些独特的数据，可以用来帮助客户？

因此，在软件层，我们真正寻找的是拥有深度专有数据的公司，可以使用这些数据来创建差异化的用例和体验。

但从投资机会的角度来看，这主要是公开市场现象。不会出现大量私营公司来颠覆这些行业的结构。

**总结一下：您从这项研究中获得的最大收获是什么？**

**Sung Cho**： 我的主要观点与半导体有关。英伟达显然在近两年来一直主导着人工智能芯片领域。但现在，真正的替代品即将进入市场。我认为，英伟达是否会继续保持 100% 的市场份额，还是会开始将部分市场份额让给其他公司，这是一个真正的争论。我们开始相信，未来几年，除了英伟达之外，还会有其他受益者。

**布鲁克·戴恩**： 我的主要看法是，我们正处于一场非常深刻、影响巨大的技术转型的早期阶段，我们有信心，这些模型的状态以及它们未来的发展将推动我们一直思考和希望实现的结构性变化。

我们越来越有信心，这个技术周期是真实的。正如人们所说，它将会是一个巨大的进步。

<https://www.goldmansachs.com/insights/articles/will-the-1-trillion-of-generative-ai-investment-pay-off>

# 6. AI数据中心价值链

AI 数据中心的扩建是历史上最大的计算基础设施扩建之一。

在过去的四个季度中，仅 Microsoft、Amazon、Google 和 Meta 就看到了 $150B+ 的资本支出。

随着数千亿美元流经生态系统，供应链在堆栈的每一层都捉襟见肘。

从能源到建筑再到半导体，公司都有机会解决这些瓶颈。

![](/picture/1728999063008.jpg)

# 7. AI芯片供应链

4 大公司垄断 AI 芯片供应链

1. Nvidia：AI 芯片的架构师（80-95% 的市场份额）
Nvidia 处于 AI 芯片设计的前沿，该公司以其图形处理单元 （GPU） 而闻名，在 AI 加速中得到了广泛的应用。

据估计，Nvidia 的市场份额从 80% 到 95% 不等，在 AI 芯片架构领域占据主导地位。此外，其 GPU 采用针对 AI 任务优化的专用内核量身定制，已成为许多 AI 应用程序的事实标准。这包括从深度学习到科学计算。

2. ASML：先进半导体制造（100% 市场份额）
在半导体光刻领域，ASML 占据主导地位。作为先进节点尖端光刻设备的唯一供应商，ASML 拥有惊人的 100% 市场份额。

此外，其技术对于制造现代 AI 芯片的复杂设计是必不可少的，使制造商能够突破性能和效率的界限。

3. 台积电：打造 AI 芯片的未来（90% 的市场份额）
TSMC 是世界领先的半导体代工厂。该公司在先进芯片制造方面拥有约 90% 的市场份额。

此外，台积电的先进制造工艺能够以前所未有的效率和规模生产高性能 AI 芯片。

4. Amazon Web Services （AWS）：为 AI 计算提供支持（32% 的市场份额）
在云计算领域，Amazon Web Services （AWS） 是一股主导力量。该公司提供 AI 应用程序所必需的基础设施和计算资源。

AWS 拥有 32% 的可观市场份额，可提供训练和推理任务所需的计算能力。该公司促进了 AI 解决方案的大规模部署。

![](/picture/AI_Semiconductor_Ecosystem.jpg)

# 8. Nvidia

## 8.1 NVLink

想象一下，你有一群人在做一个巨大的谜题。如果他们不能快速地相互交谈或有效地分享作品，他们将难以取得进展。话题标签#NVLink 就像给这些人提供具有即时通信和超快速共享功能的对讲机。在计算方面，NVLink 为 GPU 执行此操作！

什么是 NVLink？
NVLink 是 NVIDIA 开发的一种高速连接技术。它使多个 GPU（图形处理单元）能够比 话题标签#PCIExpress 等传统技术更快地相互通信，后者仍在许多计算机中使用。从本质上讲，NVLink 将单个 GPU 变成了一个可以无缝协作的“超级团队”。

为什么 NVLink 很重要？
在 NVIDIA 的 Blackwell 系统 （https://lnkd.in/gtu-f-6E） 中，可以使用 NVLink 互连 144 个 GPU。这种大规模的互连性使所有 GPU 都可以作为一个统一的系统运行。数据毫不费力地流动，延迟最小，可以更快、更高效地完成大型任务，例如训练 AI 模型。

好处
处理大数据：在 AI 等任务中，数据在 GPU 之间不断移动。如果通信速度慢，系统就会陷入困境。使用 NVLink，数据移动速度更快，使一切保持同步。

生成式 AI：创建新图像或生成类似人类的文本等应用程序需要同时进行大量计算。借助 NVLink，所有涉及的 GPU 都可以协同工作而不会降低速度。

扩大规模：需要更多功能？NVLink 允许轻松添加更多 GPU，并且它们都可以有效地相互“对话”。这种可扩展性对于不断增长的 AI 工作负载至关重要。

更大的图景
虽然 NVLink 乍一看似乎只是一个更快的连接，但它是一项基础技术，允许像 Blackwell 这样的大型 AI 系统作为一台超级强大的智能机器运行。通过保持 GPU 连接和数据平稳移动，NVLink 成为推动 AI 未来发展的关键部分。

🚀 下次当您考虑复杂的 AI 应用程序或大型数据处理任务时，请记住，NVLink 等技术是实现这些惊人突破的原因。

![](/picture/NVLink.gif)

<https://www.linkedin.com/posts/chandan-h-p-271b61108_nvidia-nvlink-pciexpress-activity-7261365061510717441-lN3M?utm_source=share&utm_medium=member_desktop>
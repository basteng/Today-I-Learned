# 1.变的是数据来源，没变的是数据质量 （by orange.ai）
[链接](https://x.com/oran_ge/status/1815552616979702174)

需求一直在那里，但是一直没被满足好。

以前的数据散落在各处，就像大众点评找餐厅，我们通过搜索引擎获得了一些坐标，并前往去寻找。

现在的数据则被汇聚到了模型里，就像一个中央厨房，我们可以随时打上一句招呼，它就端菜上桌，任君食用。

但是预制菜嘛，就是不太新鲜，所以我们做了RAG，做了AI搜索，获取新鲜的实时信息。

大到金融、医疗，小到生活百科，我们的需求一直是高质量的数据，高质量的信息。

但需求从未被满足。

不管是模型训练的数据、SFT的数据，还是RAG的数据，质量都是第一性原理。

好数据出好结果，没有捷径，从未变过。

前几天和一位前同事吃饭，他说了一句金句：

最近的AI资讯其实是噪音。

原因是因为AI技术的进展很小，可用性也不高，关注这样的资讯，反而不如花时间深度思考和积极行动。

这句话获得了很多人的共鸣。

本质是因为每个人所需要的好数据也是不同的。

自己不需要的信息，其实就是噪音。

人们需要的从来不是那么多信息，而是自己关心的信息。

如果AI对你的兴趣有足够多足够深的了解，就会成为让推荐算法更强的推荐引擎。

需求如山，而山，一直在那里。

---

# 2.colab里如何运行nanoGPT

首先设置GPU
修改 - 笔记本设置 - 硬件加速器 T4 GPU

```
!git clone https://github.com/karpathy/nanoGPT

!pip install tiktoken transformers

!cd ./nanoGPT/data/shakespeare/ && python prepare.py

!cd ./nanoGPT/ && python train.py --dtype=float16 --dataset=shakespeare --block_size=64 --batch_size=8 --n_layer=4 --n_head=4 --n_embd=64 --max_iters=1 --eval_interval=1 --init_from=gpt2

!cd ./nanoGPT && python sample.py --dtype=float16 --num_samples=5 --max_new_tokens=10 --start="foolish pig"
```

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
训练：在 shakespere 数据集上微调 GPT
python train.py --dtype=float16 --dataset=shakespeare --compile=False --n_layer=4 --n_head=4 --n_embd=64 --block_size=64 --batch_size=8 --init_from=gpt2 --eval_interval=100 --eval_iters=100 --max_iters=300 --bias=True

train.py论点解释：

colab GPU 不支持默认 bfloat16
--dtype=float16
colab 目前使用 PyTorch 1.13.1+cu116，但编译需要 PyTorch 2.0
--compile=False
大于gpt2-mediumColab 上 RAM 耗尽的模型（12.7GB）
--init_from=gpt2-medium
“更小的 Transformer”显著加快训练速度
--n_layer=4 --n_head=4 --n_embd=64 block_size=64 --batch_size=8
每 100 次迭代保存一次模型：
--eval_interval=100
计算每 100 次迭代的 val 损失：
--eval_iters=100
300 次迭代后停止训练：
--max_iters=300
示例：查看已保存模型的输出
!cd ./nanoGPT && python sample.py --dtype=float16 --num_samples=5 --max_new_tokens=10 --start="to be"

sample.py论点解释：

单独示例输出的数量：
--num_samples=5
~ 每个示例要输出的单词数（单词 ~ 标记 x 0.75）
--max_new_tokens=10
每个输出示例都以以下内容开始：
--start="to be"


<https://github.com/eniompw/nanoGPTshakespeare>

---
# 3. 半导体技术不断发展以满足生成式人工智能的需求

1.HBM4 将如何发展？   
生成式人工智能和高性能计算 (HPC) 正在推动数据中心动态随机存取存储器 (DRAM) 需求的增长。

![image1](/picture/img_gen-ai-hbm-product-development_yint_july-2024-1-1024x662.jpg)

Yole Group 预测，2023 年至 2029 年间，高带宽存储器 (HBM) 的出货量将增长约 48%，HBM 在 DRAM 市场的份额将从 2023 年的 2% 左右上升至 6% 以上。

Yole Group 的拆解显示，NVIDIA 在其 Hopper Tensor Core H100 GPU 中引入了一种创新设计，该设计使用 HBM3，提供比其前身 A100 多两倍的 DRAM 带宽。该 GPU 与 Grace CPU 配对，使用 NVIDIA 的超高速芯片间互连，提供 900GB/s 的带宽，为 HPC、AI 和游戏市场运行 TB 级数据的应用程序提供高达 10 倍的性能。

HBM 目前掌握在三家主要厂商手中——SK 海力士、三星和美光。SK 海力士很可能在 2026 年率先推出 HBM4，但是否会使用混合键合仍有待观察。下一代混合键合可使用更小的连接来实现更密集的堆栈。

2.封装趋势转向玻璃基板和小芯片
目前AI加速器的平均基板尺寸约为70*70mm²，下一代产品有望向更大的尺寸发展，但当尺寸达到100*100mm²时，这一趋势就开始受到限制，超过这个限制，良率就会急剧下降。

并非所有当前的 AI 加速器都使用最大层数，但下一代产品预计将迅速采用更高的层数，以应对信号布线和电力传输挑战以及增大的尺寸。
![image2](/picture/img_high_end_performance_packaging_all-platforms_yg_july2024-1-1024x662.jpg)


提高可扩展性的一种方法是采用玻璃作为新的核心材料，将先进基板提升到一个新的水平。玻璃芯基板可以提供更小的 L/S、更少的层数和卓越的热导率，使其成为解决热管理问题的有希望的候选者。

![image3](/picture/img-status-of-the-advanced-ic-substrates-industry_option-for-datacenters_yint_july2024-1-1024x662.jpg)

Yole Group 预计，随着制造商寻求优化成本和性能，芯片组方法将在未来占据主导地位。芯片组支持分解，因此片上系统 (SoC) 单片芯片被划分为具有不同功能的较小芯片，然后在同一封装中互连。芯片组还允许复制，因此两个或多个 SoC 单片芯片可以在同一封装中互连以形成更大的 SoC。

<https://www.yolegroup.com/strategy-insights/semiconductor-technologies-evolving-to-meet-generative-ai-demand/>
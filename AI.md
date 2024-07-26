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

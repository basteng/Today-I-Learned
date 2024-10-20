- [1.使用Tortoisegit git管理上传文件代码到github](#1使用tortoisegit-git管理上传文件代码到github)
- [2.设置git全局代理端口](#2设置git全局代理端口)
- [3.md加目录](#3md加目录)
- [4.colab里如何运行nanoGPT](#4colab里如何运行nanogpt)
- [5. 树莓派增加定时运行的程序](#5-树莓派增加定时运行的程序)
- [6. 慧博投研](#6-慧博投研)
  - [6.1 拉取行业数据](#61-拉取行业数据)
- [7. 非工程师指南：训练 LLaMA 2 聊天机器人](#7-非工程师指南训练-llama-2-聊天机器人)

<div STYLE="page-break-after: always;"></div>

# 1.使用Tortoisegit git管理上传文件代码到github

[网页链接](https://blog.csdn.net/mao_hui_fei/article/details/118546080)

# 2.设置git全局代理端口

```
git config --global http.proxy 'socks5://127.0.0.1:1080'
git config --global https.proxy 'socks5://127.0.0.1:1080'
```

# 3.md加目录

目录功能，按 Ctrl + Shift + P 呼出任务面板，然后搜索 create table 即可

# 4.colab里如何运行nanoGPT

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

<div STYLE="page-break-after: always;"></div>

# 5. 树莓派增加定时运行的程序

```
sudo crontab -e

设置时间

sudo /etc/init.d/cron restart
```

# 6. 慧博投研

## 6.1 拉取行业数据

A股一致性预期分析系统 - 行业一致性预期，选择“半导体”

上市公司财务数据分析系统 - 定期财务报告

# 7. 非工程师指南：训练 LLaMA 2 聊天机器人

介绍
在本教程中，我们将向您展示如何构建自己的开源 ChatGPT，而无需编写任何代码！我们将使用 LLaMA 2 基础模型，使用开源指令数据集对其进行微调以进行聊天，然后将模型部署到您可以与朋友分享的聊天应用程序中。只需点击一下，我们就能实现卓越。😀

为什么这很重要？机器学习，尤其是 LLM（大型语言模型），已经见证了前所未有的普及，成为我们个人和商业生活中的重要工具。然而，对于大多数机器学习工程专业领域之外的人来说，训练和部署这些模型的复杂性似乎遥不可及。如果机器学习的预期未来是充满无处不在的个性化模型，那么未来将面临一个迫在眉睫的挑战：我们如何让那些没有技术背景的人能够独立利用这项技术？

在 Hugging Face，我们一直在默默努力为这个包容性的未来铺平道路。我们的工具套件（包括 Spaces、AutoTrain 和 Inference Endpoints 等服务）旨在让每个人都能接触到机器学习的世界。

为了展示这个民主化的未来是多么容易实现，本教程将向您展示如何使用Spaces、AutoTrain和ChatUI来构建聊天应用程序。只需三个简单的步骤，无需一行代码。作为背景介绍，我也不是 ML 工程师，而是 Hugging Face GTM 团队的成员。如果我能做到，那么你也可以！让我们开始吧！

https://huggingface.co/blog/Llama2-for-non-engineers



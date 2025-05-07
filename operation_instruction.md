- [1.使用Tortoisegit git管理上传文件代码到github](#1使用tortoisegit-git管理上传文件代码到github)
- [2.设置git全局代理端口](#2设置git全局代理端口)
- [3.md加目录](#3md加目录)
- [4.colab里如何运行nanoGPT](#4colab里如何运行nanogpt)
- [5. 树莓派增加定时运行的程序](#5-树莓派增加定时运行的程序)
- [6. 慧博投研](#6-慧博投研)
  - [6.1 拉取行业数据](#61-拉取行业数据)
  - [6.2 GDP预测](#62-gdp预测)
- [7. 非工程师指南：训练 LLaMA 2 聊天机器人](#7-非工程师指南训练-llama-2-聊天机器人)
- [8. 推荐好用的SS/V2RAY/TROJAN机场](#8-推荐好用的ssv2raytrojan机场)
- [9. 海外手机卡](#9-海外手机卡)
  - [9.1 Giffgaff激活事项](#91-giffgaff激活事项)
- [10. 树莓派科学上网](#10-树莓派科学上网)
  - [10.1 简单方式 - raspberry\_pi\_shadowsocks](#101-简单方式---raspberry_pi_shadowsocks)
    - [本文为使用 python 版本的 shadowsocks 客户端来实现科学上网](#本文为使用-python-版本的-shadowsocks-客户端来实现科学上网)
    - [raspberry\_shadowsocks.sh](#raspberry_shadowsockssh)
    - [配置 chromium/firefox SwitchOmega](#配置-chromiumfirefox-switchomega)
  - [10.2 稍微复杂一点方式 - shadowsocks-for-raspberry](#102-稍微复杂一点方式---shadowsocks-for-raspberry)
    - [安装shadowsocks](#安装shadowsocks)
    - [安装SwitchyOmega](#安装switchyomega)
    - [安装privoxy](#安装privoxy)
- [11. SSR 导入](#11-ssr-导入)
- [12. Transformer by hand - Full Stack in Excel](#12-transformer-by-hand---full-stack-in-excel)
- [13. 模拟电路设计 - JKU 举办的中级 MOSFET模拟电路设计课程](#13-模拟电路设计---jku-举办的中级-mosfet模拟电路设计课程)
- [14. MOSbius 芯片 - 集成电路课程中为学生提供连接测量、仿真和分析的动手实验](#14-mosbius-芯片---集成电路课程中为学生提供连接测量仿真和分析的动手实验)
- [15.  Jetson Orin Nano Super](#15--jetson-orin-nano-super)
- [16. duino-coin - Arduino/Raspberry 可以挖矿](#16-duino-coin---arduinoraspberry-可以挖矿)
- [17. 8bit复古计算机](#17-8bit复古计算机)
- [18. github不能上传大文件 - 大于100M不可以](#18-github不能上传大文件---大于100m不可以)
- [19. iPad 连接Raspberry Pi低延迟编程](#19-ipad-连接raspberry-pi低延迟编程)
- [20. N26开卡](#20-n26开卡)
- [21. Deepseek + Kimi 生成ppt](#21-deepseek--kimi-生成ppt)
- [22. 视频转gif](#22-视频转gif)
- [23. 订阅ChatGPT Plus](#23-订阅chatgpt-plus)
- [24. 树莓派修改](#24-树莓派修改)
  - [24.1 树莓派5更改设置](#241-树莓派5更改设置)

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

## 6.2 GDP预测

A股一致性预期分析系统 - 宏观一致性预期 - 季度年度统计图 - GDP

# 7. 非工程师指南：训练 LLaMA 2 聊天机器人

介绍
在本教程中，我们将向您展示如何构建自己的开源 ChatGPT，而无需编写任何代码！我们将使用 LLaMA 2 基础模型，使用开源指令数据集对其进行微调以进行聊天，然后将模型部署到您可以与朋友分享的聊天应用程序中。只需点击一下，我们就能实现卓越。😀

为什么这很重要？机器学习，尤其是 LLM（大型语言模型），已经见证了前所未有的普及，成为我们个人和商业生活中的重要工具。然而，对于大多数机器学习工程专业领域之外的人来说，训练和部署这些模型的复杂性似乎遥不可及。如果机器学习的预期未来是充满无处不在的个性化模型，那么未来将面临一个迫在眉睫的挑战：我们如何让那些没有技术背景的人能够独立利用这项技术？

在 Hugging Face，我们一直在默默努力为这个包容性的未来铺平道路。我们的工具套件（包括 Spaces、AutoTrain 和 Inference Endpoints 等服务）旨在让每个人都能接触到机器学习的世界。

为了展示这个民主化的未来是多么容易实现，本教程将向您展示如何使用Spaces、AutoTrain和ChatUI来构建聊天应用程序。只需三个简单的步骤，无需一行代码。作为背景介绍，我也不是 ML 工程师，而是 Hugging Face GTM 团队的成员。如果我能做到，那么你也可以！让我们开始吧！

https://huggingface.co/blog/Llama2-for-non-engineers

# 8. 推荐好用的SS/V2RAY/TROJAN机场

为什么推荐机场，因为稳定和廉价，自己折腾服务器一个是不稳定，一个是水管太小总是不够用，线路没有机场全。
机场有出口大的中转服务器中转海外线路，晚高峰优先级高，延迟稳定，出口带宽充足。
机场线路流媒体支持完善，个人自建比较难找到原生IP服务器。

瑶瑶の专线(yyssr.org)

推荐指数 ⭐⭐⭐⭐⭐

性价比 ⭐⭐⭐⭐

价格 适中

TG群 https://t.me/+i6FVpkHOKx0xODE1

关于价格

小流量：16CNY/mo: 128GB流量 支持2设备在线 限速80Mbps

大流量：26.9CNY/mo: 480GB流量 支持3设备在线 限速300Mbps

超大流量：43CNY/mo: 1024GB流量 支持3设备在线 限速500Mbps

关于线路

都是Shadowsocks协议节点，简称SS协议。

线路全部都是中转线路(拥有移动+联通+BGP国际出口优化)，节点延迟低，速度挺快，稳定性也不错。

流媒体支持：新加坡 台湾 美国 日本都是支持Netflix Disney+...

网站地址：https://yyssr.org

魅影极速

推荐指数 ⭐⭐⭐⭐

性价比 ⭐⭐

价格 贵

DuyaoSS机场推荐网站上榜机场

TG群：https://t.me/joinchat/HOQoQ09I100ke8sAxlxv0g

价位

VIP3，季付180元；年付600元；每月400G流量；节点40左右；

VIP4/5，半年付480元；年付800元；每月800G流量；节点100+。

特殊说明

新用户无法直接购买VIP5，需使用VIP4半年，系统自动审核通过后免费升级；
限制6个连接数，支持443端口，目前仅支持SSR，暂不支持 Surge（测试中）；
GCX节点是给国外用户用的，非国内用户；
有风控，可多水群；在魅影群的老人可找我bot要邀请码，或有很多群的常玩TG的；其他的请去魅影自己申请过审，不要找我
倒卖账号会被封号 issue：需要代理访问,hosts能连接网站，但会因为使用内地的IP被魅影拒绝访问，与墙无关
网站地址: https://maying.co

Nexitally

推荐指数 ⭐⭐⭐⭐

性价比 ⭐⭐

价格阶梯 贵

DuyaoSS机场推荐网站上榜机场

TG群 https://t.me/nexitallyusers

价位：

科学上网

基础服务：约88元/月，约458元/半年，约799元/年；线路80+

附加服务：Premium套餐有回国线路，需要单加钱，每月+76元左右（看汇率）。比基础套餐多几条线路

Group Access：允许至多5台设备（自家客户端）同时在线，每月+43元左右
游戏加速

Glowow加速器：月卡30元，双月卡52元，季卡69元，年卡229元。 issue：你不能直接用大陆IP注册帐号，需要短暂的国际互联网环境,hosts能连接网站，但会因为使用内地的IP被

Nexitally拒绝访问，与墙无关

网站链接：https://nexitallysafe.com/Index.aspx?language=cn

AmyTelecom(Nexitally的另一个机场)

推荐指数 ⭐⭐⭐⭐

性价比 ⭐⭐⭐

价格阶梯 有点贵 / 贵

致命缺点： 偶尔抽风，看脸，速度快起来飞起，要是尿崩那就完了

TG群 https://t.me/amytelecom_Official

价位

Bronze套餐：25元/月，每月60G流量；

Gold套餐：55元/月，每月400G流量。

其他情况

不限制ip数和设备数

暂时只支持SSR

8折码：Amy-2020-New-Year

支付方式：支付宝+微信+QQ+Epay

网站地址： https://www.amytele.com

DlerCloud

推荐指数 ⭐⭐⭐

性价比 ⭐⭐⭐

价格阶梯 略贵 / 贵 / 很贵

价位

Pass Bronze：288元/年，每月200G流量（2个IP）；提供标准BGP、Global节点；

Pass Silver：128元/季，388元/年，每月400G流量（3个IP）；增加高级BGP，Back节点；

Pass Gold：488元/年，每月500G流量（4个IP）；增加标准 IPLC节点；

Pass Platinum：688元/年，每月800G流量（5个IP）；增加高级 IPLC节点；

Pass Diamond：888元/年，每月1200G流量（6个IP）；增加高级 IPLC节点；

以及30个IP等的团队套餐。

需要注意

支持 Surge 托管，支持SS订阅，支持Clash订阅，支持 V2，支持SSD，支持普通端口

进群绑定Bot

支付方式：支付宝+微信支付+Crypto

网站地址：https://dlercloud.com

ssrcloud

推荐指数 ⭐⭐⭐⭐

性价比 ⭐⭐⭐⭐

价格阶梯 便宜/中等

价位

10元/月100G流量；20元/月200G流量；30元/月300G流量；60元/月600G流量；

40元/季，总400G流量；100元/年，总1000G流量；150元/年，总1500G流量；以及240元/360元/450元等年付套餐。

188元/月，独享ip线路套餐，500G流量

需要注意

流量套餐不限制ip和设备数

支持普通端口+单端口，支持surge

网站域名更换比较频繁，这个感觉比较麻烦，所以能进群就进群吧。

另外用户反映有些节点指向同一个服务器 不过还好，总量还是比较多的

有用户分组，新用户无法获得全部的中转节点，需要用一段时间才可以。
网站地址：https://support.dellcomputer.online

<https://ace-taffy.com/user/>

**售后群**
<https://t.me/thisissupport>

**公告牌**
<https://t.me/s/ssrdata>

<https://github.com/LeeYo2005/SS-SSR-V2RAY?tab=readme-ov-file#%E6%8E%A8%E8%8D%90%E5%A5%BD%E7%94%A8%E7%9A%84ssv2raytrojan%E6%9C%BA%E5%9C%BA>

# 9. 海外手机卡

卡片一：Giffgaff英国卡 🇬🇧

申请卡片免费，需要充值10英镑话费
无月租，接收短信免费
半年发一次短信保号
这是我目前用的卡，绑定Claude和推特很顺利

申请教程链接：https://rh0w322x8w.feishu.cn/wiki/ASkswc9BliHK9IkQX5xcfeeSnJg
淘宝购买，96元，自带 10 英镑话费
群友推荐，可以获得 15 英镑话费

## 9.1 Giffgaff激活事项

注意事项：

1.关闭手机卡的流量设置
2.注意每6个月发短信保号

激活网站

<https://www.giffgaff.com/activate>

中文操作指南

<https://www.lpolaris.com/article/giffgaff>

📍 卡片二：5ber esim 🇹🇭

购卡 $12
2元/月保号
拥有泰国实体号码 + 原生IP
支持微信、支付宝充值
官网购买📄：http://esim.5ber.com

📍 卡片三：新西兰 Skinny 卡 🇳🇿

购卡 100 多元
无月租，接收短信免费
25元/年保号
支持银联充值
推特很多人在卖，搜一下就能找到

📍 卡片四：Ultra Mobile 紫卡 🇺🇸

淘宝可以买
月租 $3，不便宜

<https://x.com/Crypto_QianXun/status/1815969126122488116>

# 10. 树莓派科学上网

## 10.1 简单方式 - raspberry_pi_shadowsocks
raspberry pi 3b+ 树莓派 shadowsocks 科学上网

  >Raspberry pi 3 Model B+  
  >OS：原装系统  
  >版本：Element 14  
  
### 本文为使用 python 版本的 shadowsocks 客户端来实现科学上网  

安装 python 版本的 shadowsocks 客户端与相关套件  

    sudo apt-get install python-pip python-m2crypto  
    sudo apt-get install shadowsocks  
    
修改配置文件:  

    cd /etc/shadowsocks  
    sudo vim config.json  
    
修改为如下内容：  

    {
        "server":"xxx.xxx.xxx.xxx",
        "server_port":xxxx,
        "local_address":"127.0.0.1",
        "local_port":1080,
        "password":"xxxxxxxx",
        "timeout":600,
        "method":"aes-256-cfb",
        "fast_open":false
    }

  >server ：服务端IP  
  >server_port ：服务端开放的端口，注意没有双引号  
  >password ：端口对应的密码  
  >method ：根据自己设定的服务端的加密方式来改  
  
启动：  

    sudo /usr/bin/sslocal -c /etc/shadowsocks/config.json -d start  

若报错：  

    Traceback (most recent call last):  
    File "/usr/local/bin/sslocal", line 9, in   
    load_entry_point('shadowsocks==2.8.2', 'console_scripts', 'sslocal')()  
    ....  
    ....  
    ....  
    AttributeError: /usr/local/lib/libcrypto.so.1.1: undefined symbol: EVP_CIPHER_CTX_cleanup  
    
则是由于Openssl库更新导致的方法名称变更问题，修复方法如下：  

    sudo vim /usr/local/lib/python2.7/distpackages/shadowsocks/crypto/openssl.py  

修改两条语句：  

    libcrypto.EVP_CIPHER_CTX_cleanup.argtypes = (c_void_p,)  
    #改为  
    libcrypto.EVP_CIPHER_CTX_reset.argtypes = (c_void_p,)
>
    libcrypto.EVP_CIPHER_CTX_cleanup.argtypes = (self._ctx)  
    #改为  
    libcrypto.EVP_CIPHER_CTX_reset.argtypes = (self._ctx)  

重启，再次执行启动命令即可  

添加开机启动：  

    sudo vim /etc/rc.local  

在文件尾部 `exit 0` 前面添加如下两行  

    sudo /usr/bin/local -c /etc/shadowsocks/config.json -d stop  
    sudo /usr/bin/local -c /etc/shadowsocks/config.json -d start  

至此，ss 客户端已经配置完毕！！！

### raspberry_shadowsocks.sh  
一键配置脚本，包括以上全部下载和全部修改  
用户只需按照提示提供自己梯子的相关信息即可  

### 配置 chromium/firefox SwitchOmega 

下载链接：[SwitchOmega](https://github.com/FelisCatus/SwitchyOmega/releases)  

把下载好的直接拉进扩展程序  

  >代理协议：SOCKS5  
  >代理服务器：127.0.0.1  
  >代理端口：1080  

![image](https://github.com/Garletta/raspberry_pi_shadowsocks/raw/master/image/raspberry_youtube.png)  

## 10.2 稍微复杂一点方式 - shadowsocks-for-raspberry
新到手了树莓派4,没有ss总感觉怎么弄都不太舒服，所以折腾了半天。不保证一定正确和最优
### 安装shadowsocks
其实可以使用sudo apt-get install shadowsocks直接解决，奈何我申请的vps使用aes-256-gcm加密的，apt下来的好像没有这种加密方式，所以还是自己下载吧。
- 到https://github.com/shadowsocks/shadowsocks git clone 这个项目
- 进入目录，python setup.py --build 编译
- python setup.py --install 安装，应该可以使用--prefix指定安装目录
- suod vim /etc/shadowsocks/config.json 编辑服务器的信息
- 使用sudo sslocal -c /etc/shadowsocks/config.json -d -start 就可以运行ss了
- 设置开机自动启动，新建一个sh脚本，输入下列代码，加入执行权限，sudo chmod 755 shadowsocks.sh， 然后编辑开机启动脚本sudo vim /etc/rc.local，在exit 0 之前加入/home/pi/Documents/shadowsocks.sh
```
#!/bin/bash

sudo sslocal -c /etc/shadowsocks/config.json -d start
```
OK，shadowsocks就安装好了，但是socks5不支持http和https的协议，所以还需要安装代理，首先给chromimum安装switchyomega

### 安装SwitchyOmega
- 由于chromimum没有商店，所以到https://github.com/FelisCatus/SwitchyOmega/releases 下载.crx格式的最新插件
- 现在的chromimum不支持拖入安装，所以需要更改.crx为.zip或者.rar解压到文件夹之后，在chromimum插件页面导入整个文件夹
- 进入SwitchyOmega，在proxy页面配置ss，协议选socks，代理服务器127.0.0.1，端口1080
- 可以配置auto switch， 默认直连，代理规则选刚配置完的proxy，规则列表格式选AutoProxy，网址写入https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt
好的，现在chromimum已经能上谷歌了，如果想要shell也能使用ss，就需要安装privoxy

### 安装privoxy
- 安装privoxy， sudo apt-get install privoxy
- 配置privoxy，sudo vim /etc/privoxy/config，找到并修改为以下代码
```
listen-address  127.0.0.1:8118
forward-socks5   /               127.0.0.1:1080 .
# 访问局域网不走ss
forward         192.168.*.*/     .
forward            10.*.*.*/     .
forward           127.*.*.*/     .
```
- 启动privoxy，systemctl start privoxy
- 现在进行测试，curl google.com --proxy 127.0.0.1:8118，如果有结果那么配置成功了，现在可以通过privoxy代理任意程序了
- 局部代理
- 局部代理 sudo vim /etc/local/bin/proxy，输入以下代码，需要使用时可以通过proxy加命令执行,例如proxy curl google.com
```
#!/bin/bash
http_proxy=http://127.0.0.1:8118 https_proxy=http://127.0.0.1:8118 ftp_proxy=ftp://127.0.0.1:8118 $*
```
大功告成，上个谷歌不容易

~~可能有人需要gfwlist设置网络代理，可以通过sudo pip install genpac安装genpac，然后sudo genpac --pac-proxy="SOCKS5 127.0.0.1:1080" -o autoproxy.pac --gfwlist-url="https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt"获得~~

# 11. SSR 导入

SSRCloud导入方法

- 1.服务器订阅 -> 更新服务器订阅(不通过代理)
- 2.随便选择一个服务器
- 3.代理规则 - "绕过..."
- 4.右键点SSR
- 5.用户中心 -> [SSR] 拷贝全部节点 URL 
- 6.点击剪贴板批量导入ssr://链接

# 12. Transformer by hand - Full Stack in Excel

<https://github.com/ImagineAILab/ai-by-hand-excel/>

我刚刚发布了我的第一个 Transformer 模型的 “全栈” Excel 实现。随意下载和尝试。

= 特点 =

• 输入嵌入
• 输出嵌入
•译码器
•编码器
• 位置编码
• 自我关注
• 交叉注意力
• 多头注意力
• 休闲口罩
• 缩放点积
• 跳过连接
• LayerNorm
• ReLU 激活
• 前馈
• Softmax
• 输出概率

<https://www.linkedin.com/posts/tom-yeh_transformer-aibyhand-excel-activity-7265044110388932608-w3Te?utm_source=share&utm_medium=member_desktop>

# 13. 模拟电路设计 - JKU 举办的中级 MOSFET模拟电路设计课程

这是 JKU 举办的中级 MOSFET 模拟电路设计课程的材料，课程编号为 336.009（“KV Analoge Schaltungstechnik”）。

本课程大量使用电路仿真，使用Xschem输入原理图，使用ngspice进行仿真。采用IHP Microelectronics的130nm CMOS技术SG13G2 。

工具和PDK集成在IIC-OSIC-TOOLS Docker镜像中，将在课程中使用。

<https://iic-jku.github.io/analog-circuit-design/>

# 14. MOSbius 芯片 - 集成电路课程中为学生提供连接测量、仿真和分析的动手实验

想在集成电路课程中为学生提供连接测量、仿真和分析的动手实验吗？为此，我们创建了 MOSbius 芯片！https://mosbius.org 上提供了文档和示例实验。

68 引脚 MOSbius 芯片包含 nMOS 和 pMOS 器件作为单独的晶体管，采用电流镜、差分对、共源配置、简单操作跨导放大器或逆变器等典型配置。电路可以用外部电线构建，还有一个 65x10 片上数字控制开关矩阵，可以将 63 个晶体管端子引脚以及 VDD 和 VSS 连接到芯片上的 10 条总线上以构建电路。

MOSbius 平台提供芯片、用于将芯片放置在无焊试验板上的适配器 PCB，以及用于对芯片进行编程和处理测量结果的软件工具。此外，还提供了一个 LTspice 库来运行电路仿真。

该平台允许（学生）设计人员在独特的动手环境中试验和学习 IC 风格的 MOS 电路。他们测量实际的 CMOS 电路，并将其操作与分析模型和电路仿真进行比较。

今年秋季学期，我们在模拟电子电路课程中为大四学生和研究生提供了第一批电路实验。学生们非常感谢与课程中学习的电路的实际实现进行交互的学习机会。

如果您想在课程中使用 MOSbius，请随时与我们联系。

最后但并非最不重要的一点是，请务必查看 https://lnkd.in/eucWz7-w 以查看此项目的所有热情贡献者。 

![](/picture/1734466096503.jpg)

<https://www.linkedin.com/posts/peter-kinget-7481a3_want-to-offer-your-students-hands-on-labs-activity-7274878090617524225-iGPm?utm_source=share&utm_medium=member_desktop>

# 15.  Jetson Orin Nano Super

AI 的树莓派：NVIDIA 廉价的 AI 迷你 PC 有何用途？

NVIDIA 本周推出了 Jetson Orin Nano Super，这是一款功能强大的小型计算机，能够在本地运行生成式 AI，价格仅为 249 美元。

作为人工智能竞赛的女王，NVIDIA 正在扩大其项目，并刚刚推出了 Jetson Orin Nano 超级开发套件。这个对于普通人来说有点野蛮的名字背后，我们发现了一个专门用于人工智能处理的开发套件——或者更确切地说是一个迷你超级计算机。该项目已经存在多年（2014 年推出了 Jetson TK1），并定期更新，直到 2019 年的 Nano 和 2022 年的 Orin Nano。顾名思义，后者现在是这个超级版本的基础，包含许多改进的更新。

适合开发者和人工智能爱好者的强大迷你电脑

有点像 Raspberry Pi，Jetson Orin Nano Super 并不是一台能够运行应用程序的简单迷你 PC。它更适合那些希望以非常紧凑的格式在本地运行生成式人工智能的修补者。

除了提高性能外，新型迷你 PC 还显着提高了人工智能应用程序的性能。 NVIDIA 声称，在某些生成式 AI 使用案例中，这些性能提高了 70%，AI 性能高达 67 TOPS。相比之下，旧版本的速度为 40 TOPS，而配备 M4 芯片的 Mac mini 则为 38 TOPS。新型号的内存带宽也提高了 50%，达到 102 GB/s。

正如我们来自专业网站Hardware & Co 的同事所解释的那样，NVIDIA 为其 Jetson Orin Nano Super 使用了一个简单的方法：超频。软件更新为迷你 PC 添加了 25 W 配置文件以提高性能，允许 ARM CPU 部分（六个 Cortex-A78E 内核）获得 200 MHz 达到 1.7 GHz。最重要的是，巧妙的手法让 GPU 的频率几乎翻倍，从 635 MHz 升至 1020 MHz。 Ampere一代iGPU拥有1,024个核心和32个Tensor核心。

正如我们来自专业网站Hardware & Co 的同事所解释的那样，NVIDIA 为其 Jetson Orin Nano Super 使用了一个简单的方法：超频。软件更新为迷你 PC 添加了 25 W 配置文件以提高性能，允许 ARM CPU 部分（六个 Cortex-A78E 内核）获得 200 MHz 达到 1.7 GHz。最重要的是，巧妙的手法让 GPU 的频率几乎翻倍，从 635 MHz 升至 1020 MHz。 Ampere一代iGPU拥有1,024个核心和32个Tensor核心。

<https://hardwareand.co/actualites/breves/nvidia-super-ise-sa-plateforme-de-developpement-jetson-orin-nano>

NVIDIA 将价格减半（这是有充分理由的）

NVIDIA 还寻求以 249 美元的价格提供其套件，比之前的型号（499 美元）便宜一半。这一决定旨在帮助变色龙继续前进，继续保持人工智能之王的地位。 2024 年对于 NVIDIA 来说是特别多产的一年，它真正改变了维度。

Jetson Orin Nano Super“降价”的决定也与这款迷你 PC 并未在硬件层面进化有关。它尤其受益于 NVIDIA 将向旧版 Jetson Orin Nano 用户免费提供的更新。除了 7 W 和 15 W 配置文件之外，后者还将能够受益于 25 W 配置文件的相同改进。但是，人们可能想知道为什么该品牌要等待才发布其小套件。

NVIDIA 合作伙伴 Palit 借此机会展示了Pandora。该公司并未将其称为“迷你电脑”，而是将其称为“迷你人工智能硬件”，并且不打算将其面向公众。它是为爱好者和开发人员设计的，有多种配置（8 GB 或 16 GB RAM），这将决定最大 TOPS 速度。然而，在撰写本文时，价格和供货情况仍未知。

<https://videocardz.com/pixel/palit-launches-pandora-nvidia-jetson-orin-nx-turned-mini-pc>

<https://www.journaldugeek.com/2024/12/20/raspberry-de-lia-a-quoi-sert-le-mini-pc-ia-pas-cher-de-nvidia/>

# 16. duino-coin - Arduino/Raspberry 可以挖矿

Raspberry Pi（自动安装）

wget https://raw.githubusercontent.com/revoxhere/duino-coin/master/Tools/duco-install-rpi.sh
sudo chmod a+x duco-install-rpi.sh
./duco-install-rpi.sh

https://github.com/revoxhere/duino-coin

# 17. 8bit复古计算机

有几台最新的（最近发布或将来发布的） 8 位计算机保留了旧计算机的乐趣，同时为它们提供了一些现代便利设施，如 SD 卡，有些甚至还有以太网。

ZX spectrum Next 看起来很棒。然后是 8 位人的 Commander X-16，由他和许多其他志愿者建造，应该很快就会准备好在 Kickstarter 上启动。此外还有 Mega65 项目，这是一个与 Commander X16 非常相似的项目。还有 Color Maximite 2，它似乎是一台速度超快的 BASIC 计算机，并不意味着与我所知道的任何机器完全兼容。其中一些是在 FPGA 上实现的，另一些是在实际芯片上实现的，有些集成了键盘/计算机，而有些则没有。无论如何，我真的很高兴终于能够购买其中一台有趣的旧机器，您可以在其中完全了解整个系统并轻松制作简单的游戏。

- ZX spectrum Next
- Commander X-16
- Color Maximite 2
- Mega65

<https://news.ycombinator.com/item?id=24611341>

# 18. github不能上传大文件 - 大于100M不可以

如果上传的话，需要删除

# 19. iPad 连接Raspberry Pi低延迟编程

通过 USB-C 将 Raspberry Pi 5 连接到 iPad Pro，打造便携式开发环境。设置 SSH、USB0 以太网、VNC、Neovim 和 Code-Server，实现在任何地方进行低延迟编码。

<https://github.com/av1155/RaspberryPi5-FullSetup>

# 20. N26开卡

<https://zhuanlan.zhihu.com/p/578071431>

<https://www.eluyee.com/n26/>

# 21. Deepseek + Kimi 生成ppt

1. Deepseek 深度思考 生成ppt大纲
2. Kimi ppt助手，生成ppt内容，一键生成，选择模版

<https://weibo.com/1842136381/PfVieEyAt>

# 22. 视频转gif

<https://www.aconvert.com/video/>

# 23. 订阅ChatGPT Plus

1. 参考这个链接，美区ID，购买gift卡。时常会出现登陆不上的情况，反复多刷几次，或者苹果ID登出再登陆即可

<https://github.com/farion1231/Way-to-ChatGPT-Plus/blob/main/%E4%BD%BF%E7%94%A8%E7%BE%8E%E5%9B%BD%E5%8C%BAApple%20ID%E8%AE%A2%E9%98%85.md>

credit card接收邮件，可以随意，不用非得美区ID的注册邮箱

购买礼品卡

第一步，前往苹果官网购买礼品卡。

<https://www.apple.com/shop/buy-giftcard/giftcard>

![](/picture/card1.png)
![](/picture/card2.png)

发送方式选择Email，面额选择右下角，填入20（或者19.99，IOS端订阅可以省$0.01），然后是实用的姓名和邮箱、发件人的姓名和邮箱，一定要使用自己能登录的邮箱地址，然后点击添加到购物袋。

![](/picture/card3.png)

检查邮箱地址无误后结账，下一步因为不使用Apple Card支付所以直接点击访客访问。

![](/picture/card4.png)

重头戏来了，选择信用卡或借记卡支付，填写入银联账户的卡号、过期时间和CVV码。下面地址栏填写入之前注册的美国地址和联系方式，再次强调一定要填写消防州的地址，否则会被收税。

![](/picture/card5.png)

勾选同意下一个订单，在下一个页面可以看到订单号，点击进入后可以查看订单明细。

![](/picture/card6.png)

一小时内，惯例邮箱内就能收到邮件，盒子里面就是兑换码，它就把复制到我们手机上。

![](/picture/card7.png)

在AppStore里面登录美区账号（注意一定不要在系统设置里登录），点击右上角头像，选择兑换充值卡或代码，将兑换码进去复制充值，成功后可以在账户界面看到余额。

![](/picture/card8.png)

最后打开ChatGPT应用，点击PLUS订阅，输入Apple ID密码即可成功订阅。在Appstore的订阅里取消订阅。

2. 上述链接有个错误，订阅 是在 设置 -> 最顶端的Apple账户 -> 订阅

- 取消也是在这里取消
- 第一次注册时，在App store里看不到“订阅” 

# 24. 树莓派修改

## 24.1 树莓派5更改设置

![](/picture/rpi5__20250503_change2.png)

参考操作

<https://www.licc.tech/article?id=79>
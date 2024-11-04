- [1.使用Tortoisegit git管理上传文件代码到github](#1使用tortoisegit-git管理上传文件代码到github)
- [2.设置git全局代理端口](#2设置git全局代理端口)
- [3.md加目录](#3md加目录)
- [4.colab里如何运行nanoGPT](#4colab里如何运行nanogpt)
- [5. 树莓派增加定时运行的程序](#5-树莓派增加定时运行的程序)
- [6. 慧博投研](#6-慧博投研)
  - [6.1 拉取行业数据](#61-拉取行业数据)
- [7. 非工程师指南：训练 LLaMA 2 聊天机器人](#7-非工程师指南训练-llama-2-聊天机器人)
- [8. 推荐好用的SS/V2RAY/TROJAN机场](#8-推荐好用的ssv2raytrojan机场)
- [9. 海外手机卡](#9-海外手机卡)
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

售后群
<https://t.me/thisissupport>

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

# 10.1 简单方式 - raspberry_pi_shadowsocks
raspberry pi 3b+ 树莓派 shadowsocks 科学上网

  >Raspberry pi 3 Model B+  
  >OS：原装系统  
  >版本：Element 14  
  
## 本文为使用 python 版本的 shadowsocks 客户端来实现科学上网  

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

## raspberry_shadowsocks.sh  
一键配置脚本，包括以上全部下载和全部修改  
用户只需按照提示提供自己梯子的相关信息即可  

## 配置 chromium/firefox SwitchOmega 

下载链接：[SwitchOmega](https://github.com/FelisCatus/SwitchyOmega/releases)  

把下载好的直接拉进扩展程序  

  >代理协议：SOCKS5  
  >代理服务器：127.0.0.1  
  >代理端口：1080  

![image](https://github.com/Garletta/raspberry_pi_shadowsocks/raw/master/image/raspberry_youtube.png)  

# 10.2 稍微复杂一点方式 - shadowsocks-for-raspberry
新到手了树莓派4,没有ss总感觉怎么弄都不太舒服，所以折腾了半天。不保证一定正确和最优
## 安装shadowsocks
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

## 安装SwitchyOmega
- 由于chromimum没有商店，所以到https://github.com/FelisCatus/SwitchyOmega/releases 下载.crx格式的最新插件
- 现在的chromimum不支持拖入安装，所以需要更改.crx为.zip或者.rar解压到文件夹之后，在chromimum插件页面导入整个文件夹
- 进入SwitchyOmega，在proxy页面配置ss，协议选socks，代理服务器127.0.0.1，端口1080
- 可以配置auto switch， 默认直连，代理规则选刚配置完的proxy，规则列表格式选AutoProxy，网址写入https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt
好的，现在chromimum已经能上谷歌了，如果想要shell也能使用ss，就需要安装privoxy

## 安装privoxy
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

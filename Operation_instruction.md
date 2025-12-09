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
- [25. Google Colab 集成了 Data Science Agent](#25-google-colab-集成了-data-science-agent)
- [26. Chrome网页保存为pdf](#26-chrome网页保存为pdf)
- [27. 树莓派上配置 shadowsocks-libev 客户端并实现自动重启](#27-树莓派上配置-shadowsocks-libev-客户端并实现自动重启)
  - [**1. 安装 shadowsocks-libev**](#1-安装-shadowsocks-libev)
  - [**2. 配置 Shadowsocks 客户端参数**](#2-配置-shadowsocks-客户端参数)
  - [**3. 启动并设置自动重启**](#3-启动并设置自动重启)
    - [**启动 Shadowsocks 本地客户端**](#启动-shadowsocks-本地客户端)
    - [**设置开机自启（自动重启）**](#设置开机自启自动重启)
  - [**4. 检查运行状态**](#4-检查运行状态)
  - [**5. （可选）重启服务以应用新配置**](#5-可选重启服务以应用新配置)
  - [**6. 让设备使用代理**](#6-让设备使用代理)
  - [**小结**](#小结)
- [29. 树莓派浏览器设置](#29-树莓派浏览器设置)
  - [1. 浏览器科学上网](#1-浏览器科学上网)
  - [2. 终端命令行科学上网](#2-终端命令行科学上网)
  - [3. 系统全局代理（仅部分桌面环境支持）](#3-系统全局代理仅部分桌面环境支持)
  - [4. 直接测试](#4-直接测试)
  - [5. 进阶：Privoxy 转 HTTP 代理（可选）](#5-进阶privoxy-转-http-代理可选)
- [30. WSL科学上网](#30-wsl科学上网)
  - [30.1 当代理修改时，需要修改端口](#301-当代理修改时需要修改端口)
- [31. VSCode如何打开WSL路径](#31-vscode如何打开wsl路径)
- [32. 输入命令：code .，打开的是cursor，怎么换成VS CODE](#32-输入命令code-打开的是cursor怎么换成vs-code)
- [33. how to install claude code in windows](#33-how-to-install-claude-code-in-windows)
  - [1. **Native Windows Installation (No WSL, as of July 2025)**](#1-native-windows-installation-no-wsl-as-of-july-2025)
  - [2. **Installation Using WSL (Windows Subsystem for Linux)**](#2-installation-using-wsl-windows-subsystem-for-linux)
  - [**Key Considerations and Limitations**](#key-considerations-and-limitations)
  - [**Resources**](#resources)
- [34. cmd中可以运行gemini CLI，但是VS Code里不能运行gemini CLI 解决方法](#34-cmd中可以运行gemini-cli但是vs-code里不能运行gemini-cli-解决方法)
  - [方案 A（最快）：把 VS Code 终端切换为 **Command Prompt (cmd)**](#方案-a最快把-vs-code-终端切换为-command-prompt-cmd)
  - [方案 B（当前终端临时绕过）：在 PowerShell 中临时放开策略](#方案-b当前终端临时绕过在-powershell-中临时放开策略)
  - [方案 C（对你账号永久生效）：把 PowerShell 策略改为 **RemoteSigned**](#方案-c对你账号永久生效把-powershell-策略改为-remotesigned)
  - [方案 D（不改策略也能跑）：显式调用 `.cmd` 可执行](#方案-d不改策略也能跑显式调用-cmd-可执行)
  - [额外检查（可选但有用）](#额外检查可选但有用)
- [35. Kodi插件配置](#35-kodi插件配置)
- [36. 设置Gemini CLI API Key](#36-设置gemini-cli-api-key)
- [37. Foxmail 6.5导入邮件](#37-foxmail-65导入邮件)
- [38. VS Code 配置 GitHub 代理](#38-vs-code-配置-github-代理)
  - [方法 1：配置 Git 全局代理（推荐）](#方法-1配置-git-全局代理推荐)
  - [查看代理](#查看代理)

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

# 25. Google Colab 集成了 Data Science Agent

Google Colab 是一个免费、云端托管的 Jupyter Notebook 环境，您可以直接在浏览器中编写并运行 Python 代码。它免费提供对 Google Cloud GPU 和 TPU 的访问权限，这对运行 AI 模型来说是一个革命性的改变，也让项目协作变得更加简化。

去年 12 月，Google 分享了 Colab 中的 Data Science Agent 如何借助 Gemini 为受信任的测试者自动创建笔记本，省去了导入库、加载数据以及编写模板代码等繁琐操作。受信任的测试者对 Data Science Agent 反响热烈，认为它让工作流程更流畅，并能比以往更快地发现洞察。

如今，Google 宣布将 Data Science Agent 推广至年满 18 岁的 Colab 用户以及部分国家和语言地区。Google 也在扩展与大学的合作，希望通过将简单的自然语言描述转换成完整且可运行的 Colab 笔记本，帮助研究实验室在数据处理和分析方面节省时间。

Data Science Agent 的工作原理如下：
1. 从空白开始： 打开一个空白的 Colab 笔记本。
2. 添加数据： 上传您的数据文件。
3. 描述目标： 在 Gemini 侧边栏中描述您想进行的分析或需要的原型（例如，“可视化趋势”、“构建并优化预测模型”、“填充缺失值”、“选择最佳统计方法”）。
4. 见证 Data Science Agent 的自动化过程： 静待生成必要的代码、导入库以及可在 Colab 中执行的分析结果。
视频演示示例：Data Science Agent 从理解数据到在 Colab 笔记本中呈现洞察的自动化分析过程（序列已简化，仅作演示之用。Data Science Agent 可能会出现错误。）

Data Science Agent 带来的益处
• 完整的可运行 Colab 笔记本： 不仅仅是代码片段，而是可以直接执行的完整笔记本。
• 可修改的解决方案： 轻松定制和扩展生成的代码，以满足您的特定需求。
• 可共享的结果： 借助 Colab 标准分享功能，与团队成员进行协作。
• 节省时间： 将更多精力集中在从数据中获取洞察，而不是在环境设置和模板代码上浪费时间。

同时，Google 的 Data Science Agent 在 HuggingFace 的 DABStep 基准测试（DABStep: Data Agent Benchmark for Multi-step Reasoning） 中取得了第 4 名，表现优于基于 GPT 4.0 的 ReAct agents、Deepseek、Claude 3.5 Haiku 和 Llama 3.3 70B 等模型。

立即开始体验 Data Science Agent
只需上传一些数据，然后在 Gemini 侧边栏中概述您的数据分析目标即可轻松上手。您可以在 Kaggle 或 Data Commons 上探索数据集，以下是一些示例数据和提示供您参考：

• Stack Overflow 年度开发者调查：可以尝试询问“可视化最受欢迎的编程语言”
• Iris 鲜花数据集：可以尝试询问“计算并可视化数据集中 Pearson、Spearman 和 Kendall 的相关性”
• Glass Classification：可以尝试询问“在此数据集上训练一个随机森林分类器”

Google 希望这能彻底改变您的数据分析工作流程。

<https://weibo.com/1727858283/PgVSP0KrA>

官方链接

<https://developers.googleblog.com/en/data-science-agent-in-colab-with-gemini/?linkId=13237992&continueFlag=4b7ee00dfb52f7b3f6f63d1958338a4b>

# 26. Chrome网页保存为pdf

Chrome 右上角三个点，选 打印 -> 目标打印机选择 “另存为pdf”

# 27. 树莓派上配置 shadowsocks-libev 客户端并实现自动重启

下面是**树莓派上配置 shadowsocks-libev 客户端并实现自动重启**的完整步骤，适用于科学上网（翻墙）需求：

---

## **1. 安装 shadowsocks-libev**

在树莓派终端输入：

```bash
sudo apt update
sudo apt install shadowsocks-libev
```


---

## **2. 配置 Shadowsocks 客户端参数**

编辑配置文件 `/etc/shadowsocks-libev/config.json`：

```bash
sudo nano /etc/shadowsocks-libev/config.json
```

示例内容（请用你的SSR节点信息替换）：

```json
{
  "server":"你的服务器IP或域名",
  "server_port":8388,
  "local_address":"0.0.0.0",
  "local_port":1080,
  "password":"你的密码",
  "timeout":300,
  "method":"aes-256-cfb"
}
```


---

## **3. 启动并设置自动重启**

### **启动 Shadowsocks 本地客户端**

```bash
sudo systemctl start shadowsocks-libev-local@config
```
这里的 `config` 指的是 `/etc/shadowsocks-libev/config.json`，如你用其他文件名需对应修改[5]。

### **设置开机自启（自动重启）**

```bash
sudo systemctl enable shadowsocks-libev-local@config
```
这样每次开机或异常退出后都会自动重启[2][3][5]。

---

## **4. 检查运行状态**

查看服务运行情况：

```bash
sudo systemctl status shadowsocks-libev-local@config
```


---

## **5. （可选）重启服务以应用新配置**

每次修改配置后，重启服务：

```bash
sudo systemctl restart shadowsocks-libev-local@config
```


---

## **6. 让设备使用代理**

- 树莓派本地监听端口（如1080）为SOCKS5代理端口。
- 其他设备可将代理设置为树莓派IP:1080，或结合iptables等实现透明代理。

---

## **小结**

1. 安装 shadowsocks-libev  
2. 编辑 `/etc/shadowsocks-libev/config.json` 填写SSR节点信息  
3. 启动并设置 `shadowsocks-libev-local@config` 服务自启  
4. 检查和重启服务确保生效

这样设置后，shadowsocks-libev 会随系统启动自动运行，异常退出也会自动重启，科学上网稳定可靠[2][3][5]。

Citations:
[1] https://blog.bingliang.me/posts/2016-05-28-make-raspberry-pi-a-fqrouter/
[2] https://gfw.report/blog/ss_tutorial/en/
[3] https://www.zhangminghao.com/2016/08/24/1472047768/
[4] https://zlotus.github.io/2018/09/25/rbp3-aws-gateway/
[5] https://www.zixi.org/archives/raspberrypi-proxy-shadowsocks.html
[6] https://tuki.moe/use-raspberry-pi-as-gateway-for-global-internet-browsing/
[7] https://upcloud.com/resources/tutorials/install-shadowsocks-libev-socks5-proxy
[8] https://github.com/nvidhub/note/blob/master/%E6%A0%91%E8%8E%93%E6%B4%BE3B%E5%AE%89%E8%A3%85OpenWRT%E5%AE%9E%E7%8E%B0%E7%BF%BB%E5%A2%99.md
[9] https://www.e2encrypted.com/howtos/install-shadowsocks-libev-with-simple-obfs/
[10] https://www.reddit.com/r/MagicMirror/comments/vw7rfi/using_systemd_services_to_autostart_fails_rpi4/

---
Answer from Perplexity: pplx.ai/share

# 29. 树莓派浏览器设置

你已经在树莓派上成功启动了 shadowsocks-libev 的本地客户端（ss-local），现在只需让本地应用流量通过 SOCKS5 代理即可科学上网。常见方法如下：

---

## 1. 浏览器科学上网

- **推荐方式**：在浏览器（如Firefox或Chrome）设置代理。
- 代理类型选择 SOCKS5，服务器填写 `127.0.0.1`，端口填写 `1080`（与你 config.json 保持一致）。
- 例如，Firefox 设置路径：设置 → 网络设置 → 手动代理配置 → SOCKS Host 填写 127.0.0.1，端口 1080，选择 SOCKS v5[14]。

---

## 2. 终端命令行科学上网

- 使用 `proxychains` 工具让终端命令通过 SOCKS5 代理：
  ```bash
  sudo apt install proxychains4
  ```
- 编辑 `/etc/proxychains4.conf`，在末尾添加：
  ```
  socks5  127.0.0.1 1080
  ```
- 用法示例：
  ```bash
  proxychains4 curl https://www.google.com
  ```
  这样 curl 等命令就会通过 shadowsocks 科学上网[8][6]。

---

## 3. 系统全局代理（仅部分桌面环境支持）

- 有些桌面环境（如GNOME）支持在“网络”设置中配置系统代理，填写 SOCKS5 代理为 127.0.0.1:1080。
- 但部分命令行程序和系统服务不会自动走全局代理。

---

## 4. 直接测试

- 你可以用 curl 测试代理是否生效：
  ```bash
  curl --socks5 127.0.0.1:1080 https://ipinfo.io
  ```
  返回的 IP 若为你的代理服务器出口 IP，说明已成功翻墙[6]。

---

## 5. 进阶：Privoxy 转 HTTP 代理（可选）

- 如果有应用只支持 HTTP 代理，可用 privoxy 将 SOCKS5 转为 HTTP 代理[8]。

---

**总结**：  
你只需在需要科学上网的应用中设置 SOCKS5 代理为 `127.0.0.1:1080`，即可让树莓派本地科学上网，无需额外配置网关或 DNS[6][14][8]。

Citations:
[1] https://blog.csdn.net/aaaaaaaa123345/article/details/131106506
[2] https://haipeng.me/2017/12/12/raspberry-pi-vpn-remote-access/
[3] https://github.com/nvidhub/note/blob/master/%E6%A0%91%E8%8E%93%E6%B4%BE3B%E5%AE%89%E8%A3%85OpenWRT%E5%AE%9E%E7%8E%B0%E7%BF%BB%E5%A2%99.md
[4] https://www.cnblogs.com/jojodru/p/15789320.html
[5] https://www.aihoom.com/1802.html
[6] https://cloud.tencent.com/developer/article/2449948
[7] https://zlotus.github.io/2018/09/25/rbp3-aws-gateway/
[8] https://blog.biofan.org/2019/08/linux-proxy/
[9] https://blog.csdn.net/Isaachim/article/details/110383558
[10] https://zsummer.github.io/2020/05/09/2020-06-15-shadowsock-proxy/
[11] https://www.liaol.net/posts/raspberry-as-gfw-fucker/
[12] https://titaniumblog.site123.me/%E5%8D%9A%E5%AE%A2/shadowsocks
[13] https://picockpit.com/raspberry-pi/zh/%E5%A6%82%E4%BD%95%E7%94%A8%E6%A0%91%E8%8E%93%E6%B4%BE%E8%AE%BE%E7%BD%AE%E8%BF%9C%E7%A8%8B%E5%B7%A5%E4%BD%9C%E7%9A%84vpn%EF%BC%9F/
[14] https://cn.linux-terminal.com/?p=3467
[15] https://sulian-blog.com/shadowsocks-v2ray-ws-proxy/
[16] https://gfw.report/blog/ss_tutorial/zh/
[17] https://libertyleadingnetwork.blogspot.com/2019/08/shadowsocksss-redirprivoxytpproxy.html
[18] https://shiping.date/4.html

---
Answer from Perplexity: pplx.ai/share

# 30. WSL科学上网

在 Windows 上通过 Clash 可以科学上网，但 WSL 无法科学上网的原因，通常是因为 WSL 网络没有正确配置为使用 Windows 的代理。下面是解决方法，让你的 WSL 也能走 Clash 的代理。

✅ 方法一：配置环境变量（适用于 HTTP/HTTPS 流量）
假设你在 Clash 中配置的本地代理端口是：

HTTP 代理端口：7890

SOCKS5 代理端口：7891

在 WSL 中编辑 ~/.bashrc 或 ~/.zshrc 文件（取决于你使用的 shell）：

nano ~/.bashrc
添加以下内容（以 Clash 默认端口为例）：

export http_proxy="http://127.0.0.1:7890"
export https_proxy="http://127.0.0.1:7890"
export all_proxy="socks5://127.0.0.1:7891"
保存并执行：

source ~/.bashrc
测试一下网络连通性：

curl https://google.com

## 30.1 当代理修改时，需要修改端口

Clash Verge 

设置-clash设置-端口设置-用鼠标点“7897”-显示混合端口7897，socks代理端口7898，https代理端口7899

http: 7899
socks5: 7898

nano ~/.bashrc

export http_proxy="http://127.0.0.1:7899" 
export https_proxy="http://127.0.0.1:7899" 
export all_proxy="socks5://127.0.0.1:7898"

保存并执行：

source ~/.bashrc

测试一下网络连通性：

curl https://google.com

# 31. VSCode如何打开WSL路径

要在VSCode中打开WSL路径，可以采用以下常用方法：

1. **在WSL终端中使用 code 命令**
   - 打开你的WSL终端（如Ubuntu）。
   - 进入你想用VSCode打开的目录，例如 `cd ~/myproject`。
   - 输入命令：`code .`
   - 这会直接以Remote WSL方式在VSCode中打开该文件夹。如果首次使用，会自动下载安装所需组件[9][7][11][13]。

2. **从VSCode窗口中连接WSL**
   - 在Windows上启动VSCode。
   - 按下 `F1` 键，输入并选择 `WSL: Connect to WSL`（连接默认发行版），或 `WSL: Connect to WSL using Distro`（选择特定发行版）。
   - 使用“文件”>“打开文件夹”选择你在WSL下的目标目录[10][9]。

3. **从Windows命令行或PowerShell直接指定WSL路径**
   - 使用命令格式：
     ```
     code --remote wsl+ 
     ```
     例如：`code --remote wsl+Ubuntu /home/username/project`[9][10]。

4. **通过VSCode终端切换默认Shell为WSL**
   - 在VSCode中按 `Ctrl+Shift+P`，输入 `Terminal: Select Default Shell`，然后选择你安装的WSL终端。
   - 新终端即为WSL环境[5]。

**注意事项：**
- `code .`命令需要在VSCode安装时勾选“添加到PATH”，否则WSL终端中无法识别该命令[6][9]。
- 若遇到`code`命令无效，可重启终端或重新安装VSCode并确保PATH设置[10]。

以上方法均可高效地在VSCode中打开和管理WSL下的文件和项目目录。

[1] https://www.youtube.com/watch?v=q74CP4fB7cY
[2] https://www.youtube.com/watch?v=8Q1bRZaHH24
[3] https://www.youtube.com/watch?v=FQNO8DsGnlQ
[4] https://www.youtube.com/watch?v=Qcyycy4aYgY
[5] https://worktile.com/kb/ask/553003.html
[6] https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/wsl-vscode
[7] https://blog.csdn.net/Little_Shrimp/article/details/128106347
[8] https://blog.csdn.net/qq_43152052/article/details/124640317
[9] https://vscode.js.cn/docs/remote/wsl
[10] https://vscode.github.net.cn/docs/remote/wsl
[11] https://jingyan.baidu.com/article/9c69d48f6afb4a52c8024e2e.html
[12] https://mission-young.github.io/2020/03/26/%E8%A7%A3%E5%86%B3vscode-%E6%89%93%E5%BC%80WSL-%E7%B3%BB%E7%BB%9F%E7%9B%AE%E5%BD%95%E5%87%BA%E9%94%99%E7%9A%84%E9%97%AE%E9%A2%98/
[13] https://www.cnblogs.com/tianyamoon/p/14195169.html

# 32. 输入命令：code .，打开的是cursor，怎么换成VS CODE

出现你在WSL中输入`code .`却打开的是**Cursor**，不是**VS Code**，原因是Cursor安装时在PATH变量中优先于VS Code，导致code命令被Cursor覆盖了[5][6]。

**解决办法：**

1. **调整环境变量PATH顺序（推荐）**
   - 打开Windows“系统属性”->“高级”->“环境变量”。
   - 找到“系统变量”或“用户变量”里的`PATH`，把VS Code的路径（如 `C:\Users\\AppData\Local\Programs\Microsoft VS Code\bin`）移到Cursor路径（如 `C:\Users\\AppData\Local\Programs\cursor\resources\app\bin`）的前面[5][6]。
   - 确保在PATH变量中，VS Code的bin路径排在Cursor前。

2. **注销或重启生效**
   - 修改PATH后，关闭所有终端窗口，并重新打开WSL终端再执行`code .`命令。

3. **卸载或重命名Cursor命令（可选）**
   - 不需要Cursor的“code”命令时，可以直接卸载Cursor，或手动重命名Cursor的`code`和`code.cmd`为其他名字（如`cursor`和`cursor.cmd`）[5]。

这样设置好后，`code .`会在WSL中正确启动VS Code，而`cursor .`可以单独用来启动Cursor编辑器，实现两个命令分别调用不同的编辑器。

**注意：**
- 修改环境变量需要管理员权限，并注意不要删除其他系统路径，否则可能导致程序异常。
- 这种现象是因为Cursor安装时把自己注册为`code`命令，很多用户反馈有同样困扰[5][6]。

[1] https://blog.csdn.net/henryhu712/article/details/132812380
[2] https://cloud.tencent.com/developer/information/VScode%E6%97%A0%E6%B3%95%E6%AD%A3%E7%A1%AE%E8%BF%9E%E6%8E%A5%E5%88%B0WSL
[3] https://www.reddit.com/r/ClaudeAI/comments/1lantwy/complete_wsl_claude_code_cursor_setup_guide_for/?tl=zh-hans
[4] https://blog.csdn.net/Flying_Motor/article/details/138114028
[5] https://github.com/cursor/cursor/issues/1238
[6] https://forum.cursor.com/t/cursor-install-broke-code-command-in-wsl2/712
[7] https://cloud.tencent.com/developer/information/WSL2:%E4%BD%BF%E7%94%A8*..code%20workspace%E6%96%87%E4%BB%B6%E4%BB%8E%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%90%AF%E5%8A%A8VSCode
[8] https://www.youtube.com/watch?v=8Q1bRZaHH24
[9] https://developer.aliyun.com/article/1673794

# 33. how to install claude code in windows

Claude Code can now be installed on Windows in two main ways: using **WSL (Windows Subsystem for Linux)**, which has been the traditional and most reliable approach, and as of July 2025, also **natively using Windows terminal, Node.js, and Git Bash**. Here are both methods with step-by-step instructions, including important caveats.

## 1. **Native Windows Installation (No WSL, as of July 2025)**

**Requirements:**
- Windows 10 (version 2004+) or Windows 11
- Node.js (v18 or higher recommended)
- Git for Windows (needed for bash commands)
- NPM (Node.js package manager)
- Anthropic subscription with Claude Code access

**Steps:**

1. **Install Node.js (LTS recommended):**
   - Download from the Node.js official website and install. Confirm version:
     ```
     node -v
     npm -v
     ```
2. **Install Git for Windows:**
   - Download and install from the official Git website.
   - Take note of the install path, e.g., `C:\Program Files\Git\bin\bash.exe`[7][1].

3. **Set the `CLAUDE_CODE_GIT_BASH_PATH` environment variable:**
   - Open a PowerShell window and run:
     ```
     $env:CLAUDE_CODE_GIT_BASH_PATH="C:\Program Files\Git\bin\bash.exe"
     ```
     Adjust path if you installed Git elsewhere[1][7].

4. **Install Claude Code globally with npm:**
   ```
   npm install -g @anthropic-ai/claude-code
   ```

5. **Authenticate Claude Code:**
   ```
   claude auth login
   ```
   - Copy the browser URL from the terminal into your browser to complete authentication[8][7].

6. **Run Claude Code:**
   ```
   claude
   ```

**Troubleshooting:**
- If you encounter permission errors with npm, configure npm to use a user-writable directory:
  ```
  mkdir ~/.npm-global
  npm config set prefix '~/.npm-global'
  ```
  Then re-run the install command[9][1].

## 2. **Installation Using WSL (Windows Subsystem for Linux)**

**WSL-based installs are still widely supported and work reliably.**

**Requirements:**
- Windows 10/11
- WSL2 (with Ubuntu or Debian recommended)

**Steps:**

1. **Enable WSL and install Ubuntu:**
   - In an **Administrator PowerShell**:
     ```
     wsl --install
     wsl --install -d Ubuntu
     ```

2. **Open Ubuntu from Start Menu and update packages:**
   ```
   sudo apt update
   sudo apt upgrade
   ```

3. **Install Node.js & npm:**
   ```
   curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
   sudo apt-get install -y nodejs
   node -v
   npm -v
   ```
  
4. **Install Claude Code:**
   ```
   sudo npm install -g @anthropic-ai/claude-code
   ```

5. **Authenticate Claude Code:**
   ```
   claude auth login
   ```
   - Open the provided URL in your browser to complete authentication.

6. **Usage:**
   - You can now access your Windows files under `/mnt/c/` from within WSL and run Claude Code commands[5][3][10].

## **Key Considerations and Limitations**

- Only the **native Windows install** route (with Node.js, Git Bash, and correct environment variable) allows installation *without* WSL as of July 2025[7][1][8].
- If you encounter issues with the native method, WSL remains the fallback and most robust solution.
- Always authenticate via `claude auth login` after installation; you may need to manually copy the URL into your Windows browser for login[5][6].

## **Resources**

- Anthropic official docs: step-by-step setup and troubleshooting guide for both WSL and native[1].
- Community guides with scripts and troubleshooting details[5][6].
- Japanese-language step-by-step guides available for Pro/Max users[8].

If you are unsure whether to use **WSL or Native**: for maximum compatibility, use WSL; for new installs and convenience, try Native first. If you encounter issues, consult the related troubleshooting sections in the official and community guides.

[1] https://docs.anthropic.com/en/docs/claude-code/setup
[2] https://www.youtube.com/watch?v=lQmsLSR13ac
[3] https://claude.ai/public/artifacts/03a4aa0c-67b2-427f-838e-63770900bf1d
[4] https://www.youtube.com/watch?v=hI6Wb4zWK3Q
[5] https://github.com/VonHoltenCodes/CLAUDECODE_COMPLETE_WINDOWS_INSTALL_GUIDE
[6] https://github.com/SankeerthBoddu/ClaudeCodeWindows
[7] https://www.youtube.com/watch?v=jXhCXVY9WCU
[8] https://note.com/ritsuto2525/n/n46c8757a21b1
[9] https://www.geeky-gadgets.com/how-to-install-claude-code-on-windows/
[10] https://www.reddit.com/r/ChatGPTCoding/comments/1iyxtay/how_to_install_and_use_claude_code_maybe_the_best/
[11] https://www.youtube.com/watch?v=hI6Wb4zWK3Q&vl=en-US
[12] https://www.youtube.com/watch?v=yw14MMPTaEg
[13] https://www.youtube.com/watch?v=pClhzCbGE8M
[14] https://www.youtube.com/watch?v=XMQTJf8Pszc
[15] https://www.youtube.com/watch?v=VB68aY71bTI
[16] https://www.youtube.com/watch?v=-sNLKVptR8U
[17] https://www.youtube.com/watch?v=hpMrTabldEY&vl=en

# 34. cmd中可以运行gemini CLI，但是VS Code里不能运行gemini CLI 解决方法

你这个现象是**VS Code 默认用 PowerShell** 作为集成终端，而 PowerShell 的 **ExecutionPolicy（脚本执行策略）被设置为“Restricted”**，所以像 `npm.ps1`、`gemini.ps1` 这类 shim 脚本会被拦截；在 **cmd** 里没问题，是因为它走的是 `npm.cmd` / `gemini.cmd`，不受 PowerShell 限制。

给你几种等价解决方案，按偏好选择其一即可：

---

## 方案 A（最快）：把 VS Code 终端切换为 **Command Prompt (cmd)**

1. VS Code 顶部菜单 **Terminal → New Terminal** 右侧的小箭头 → **Select Default Profile**
2. 选 **Command Prompt**。
3. 打开一个新终端，再运行：

   ```cmd
   gemini --help
   npm -v
   ```

> 这和你在独立的 cmd 中运行一致，基本“一步到位”。

---

## 方案 B（当前终端临时绕过）：在 PowerShell 中临时放开策略

在 VS Code 的 PowerShell 终端先执行（仅对**当前终端会话**有效）：

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
```

然后再试：

```powershell
npm -v
gemini --help
```

---

## 方案 C（对你账号永久生效）：把 PowerShell 策略改为 **RemoteSigned**

> 适用于个人电脑。公司域策略可能会覆盖，如果报错就用方案 A 或 B。

在 PowerShell（普通权限即可）执行：

```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

验证：

```powershell
Get-ExecutionPolicy -List
```

重启 VS Code，再试：

```powershell
npm -v
gemini --help
```

---

## 方案 D（不改策略也能跑）：显式调用 `.cmd` 可执行

在 PowerShell 中直接调用 `.cmd` 版本，绕过 `.ps1`：

```powershell
npm.cmd -v
gemini.cmd --help
npx.cmd gemini "hello"
```

---

## 额外检查（可选但有用）

1. **确保全局 npm bin 在 PATH 中**（通常是 `%APPDATA%\npm`）
   在 PowerShell 中：

   ```powershell
   echo $env:PATH
   where gemini
   where npm
   ```

   如果 `where gemini` 指向 `…\AppData\Roaming\npm\gemini.cmd` / `gemini.ps1` 就对了。
2. **修改后重启 VS Code**，让 PATH/策略生效。

---

如果你希望继续用 PowerShell，我建议用 **方案 C（RemoteSigned）**；如果想省事直接能跑，用 **方案 A（切到 cmd）**。
你现在在 VS Code 里具体报的错误（比如运行 `gemini` 的提示信息）也可以贴出来，我再帮你对症处理。

# 35. Kodi插件配置

1. 确定配置文件位置
对于 Kodi 的 YouTube 插件，API 信息应该写在：

text
~/.kodi/userdata/addon_data/plugin.video.youtube/settings.xml

修改配置

<setting id="youtube.api.key" value="XXXXXXXXXX"/>
<setting id="youtube.api.id" value="YYYYYYYYYYYYYYYYY.apps.googleusercontent.com"/>
<setting id="youtube.api.secret" value="ZZZZZZZZZZZZZZZZZZZZ"/>

默认配置

<setting id="youtube.api.key" default="true" />
<setting id="youtube.api.id" default="true" />
<setting id="youtube.api.secret" default="true" />

# 36. 设置Gemini CLI API Key

访问
 https://console.cloud.google.com/

太好了！现在我来指导您在 Google Cloud Console 中创建 API Key：

**步骤1：创建或选择项目**
1. 在页面顶部，您会看到一个项目选择器（通常显示为项目名称或"选择项目"）
2. 点击它，然后：
   - 如果您已有项目，可以选择现有的
   - 如果没有项目，点击"新建项目"
   - 输入项目名称（比如"Gemini-CLI-Project"）
   - 点击"创建"

**步骤2：启用 Generative Language API**
1. 在左侧菜单中，找到并点击"APIs和服务"→"库"
2. 在搜索框中输入"Generative Language API"
3. 点击搜索结果中的"Generative Language API"
4. 点击"启用"按钮

**步骤3：创建 API 密钥**
1. 在左侧菜单中，点击"APIs和服务"→"凭据"
2. 点击页面顶部的"+ 创建凭据"按钮
3. 从下拉菜单中选择"API 密钥"
4. 系统会生成一个 API 密钥，**立即复制并保存它**（格式类似：`AIzaSyD...`）

**步骤4：限制 API 密钥（安全建议）**
1. 点击刚创建的 API 密钥旁边的"编辑"按钮
2. 在"API 限制"部分，选择"限制密钥"
3. 勾选"Generative Language API"
4. 点击"保存"

请告诉我您现在看到了什么，或者您完成到了哪一步，我会继续指导您。

如果在任何步骤中遇到问题，请截图或描述您看到的界面，我会帮您解决。

非常好！您已经成功创建并限制了 API 密钥。现在让我们回到 Gemini CLI 中完成认证设置：

**步骤5：在 Gemini CLI 中使用 API Key**

1. **回到您的命令行终端**，应该还能看到 Gemini CLI 的认证选择界面

2. **选择 API Key 选项**
   ```
   使用方向键 ↓ 移动到 "Gemini API Key (AI Studio)" 选项
   按 Enter 确认选择
   ```

3. **输入 API Key**
   ```
   当提示输入 API Key 时，粘贴您刚才复制的 API Key
   （格式类似：AIzaSyD...）
   按 Enter 确认
   ```

4. **验证认证成功**
   - CLI 应该会显示认证成功的消息
   - 您应该能看到 Gemini CLI 的主界面或提示符

**如果认证成功，您应该能够：**
- 开始与 Gemini 对话
- 运行各种 Gemini CLI 命令
- 看到类似 `gemini>` 的提示符

**测试一下**
认证完成后，可以尝试发送一个简单的消息测试：
```
Hello, can you help me test this connection?
```

请告诉我：
1. 您是否成功进入了 API Key 输入界面？
2. 输入 API Key 后有什么反应？
3. 是否看到了认证成功的提示？

如果遇到任何错误信息，请告诉我具体的错误内容，我会帮您解决。

看到了！Gemini CLI 需要您设置环境变量而不是直接输入 API Key。让我们来设置环境变量：

**方法1：临时设置（推荐先试这个）**

在当前命令行窗口中运行：
```cmd
set GEMINI_API_KEY=您的API密钥
```

**替换"您的API密钥"为您刚才复制的实际 API Key**，例如：
```cmd
set GEMINI_API_KEY=AIzaSyD1234567890abcdefghijklmnop
```

然后重新运行：
```cmd
gemini
```

**方法2：永久设置（如果方法1有效）**

1. **通过系统设置**：
   ```
   1. 按 Win + R，输入 sysdm.cpl，按 Enter
   2. 点击"高级"选项卡
   3. 点击"环境变量"
   4. 在"用户变量"部分点击"新建"
   5. 变量名：GEMINI_API_KEY
   6. 变量值：您的API密钥
   7. 点击"确定"保存
   ```

2. **重新打开命令行窗口**测试

**方法3：创建 .env 文件**

在您当前的目录中创建一个名为 `.env` 的文件：
```cmd
echo GEMINI_API_KEY=您的API密钥 > .env
```

**现在请先尝试方法1**，在当前命令行中运行：
```cmd
set GEMINI_API_KEY=您的实际API密钥
gemini
```

告诉我执行后看到了什么结果！

# 37. Foxmail 6.5导入邮件

首先在Foxmail中创建一个新账户 lvwb09@tsinghua.edu.cn 

然后将移动硬盘 H:\03_THU\Mail\Thumail 

下所有文件拷贝到

D:\Program Files (x86)\Foxmail\mail\lvwb09@tsinghua.edu.cn

# 38. VS Code 配置 GitHub 代理

VS Code 中访问 GitHub 需要配置 Git 和 VS Code 的代理设置。

## 方法 1：配置 Git 全局代理（推荐）

打开终端（在 VS Code 中按 `Ctrl + ~`），运行：

```bash
# HTTP/HTTPS 代理
git config --global http.proxy http://127.0.0.1:7899
git config --global https.proxy http://127.0.0.1:7899

# 如果需要 SOCKS5 代理
git config --global http.proxy socks5://127.0.0.1:7900

# 查看配置
git config --global --list | grep proxy
```

## 查看代理

PS D:\27_Github\Today-I-Learned\Today-I-Learned> git config --global --list | Select-String proxy

http.proxy=http://127.0.0.1:7899 
https.proxy=http://127.0.0.1:7899

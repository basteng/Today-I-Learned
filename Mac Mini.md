- [1. 安装Homebrew](#1-安装homebrew)
  - [对于 macOS 用户，系统自带 bash、git 和 curl，在命令行输入 xcode-select --install 安装 CLT for Xcode 即可。](#对于-macos-用户系统自带-bashgit-和-curl在命令行输入-xcode-select---install-安装-clt-for-xcode-即可)
  - [接着，在终端输入以下几行命令设置环境变量：](#接着在终端输入以下几行命令设置环境变量)
  - [前往 Homebrew bottles 镜像使用帮助中「长期替换」一节设置好 HOMEBREW\_API\_DOMAIN 与 HOMEBREW\_BOTTLE\_DOMAIN。](#前往-homebrew-bottles-镜像使用帮助中长期替换一节设置好-homebrew_api_domain-与-homebrew_bottle_domain)
  - [前往 PyPI 镜像使用帮助中「Homebrew」一节设置好 HOMEBREW\_PIP\_INDEX\_URL。](#前往-pypi-镜像使用帮助中homebrew一节设置好-homebrew_pip_index_url)
  - [最后，在终端运行以下命令以安装 Homebrew / Linuxbrew：](#最后在终端运行以下命令以安装-homebrew--linuxbrew)
  - [安装成功后需将 brew 程序的相关路径加入到环境变量中：](#安装成功后需将-brew-程序的相关路径加入到环境变量中)
- [2. Mac Mini 网络配置指南](#2-mac-mini-网络配置指南)
  - [网络拓扑](#网络拓扑)
  - [一、查看网络信息](#一查看网络信息)
    - [查看本机 IP](#查看本机-ip)
    - [查看是否静态 IP / 网关](#查看是否静态-ip--网关)
    - [查看默认路由走哪个网口](#查看默认路由走哪个网口)
    - [查看上级路由器 IP（网关）](#查看上级路由器-ip网关)
    - [查看 DHCP 服务器是谁发的](#查看-dhcp-服务器是谁发的)
    - [扫描同网段所有设备](#扫描同网段所有设备)
    - [查看 ARP 表（找设备 MAC 地址）](#查看-arp-表找设备-mac-地址)
  - [二、在树莓派上设置 Mac Mini 静态 IP（DHCP 绑定）](#二在树莓派上设置-mac-mini-静态-ipdhcp-绑定)
    - [Step 1：确认 DHCP 服务](#step-1确认-dhcp-服务)
    - [Step 2：获取 Mac Mini 的 MAC 地址](#step-2获取-mac-mini-的-mac-地址)
    - [Step 3：在树莓派上创建绑定配置](#step-3在树莓派上创建绑定配置)
    - [Step 4：重启 NetworkManager 生效](#step-4重启-networkmanager-生效)
    - [Step 5：Mac Mini 重新获取 IP](#step-5mac-mini-重新获取-ip)
    - [Step 6：验证是否生效](#step-6验证是否生效)
  - [三、关闭 FileVault（让重启后可直接 SSH，无需登录）](#三关闭-filevault让重启后可直接-ssh无需登录)
    - [查看 FileVault 状态](#查看-filevault-状态)
    - [关闭 FileVault](#关闭-filevault)
    - [确认 SSH 服务已开启](#确认-ssh-服务已开启)
    - [重启 Mac Mini](#重启-mac-mini)
  - [四、SSH 连接方式](#四ssh-连接方式)

# 1. 安装Homebrew

参考 <https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/>

## 对于 macOS 用户，系统自带 bash、git 和 curl，在命令行输入 xcode-select --install 安装 CLT for Xcode 即可。

## 接着，在终端输入以下几行命令设置环境变量：

~~~
export HOMEBREW_BREW_GIT_REMOTE="https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git"
export HOMEBREW_CORE_GIT_REMOTE="https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git"
export HOMEBREW_INSTALL_FROM_API=1
# export HOMEBREW_API_DOMAIN
# export HOMEBREW_BOTTLE_DOMAIN
# export HOMEBREW_PIP_INDEX_URL
~~~

## 前往 Homebrew bottles 镜像使用帮助中「长期替换」一节设置好 HOMEBREW_API_DOMAIN 与 HOMEBREW_BOTTLE_DOMAIN。

~~~
echo 'export HOMEBREW_API_DOMAIN="https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles/api"' >> ~/.zprofile
echo 'export HOMEBREW_BOTTLE_DOMAIN="https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles"' >> ~/.zprofile
export HOMEBREW_API_DOMAIN="https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles/api"
export HOMEBREW_BOTTLE_DOMAIN="https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles"
~~~

<https://mirrors.tuna.tsinghua.edu.cn/help/homebrew-bottles/>

## 前往 PyPI 镜像使用帮助中「Homebrew」一节设置好 HOMEBREW_PIP_INDEX_URL。

~~~
export HOMEBREW_PIP_INDEX_URL="https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple"
~~~

<https://mirrors.tuna.tsinghua.edu.cn/help/pypi/>

## 最后，在终端运行以下命令以安装 Homebrew / Linuxbrew：

~~~
# 从镜像下载安装脚本并安装 Homebrew / Linuxbrew
git clone --depth=1 https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/install.git brew-install
/bin/bash brew-install/install.sh
rm -rf brew-install
~~~

## 安装成功后需将 brew 程序的相关路径加入到环境变量中：

~~~
test -r ~/.bash_profile && echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.bash_profile
test -r ~/.zprofile && echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
~~~

# 2. Mac Mini 网络配置指南

## 网络拓扑

```
上级路由/树莓派 (10.42.0.1)
    ↕ 无线
小米路由器（无线中继）
    ↕ 有线网线
Mac Mini
├── en0 以太网（有线）→ 10.42.0.105  ← 默认网口
└── en1 Wi-Fi（无线）→ 10.42.0.100
```

---

## 一、查看网络信息

### 查看本机 IP
```bash
ipconfig getifaddr en0      # 有线
ipconfig getifaddr en1      # 无线
```

### 查看是否静态 IP / 网关
```bash
networksetup -getinfo "Ethernet"
```

### 查看默认路由走哪个网口
```bash
route -n get default
# 看 interface 字段：en0 有线，en1 无线
```

### 查看上级路由器 IP（网关）
```bash
route -n get default | grep gateway
```

### 查看 DHCP 服务器是谁发的
```bash
ipconfig getpacket en0 | grep server_identifier
```

### 扫描同网段所有设备
```bash
for i in $(seq 1 254); do ping -c1 -W1 10.42.0.$i &>/dev/null && echo "10.42.0.$i up"; done
```

### 查看 ARP 表（找设备 MAC 地址）
```bash
arp -a
```

---

## 二、在树莓派上设置 Mac Mini 静态 IP（DHCP 绑定）

> 树莓派使用 NetworkManager 管理的 dnsmasq 作为 DHCP 服务器

### Step 1：确认 DHCP 服务
```bash
systemctl is-active NetworkManager   # 应返回 active
ps aux | grep dhcp | grep -v grep    # 确认 dnsmasq 在跑
```

### Step 2：获取 Mac Mini 的 MAC 地址
```bash
# 在 Mac Mini 上执行
networksetup -getinfo "Ethernet"
# 看 Ethernet Address 字段，例如：d0:11:e5:d3:5e:33
```

### Step 3：在树莓派上创建绑定配置
```bash
sudo nano /etc/NetworkManager/dnsmasq-shared.d/static-hosts.conf
```

写入（MAC地址对应固定IP，infinite表示永久租约）：
```
dhcp-host=d0:11:e5:d3:5e:33,10.42.0.105,infinite
```

### Step 4：重启 NetworkManager 生效
```bash
sudo systemctl restart NetworkManager
```

### Step 5：Mac Mini 重新获取 IP
```bash
sudo ipconfig set en0 DHCP
```

### Step 6：验证是否生效
```bash
# Mac Mini 上验证租约（lease_time 应为 0xffffffff 表示永久）
ipconfig getpacket en0

# 树莓派上查看租约记录
sudo cat /var/lib/NetworkManager/dnsmasq-wlan0.leases
```

---

## 三、关闭 FileVault（让重启后可直接 SSH，无需登录）

### 查看 FileVault 状态
```bash
fdesetup status
```

### 关闭 FileVault
```bash
sudo fdesetup disable
# 按提示输入用户名和密码
```

### 确认 SSH 服务已开启
```bash
sudo systemsetup -getremotelogin   # 应返回 Remote Login: On
sudo systemsetup -setremotelogin on  # 如果未开启则执行此命令
```

### 重启 Mac Mini
```bash
sudo reboot
```

重启后无需登录即可直接 SSH 连入。

---

## 四、SSH 连接方式

| 方式 | 地址 | 说明 |
|------|------|------|
| 有线 | `ssh wenbinlv@10.42.0.105` | 走 en0，推荐 |
| 无线 | `ssh wenbinlv@10.42.0.100` | 走 en1 |
| 跳板机 | MobaXterm gateway: `basteng@192.168.0.105` | 外网访问时用 |
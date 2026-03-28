

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


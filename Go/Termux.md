# 手机运行空投脚本方案，每一个脚本都适用
### 注意事项 
1. **先说一下问题哈，手机只能运行API方案的脚本，使用tgWebAppData，也就是query_id方案的脚本，弄不了，除非你有电脑**
2. **或者抓包获取query_id，这个对你们来说有点折腾，本文就不介绍了**


### 教程开始，首先安装Termux

[视频教程]()
**切记不要在Google Play下载，那个是旧版本，最好从Github或者使用F-Droid下载**
[Termux Github下载地址](https://github.com/termux/termux-app/releases)
[Termux F-Droid下载地址](https://f-droid.org/zh_Hans/packages/com.termux/)

### 使用它tmoe安装proot环境Ubuntu

```bash
. <(curl -L gitee.com/mo2/linux/raw/2/2)
```
**详情请看Youtube视频教程**
### 安装python3
    # 在 Linux 上使用 pyenv 安装 Python 3.10

### 首先安装依赖

在开始之前，确保你已安装一些必需的构建工具和库。这些依赖项对于编译 Python 是必需的。


```sh
sudo apt update
sudo apt install -y build-essential libssl-dev zlib1g-dev libbz2-dev \
    libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev \
    libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python3-openssl \
    git
```




### 安装 pyenv,克隆 `pyenv` 仓库

首先，你需要安装 Git。如果你还没有安装 Git，请使用适合你的发行版的命令安装。

然后，克隆 `pyenv` 的 Git 仓库到本地：

```sh
curl https://pyenv.run | bash
```
### 更新环境变量

添加 `pyenv` 到你的 shell 配置文件中。根据你使用的 shell 类型，执行以下步骤：


打开 `~/.bashrc` 文件并添加以下内容：

```sh
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv virtualenv-init -)"
```
然后，运行以下命令以使更改生效：

```bash
source ~/.bashrc
```
### 使用pyenv安装指定版本的python
现在，你可以使用 `pyenv` 安装 Python 3.10：

```bash
pyenv install 3.10.0
```
这将下载并编译 Python 3.10。根据网络速度和系统性能，这可能需要一些时间。

### 设置 Python 3.10 为全局版本
安装完成后，你可以将 Python 3.10 设置为默认的 Python 版本：
```bash
pyenv global 3.10.0
```
验证安装
使用以下命令检查 Python 版本，以确保 Python 3.10 已成功安装：
```bash
python --version
```
应该会看到输出 Python 3.10.0，这表示 Python 3.10 已成功安装并设置为默认版本。


### 然后就是安装git
```bash
apt install git
```
这个命令会安装git工具


### Vim 编辑器介绍

Vim 是一个高度可配置的文本编辑器，它广泛用于程序开发和文本编辑。Vim 是 Vi 编辑器的改进版，提供了许多高级功能，提升了用户的编辑效率。

Vim 有几种主要的模式，每种模式都有不同的功能和用途。最常用的模式包括：

#### 正常模式（Normal Mode）

- **功能**：这是 Vim 启动时的默认模式。你可以在这个模式下进行文本导航、删除、复制、粘贴等操作。
- **进入方式**：按 `Esc` 键可以返回到正常模式。

#### 插入模式（Insert Mode）

- **功能**：在插入模式下，你可以像普通文本编辑器那样输入文本。
- **进入方式**：从正常模式下，按 `i` 进入插入模式。其他进入插入模式的命令还有 `I`（在行首插入）、`a`（在光标后插入）、`A`（在行尾插入）、`o`（在当前行下方插入新行）等。

#### 命令行模式（Command-Line Mode）

- **功能**：在这个模式下，你可以执行各种命令，例如保存文件、退出 Vim、搜索文本等。
- **进入方式**：在正常模式下，按 `:` 进入命令行模式。

**保存文件**

在 Vim 中，保存文件通常需要使用命令行模式。以下是一些常用的保存命令：

- `:w`：保存当前文件，但不退出 Vim。
- `:w filename`：将当前编辑的内容保存为 `filename` 文件。
- `:x` 或 `:wq`：保存文件并退出 Vim。
- `:q!`：强制退出 Vim，不保存任何更改。

**切换模式示例**

1. **进入插入模式**：
   - 从正常模式按 `i` 键，进入插入模式，可以开始输入文本。

2. **返回正常模式**：
   - 在插入模式下，按 `Esc` 键返回正常模式。

3. **保存并退出**：
   - 在正常模式下，按 `:` 键进入命令行模式，然后输入 `wq` 并按 `Enter` 键保存文件并退出 Vim。

Vim 的高效编辑和强大的功能使其成为许多程序员和文本编辑者的首选工具。通过熟练掌握这些

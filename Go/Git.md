# Git for Windows 安装教程

## 为什么要安装git?

1. 找到自己要下载的目录，然后用git命令随时克隆仓库
2. 随时更新，不然下载的话，人家更新了还得重新删除原来的文件然后重新下载


## 下载 Git for Windows

1. 打开 [Git for Windows 发布页面](https://github.com/git-for-windows/git/releases)。
2. 在版本发布页面中，找到“Assets”部分，下载 `MinGit-2.46.0-64-bit.zip
`

## 安装 Git for Windows 配置环境变量

1. 右键解压这个压缩包
2. 然后打开控制面板 -> 系统和安全 -> 系统 -> 高级系统设置 -> 环境变量 
3. 在下面的内容库框里找到path。
4. 然后双击打开，新建 -> 浏览 -> 找到刚刚下载的文件夹，找到`MinGit-2.46.0-64-bit`文件中的`cmd`文件夹
5. 然后点确定，就成功了


## 验证安装

1. 打开命令提示符（CMD）或 PowerShell。
2. 输入以下命令以检查 Git 是否安装成功：
   ```bash
   git --version

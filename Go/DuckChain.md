
# DuckChain 自动养殖机器人
该机器人将在 DuckChain Telegram 机器人上执行“Quack”或点击操作，支持代理、多账户/多线程。注册⨠

[DuckChain链接](https://t.me/DuckChain_bot/quack?startapp=zrtrCpPw)

### 功能
- 自动 Quack / 点击
- 支持多账户 / 多线程
- 支持代理
- 可通过 `config.json` 进行配置


### 先决条件
在安装和运行此项目之前，请确保你具备以下先决条件：
- Python 3 版本 1.0.1+ = Python 3.10+
- 其他必要的依赖项

### 安装
1. 将此仓库克隆到本地机器：
    ```bash
    git clone https://github.com/jawikas/duckchain-bot.git
    ```
2. 进入项目目录：
    ```bash
    cd duckchain-bot
    ```
3. 原文档没有创建虚拟环境，经过测试，不创建虚拟环境会报错
    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```
4. 安装必要的依赖项：
    ```bash
    pip install -r requirements.txt
    ```

### 如果要用静态代理，请在`config.json`中添加配置设置

 **布尔值** : `true` 或 `false` | 开启或关闭代理

  ```bash
{
    "use_proxy": false,
    "quack_delay": 0.4
}
```
### 代理格式如下 `proxies.txt` 

  ```bash
username:password@proxy:port
  ```



### 使用方法
在启动机器人之前，你必须拥有自己的 initdata / queryid Telegram！为什么需要 query id？有了 query_id，会更加方便，因为你不必每次都更改 init 数据。

### 配置TOKEN需要打开Telegram WebView调试功能，请看Youtbe视频
1. 使用 PC/笔记本电脑打开Teleg
2. 打开 `DuckChain bot`
3. 按下键盘上的 `Inspect Element` `(F12)`
4. 在顶部选择 "`Application`"
5. 然后选择 "`Session Storage`"
6. 选择链接 "`DuckChain bot`" 和 "`tgWebAppData`"
7. 获取 "`tgWebAppData`" 的值部分
8. 获取如下格式的部分：以下为一个示例

```txt
query_id=xxxxxxxxx-Rxxxxuj&user=%7B%22id%22%3A1323733375%2C%22first_name%22%3A%22xxxx%22%2C%22last_name%22%3A%22%E7%9A%BF%20xxxxxx%22%2C%22username%22%3A%22xxxxx%22%2C%22language_code%22%3A%22id%22%2C%22allows_write_to_pm%22%3Atrue%7D&auth_date=xxxxx&hash=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
### 运行机器人
然后使用以下命令运行机器人：

```bash
python main.py
```


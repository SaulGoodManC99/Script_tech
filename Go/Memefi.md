# MemeFiBot 新手教程

欢迎使用 **MemeFiBot**！本教程将引导你完成在Linux和Windows系统上安装和运行 **MemeFiBot** 的步骤。

## 克隆代码库

找到自己想要下载的目录，用git命令克隆仓库

首先，克隆 **MemeFiBot** 的代码库到本地，你们也可以从github网页中下载下来

```bash
git clone https://github.com/shamhi/MemeFiBot.git
cd MemeFiBot 进入克隆的仓库目录
```
# MemeFiBot 

欢迎使用 **MemeFiBot**！以下是安装和运行 **MemeFiBot** 的步骤，分别适用于Linux和Windows系统。


## 先说配置文件 .env吧  

1. 一定要关闭windows文件管理器`隐藏已知文件类型的扩展名`
2. 不然看不到文件扩展名

``` python
API_ID=从频道获取
API_HASH=从频道获取
MIN_AVAILABLE_ENERGY=100
SLEEP_BY_MIN_ENERGY=200

ADD_TAPS_ON_TURBO=2500


主要看这里，升级点击，回能量，然后升级能量储值。`True`为开启 `False`位关闭
AUTO_UPGRADE_TAP=False
MAX_TAP_LEVEL=5
AUTO_UPGRADE_ENERGY=False
MAX_ENERGY_LEVEL=5
AUTO_UPGRADE_CHARGE=False
MAX_CHARGE_LEVEL=5
从这里结束
APPLY_DAILY_ENERGY=True
APPLY_DAILY_TURBO=True

RANDOM_TAPS_COUNT=[50,200]
SLEEP_BETWEEN_TAP=[10,25]

USE_TAP_BOT=True
EMERGENCY_STOP=True

USE_PROXY_FROM_FILE=False
```
## Windows 系统

1. 创建虚拟环境：

    ```bash
    python -m venv venv
    ```

2. 激活虚拟环境：

    ```bash
    venv\Scripts\activate
    ```

3. 安装依赖：

    ```bash
    pip install -r requirements.txt
    ```

4. 复制示例环境文件：

    ```bash
    copy .env-example .env
    ```

5. 编辑 `.env` 文件，指定你的 `API_ID` 和 `API_HASH`，其余设置保持默认：

    ```text
    # 使用文本编辑器打开 .env 文件并进行编辑
    ```

6. 运行 **MemeFiBot**：

    ```bash
    python main.py
    ```
7. 运行机器人

    ```python
    先选择1然后，取一个名称，不然你开代理ip多开，后面就不知道这是哪个账号了。
    proxy那里直接留空回车，除非你要用代理。
    然后输入号码，格式如下
    +86***********
    举个例：柬埔寨，这样输入
    +855******

    ```
## Linux 系统

1. 创建虚拟环境：

    ```bash
    python3 -m venv venv
    ```

2. 激活虚拟环境：

    ```bash
    source venv/bin/activate
    ```

3. 安装依赖：

    ```bash
    pip3 install -r requirements.txt
    ```

4. 复制示例环境文件：

    ```bash
    cp .env-example .env
    ```

5. 编辑 `.env` 文件，指定你的 `API_ID` 和 `API_HASH`，其余设置保持默认：

    ```bash
    nano .env
    ```

6. 运行 **MemeFiBot**：

    ```bash
    python3 main.py
    ```



## 注意事项

- 确保在 `.env` 文件中正确填写 `API_ID` 和 `API_HASH`。这些信息可以从 [Telegram API](https://my.telegram.org/) 获取，或者从频道获取。




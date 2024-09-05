# TimeFarm脚本运行教程

[TimeFarm空投链接](https://t.me/TimeFarmCryptoBot?start=Lj81LtA84TFprV5q)

## [设置](https://github.com/SudoLite/TimeFarmBot/blob/main/.env-example)
| 设置                      | 描述                                                                         |
|---------------------------|-------------------------------------------------------------------------------|
| **API_ID / API_HASH**     | 启动Telegram会话所需的平台数据（默认是Android）                               |
| **CLAIM_RETRY**           | 如果**Claim**不成功，重试的次数 _(例如: 3)_                                  |
| **SLEEP_BETWEEN_CLAIM**   | 两次**Claim**之间的延迟时间，以分钟为单位 _(例如: 180)_                       |
| **AUTO_UPGRADE_FARM**     | 是否提升农场等级 _(True / False)_                                             |
| **MAX_UPGRADE_LEVEL**     | 农场的最高等级 _(最高4级)_                                                   |
| **USE_PROXY_FROM_FILE**   | 是否使用`bot/config/proxies.txt`文件中的代理 (True / False)                   |





## 下载安装命令
您可以通过克隆[**仓库**](https://github.com/SudoLite/TimeFarmBot)到您的系统并安装所需的依赖项来下载：
```shell
git clone https://github.com/SudoLite/TimeFarmBot.git
cd TimeFarmBot
```
# Linux系统或者说安卓系统
```
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
cp .env-example .env
编辑.env配置文件
python3 main.py
```
# Windows系统
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
编辑.env配置文件
python main.py
```

## .env配置
``` bash
API_ID=自行注册，频道获取
API_HASH=自行注册，频道获取

CLAIM_RETRY=2
SLEEP_BETWEEN_CLAIM=5

AUTO_UPGRADE_FARM=True
MAX_UPGRADE_LEVEL=4

USE_PROXY_FROM_FILE=False
```

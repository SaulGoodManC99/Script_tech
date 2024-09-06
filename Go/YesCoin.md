# YesCoin脚本运行教程

[Yescoin空投链接](https://t.me/theYescoin_bot/Yescoin?startapp=YDNl0h)

## 第一步克隆仓库（下载脚本）
```bash
git clone https://github.com/shamhi/YesCoinBot.git 

cd YesCoinBot
```

## 第二步创建虚拟环境，安装依赖，运行脚本
```bash
# Windows
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
编辑你的.env配置
python main.py
```
然后登陆账号，或者从别的脚本那里直接复制账号session到脚本目录也是可以的
视频会演示


## .env配置
我这边关掉了自动升级，你们自己看一下配置
```bash
AUTO_UPGRADE_TAP=False 点击升级，已关闭，要打开改为True
MAX_TAP_LEVEL=20 最高等级
AUTO_UPGRADE_ENERGY=False 能量升级，已关闭，要打开改为True
MAX_ENERGY_LEVEL=20 最高等级
AUTO_UPGRADE_CHARGE=False 回能量升级，已关闭，要打开改为True
MAX_CHARGE_LEVEL=5 最高等级
```
然后在.env文件更改你要的配置
```bash
API_ID=自行注册或者频道获取，推荐自行注册
API_HASH=自行注册或者频道获取，推荐自行注册

MIN_AVAILABLE_ENERGY=100
SLEEP_BY_MIN_ENERGY=200

AUTO_UPGRADE_TAP=False
MAX_TAP_LEVEL=20
AUTO_UPGRADE_ENERGY=False
MAX_ENERGY_LEVEL=20
AUTO_UPGRADE_CHARGE=False
MAX_CHARGE_LEVEL=5

APPLY_DAILY_ENERGY=True
APPLY_DAILY_TURBO=True

RANDOM_TAPS_COUNT=50,200
SLEEP_BETWEEN_TAP=10,25
USE_PROXY_FROM_FILE=False
```


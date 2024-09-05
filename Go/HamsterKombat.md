# HamsterKombatBot脚本运行教程

## 下载安装命令
您可以通过克隆[**仓库**](https://github.com/shamhi/HamsterKombatBot)到您的系统并安装所需的依赖项来下载：
```shell
git clone https://github.com/shamhi/HamsterKombatBot.git 
cd HamsterKombatBot
```
# Linux系统或者说安卓系统
```
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
cp .env-example .env
nano .env  # 输入您的 API_ID 和 API_HASH
python3 main.py
```
# Windows系统
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
编辑 .env  # 输入您的 API_ID 和 API_HASH
python main.py
```


## .env配置文件说明看老外主页
[跳转](https://github.com/shamhi/HamsterKombatBot)

## .env文件配置
[api注册教程视频链接](https://www.youtube.com/watch?v=TWreKchDMWc&t=3s)
```
APPLY_COMBO=False
设置为关闭，不参与combo，就是每天三张卡那个
有的卡片太贵了，升级了还感觉亏了，所以关闭了 要开启请设置为True
```
```bash
API_ID=频道获取或者自行注册
API_HASH=频道获取或者自行注册


MIN_AVAILABLE_ENERGY=200
SLEEP_BY_MIN_ENERGY=[1800,3600]

AUTO_UPGRADE=True
MAX_LEVEL=20
MAX_PRICE=50000000

BALANCE_TO_SAVE=1000000
UPGRADES_COUNT=10

MAX_COMBO_PRICE=10000000

APPLY_COMBO=False
APPLY_PROMO_CODES=True
APPLY_DAILY_CIPHER=True
APPLY_DAILY_REWARD=True
APPLY_DAILY_ENERGY=True
APPLY_DAILY_MINI_GAME=True

SLEEP_MINI_GAME_TILES=[600,900]
SCORE_MINI_GAME_TILES=[300,500]
GAMES_COUNT=[1,10]

AUTO_COMPLETE_TASKS=True

USE_TAPS=True
RANDOM_TAPS_COUNT=[10,50]
SLEEP_BETWEEN_TAP=[10,25]

USE_RANDOM_DELAY_IN_RUN=True
RANDOM_DELAY_IN_RUN=[0,15]

USE_RANDOM_USERAGENT=True

```

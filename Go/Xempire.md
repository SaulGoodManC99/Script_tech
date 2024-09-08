# XEmpireBot 安装教程

### 功能支持
| 功能                           | 支持 |
|--------------------------------|------|
| 多线程                         | ✅   |
| 将代理绑定到会话                | ✅   |
| 每次会话前等待                  | ✅   |
| 领取每日奖励                    | ✅   |
| 领取好友奖励                    | ✅   |
| 领取任务奖励                    | ✅   |
| 领取离线奖励                    | ✅   |
| 自动点击                        | ✅   |
| PvP 谈判                        | ✅   |
| 每日测验和谜题解决              | ✅   |
| 投资基金（利润组合）            | ✅   |
| 自动技能提升                    | ✅   |
| Docker 支持                     | ✅   |

### 配置选项
| 选项                       | 描述                                                         |
|----------------------------|--------------------------------------------------------------|
| API_ID / API_HASH          | 启动 Telegram 会话所需的平台注册数据                           |
| TAPS_ENABLED               | 是否启用点击（True / False）                                   |
| TAPS_PER_SECOND            | 每秒点击的随机数（例如 [20,30]，最大值 30）                    |
| INVEST_ENABLED             | 是否启用投资（True / False）                                   |
| PVP_ENABLED                | 是否启用 PvP 谈判（True / False）                              |
| PVP_LEAGUE                 | 谈判中的联赛（例如 bronze 或 auto 自动选择）                   |
| PVP_UPGRADE_LEAGUE         | 如果指定的 PVP_LEAGUE 联赛不可用，是否升级联赛（True / False） |
| PVP_STRATEGY               | 谈判策略（例如 random）                                       |
| PVP_COUNT                  | 每轮谈判的数量（例如 10）                                      |
| SKILLS_COUNT               | 每轮提升的利润技能数量（例如 10）                             |
| SKILLS_MODE                | 技能选择模式（例如 profitness）                               |
| IGNORED_SKILLS             | 机器人不会提升的技能（例如 ["agi", "voice_assistant", "translators"]） |
| MINING_SKILLS_LEVEL        | 最大提升的采矿技能等级（例如 10）                             |
| PROTECTED_BALANCE          | 保护余额，防止用于 PvP、投资和技能（例如 100000000）          |
| REF_CODE                   | 邀请链接中的代码（例如 hero123456），如果未提供，将使用我的代码 |
| SLEEP_BETWEEN_START        | 每次会话开始前的等待时间（例如 [20, 360]）                     |
| ERRORS_BEFORE_STOP         | 机器人在停止之前的失败请求次数                                |
| USE_PROXY_FROM_FILE        | 是否使用 proxies.txt 文件中的代理（True / False）              |

**注意：** 可以在 [my.telegram.org/apps](https://my.telegram.org/apps) 创建应用以获取 API_ID 和 API_HASH。



### Windows快速启动脚本

1. 确保已安装 Python 3.10 或更高版本。
   **注意：** 如果使用 Python 3.12，在进行下一步之前，需要从 requirements.txt 中移除 TgCrypto 行（TgCrypto 不是关键的），或者安装自动编译此软件包所需的软件。
2. 使用 `INSTALL.bat` 进行安装，然后在 `.env` 文件中指定你的 API_ID 和 API_HASH。
3. 使用 `START.bat` 启动机器人（或在控制台中运行 `python main.py`）。

4. 克隆代码仓库或者在网页端下载：
   ```sh
   git clone https://github.com/Alexell/XEmpireBot.git && cd XEmpireBot
  ```



### .env配置文件
从配置选项中查看并修改自己想要的配置

```python
API_ID=从频道获取或者自行注册
API_HASH=从频道获取或者自行注册
TAPS_ENABLED=True
TAPS_PER_SECOND=[20,30]
INVEST_ENABLED=True 
PVP_ENABLED=True 
PVP_LEAGUE=auto
PVP_UPGRADE_LEAGUE=True 
PVP_STRATEGY=random
PVP_COUNT=10
SKILLS_COUNT=10 
SKILLS_MODE=profitness
IGNORED_SKILLS=["agi", "voice_assistant", "translators"]
MINING_SKILLS_LEVEL=10
PROTECTED_BALANCE=1000000000
REF_CODE=
SLEEP_BETWEEN_START=[20, 360]
ERRORS_BEFORE_STOP=
USE_PROXY_FROM_FILE=False
DEBUG_MODE=False
```


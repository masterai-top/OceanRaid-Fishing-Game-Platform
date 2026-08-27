# OceanRaid 捕鱼游戏全栈源码 | Arcade Fishing Game Source Code

> Cocos 客户端 + Python/C++ 游戏服务端 + Node.js 运营后台的多人街机捕鱼游戏平台源码。

[简体中文](README.md) | [English](README.en.md) | [在线文档](https://masterai-top.github.io/OceanRaid-Fishing-Game-Platform/) | [商业授权](LICENSE)

![Cocos](https://img.shields.io/badge/client-Cocos-55C2E1)
![Python](https://img.shields.io/badge/server-Python-3776AB?logo=python&logoColor=white)
![C++](https://img.shields.io/badge/core-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![Node.js](https://img.shields.io/badge/admin-Node.js-339933?logo=nodedotjs&logoColor=white)
![License](https://img.shields.io/badge/license-commercial-orange)

OceanRaid 是一套面向移动端和街机娱乐产品的捕鱼游戏全栈项目，覆盖客户端、实时游戏服务、运营管理后台以及多玩法入口。仓库适用于合法的软件评估、技术研究、二次开发和商业授权洽谈。

## 核心捕鱼玩法



### 1️⃣ 经典模式 | Classic Mode
| 场景 | 倍数范围 |
|------|----------|
| 海妖漩涡 | 1 - 30000倍 |
| 新手滩 | 1 - 30000倍 |
| 深海巨兽 | 1 - 30000倍 |
| 幽灵船长 | 1 - 30000倍 |

### 2️⃣ 比赛模式 | Tournament Mode
- 实时多人竞技
- 排行榜系统
- 丰厚奖励机制

### 3️⃣ 玉石场 | Jade Field
| 场景 | 倍数范围 |
|------|----------|
| 亡灵废墟 | 5000 - 10000倍 |
| 天宫乱斗 | 5000 - 10000倍 |

### 4️⃣ 找刺激 | Thrill Zone
| 游戏 | 类型 |
|------|------|
| 弹头夺宝 | 休闲竞技 |
| 四国征战 | 策略对战 |
| 宝石迷城 | 消除闯关 |
| 斗地主 | 棋牌 |
| 麻将 | 棋牌 |
| 拼十 | 棋牌 |
| 王者战绩 | 竞技 |
| 水浒传 | 老虎机 |
| 好运连连 | 转盘 |
| 龙虎斗 | 棋牌 |
| 红黑大战 | 棋牌 |
## 扩展休闲玩法

弹头夺宝、四国征战、宝石迷城、斗地主、麻将、拼十、王者战绩、水浒传、好运连连、龙虎斗和红黑大战。

> 玩法名称、倍率和可用模块以实际交付版本及当地法律要求为准。涉及支付、虚拟物品、概率、竞赛或奖励的功能，上线前必须完成目标地区的法律、平台政策和未成年人保护审查。

## 产品能力

- 百种鱼类与多套首领、生物和海域场景资源
- 多房间、多炮台、多人实时同步与赛事流程
- 活动、任务、排行、配置、日志和运营数据管理
- Cocos 客户端，Python/C++ 服务端，Node.js 运营后台
- 面向 Android、iOS 和定制终端的二次开发基础
- 管理员分级权限、参数配置、操作日志与风险控制扩展点

## 技术架构

```text
Cocos Client
     |
     v
Gateway / Session Services
     |
     +--> Python business services
     +--> C++ real-time game services
     +--> Match, room and fishing engines
     +--> Database, cache and message services
     |
Node.js Operations Console
```

具体数据库、中间件、部署版本和外部依赖应以实际源码中的配置与部署文档为准，不应仅根据本介绍推断可以一键上线。

## 项目结构

```text
client/                 # Cocos 客户端源码
server-python/          # Python 业务服务
server-cpp/             # C++ 实时游戏与房间服务
admin/                  # Node.js 运营后台
database/               # 数据库结构与迁移（移除真实数据）
config.example/         # 脱敏配置示例
scripts/                # 构建和部署辅助脚本
docs/                   # GitHub Pages 产品与技术文档
tests/                  # 自动化测试和验证用例
.github/workflows/      # CI 与 GitHub Pages 工作流
```

## 产品截图

发布前请把真实截图放入 `docs/assets/screenshots/`，保持以下文件名：

| 画面 | 上传文件名 |
| --- | --- |
| 游戏大厅 | `docs/assets/screenshots/lobby.webp` |
| 经典捕鱼 | `docs/assets/screenshots/classic-mode.webp` |
| 比赛模式 | `docs/assets/screenshots/tournament-mode.webp` |
| 海魔来袭 | `docs/assets/screenshots/sea-demon.webp` |
| 玉石场 | `docs/assets/screenshots/jade-arena.webp` |
| 运营后台 | `docs/assets/screenshots/admin-console.webp` |



📊 运营数据 | Operation Data
指标	数据
日流水	¥6,500,000+
日活跃用户	50,000+
在线峰值	8,000+
付费率	18.6%
ARPU	¥130+

📞 联系方式 | Contact
如有任何问题或意向，欢迎联系：

Telegram: @xuzongbin001

Email: masterai918@gmail.com


⭐ Star History
如果这个项目对你有帮助，请给一个 Star ⭐ 支持一下！
## 关键词

捕鱼源码、捕鱼游戏源码、街机捕鱼源码、Cocos 捕鱼游戏、多人捕鱼服务端、捕鱼运营后台、arcade fishing game source code、fish shooting game、Cocos game client、Python game server、C++ game server、Node.js admin dashboard。

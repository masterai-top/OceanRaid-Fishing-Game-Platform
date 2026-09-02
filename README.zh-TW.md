[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md)

# OceanRaid 多人街機捕魚遊戲平台

> 採用 Cocos 用戶端 + Python/C++ 遊戲伺服器 + Node.js 營運後台的多人街機捕魚遊戲平台原始碼。


![Cocos](https://img.shields.io/badge/client-Cocos-55C2E1)
![Python](https://img.shields.io/badge/server-Python-3776AB?logo=python&logoColor=white)
![C++](https://img.shields.io/badge/core-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![Node.js](https://img.shields.io/badge/admin-Node.js-339933?logo=nodedotjs&logoColor=white)
![License](https://img.shields.io/badge/license-commercial-orange)


OceanRaid 是一套面向行動裝置與街機娛樂產品的捕魚遊戲全端專案，涵蓋用戶端、即時遊戲服務、營運管理後台以及多種玩法入口。此儲存庫適用於合法的軟體評估、技術研究、二次開發和商業授權洽談。


> **目前公開範圍：** `server-python/`、`server-cpp/`、`admin/`、`database/` 與測試構成可執行的 `0.1.0` 基礎框架。公開的 `client/src/` 目前包含好友、登入、設定相關 Lua 模組及部分 Windows 執行函式庫，並不是可在乾淨環境獨立重建的完整 Cocos 用戶端。玩法、截圖與歷史營運數據屬於產品資料；完整商業交付應以書面清單和驗收結果為準。詳見 [PUBLIC-SCOPE.md](PUBLIC-SCOPE.md)。


## 核心捕魚玩法


### 1. 經典模式 | Classic Mode


| 場景 | 倍率範圍 |
| --- | --- |
| 海妖漩渦 | 1–30000 倍 |
| 新手灘 | 1–30000 倍 |
| 深海巨獸 | 1–30000 倍 |
| 幽靈船長 | 1–30000 倍 |


### 2. 比賽模式 | Tournament Mode


- 即時多人競技
- 排行榜系統
- 豐富獎勵機制


### 3. 玉石場 | Jade Field


| 場景 | 倍率範圍 |
| --- | --- |
| 亡靈廢墟 | 5000–10000 倍 |
| 天宮亂鬥 | 5000–10000 倍 |


### 4. 找刺激 | Thrill Zone


| 遊戲 | 類型 |
| --- | --- |
| 彈頭奪寶 | 休閒競技 |
| 四國征戰 | 策略對戰 |
| 寶石迷城 | 消除闖關 |
| 鬥地主 | 棋牌 |
| 麻將 | 棋牌 |
| 拼十 | 棋牌 |
| 王者戰績 | 競技 |
| 水滸傳 | 拉霸遊戲 |
| 好運連連 | 轉盤 |
| 龍虎鬥 | 棋牌 |
| 紅黑大戰 | 棋牌 |


## 擴充休閒玩法


彈頭奪寶、四國征戰、寶石迷城、鬥地主、麻將、拼十、王者戰績、水滸傳、好運連連、龍虎鬥和紅黑大戰。


> 玩法名稱、倍率和可用模組以實際交付版本及當地法律要求為準。涉及支付、虛擬物品、機率、競賽或獎勵的功能，上線前必須完成目標地區的法律、平台政策和未成年人保護審查。


## 產品能力


- 上百種魚類與多套首領、生物和海域場景資源
- 多房間、多砲台、多人即時同步與賽事流程
- 活動、任務、排行、設定、日誌和營運資料管理
- Cocos 用戶端、Python/C++ 伺服器與 Node.js 營運後台
- 面向 Android、iOS 和客製化終端的二次開發基礎
- 管理員分級權限、參數設定、操作日誌與風險控制擴充點


## 技術架構


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


實際資料庫、中介軟體、部署版本和外部依賴應以原始碼中的設定與部署文件為準，不應僅根據本介紹推斷可以一鍵上線。


## 專案結構


```text
client/                 # Cocos 用戶端原始碼
server-python/          # Python 業務服務
server-cpp/             # C++ 即時遊戲與房間服務
admin/                  # Node.js 營運後台
database/               # 資料庫結構與遷移（移除真實資料）
config.example/         # 去識別化設定範例
scripts/                # 建置和部署輔助指令碼
docs/                   # GitHub Pages 產品與技術文件
tests/                  # 自動化測試和驗證案例
.github/workflows/      # CI 與 GitHub Pages 工作流程
```


## 產品截圖


| 遊戲大廳 | 經典大廳 | 經典捕魚 |
| --- | --- | --- |
| ![OceanRaid 捕魚遊戲大廳](docs/assets/screenshots/lobby.png) | ![OceanRaid 經典捕魚大廳](docs/assets/screenshots/jingdian.png) | ![經典捕魚遊戲畫面](docs/assets/screenshots/classic-mode.png) |


| 比賽模式 | 海魔來襲大廳 | 海魔來襲 |
| --- | --- | --- |
| ![多人捕魚比賽模式](docs/assets/screenshots/tournament-mode.png) | ![海魔來襲大廳](docs/assets/screenshots/haimo.png) | ![海魔來襲捕魚玩法](docs/assets/screenshots/haimo.png) |


| 玉石大廳 | 玉石場 | 捕魚戰鬥畫面 |
| --- | --- | --- |
| ![捕魚玉石場大廳](docs/assets/screenshots/yushidating.png) | ![玉石場捕魚玩法](docs/assets/screenshots/jade-arena.jpg) | ![多人捕魚戰鬥畫面](docs/assets/screenshots/zhandou2.jpg) |


| 戰鬥場景 | 小遊戲入口一 | 小遊戲入口二 |
| --- | --- | --- |
| ![捕魚戰鬥場景](docs/assets/screenshots/zhandou3.jpg) | ![捕魚大廳小遊戲入口](docs/assets/screenshots/xiaoyouxi1.png) | ![休閒小遊戲列表](docs/assets/screenshots/xiaoyouxi2.png) |


## 營運資料


| 指標 | 資料 |
| --- | ---: |
| 每日流水 | ¥6,500,000+ |
| 每日活躍使用者 | 50,000+ |
| 同時在線峰值 | 8,000+ |
| 付費率 | 18.6% |
| ARPU | ¥130+ |


## 公開框架驗證


- Python 3.11+：`server-python/` 中的 FastAPI 閘道與 pytest 測試。
- CMake 3.20+ 與 C++17：`server-cpp/` 中的房間／捕魚引擎範例。
- Node.js 20+：`admin/` 中的 Express 營運 API 與 Node Test。
- Windows PowerShell 可執行 `./scripts/validate.ps1` 完成整體檢查。


以上命令只驗證公開框架，不代表完整歷史產品已通過正式環境驗收。
## MasterAI和德州项目


- [MasterAI 游戏项目主页](https://github.com/masterai-top)
- [德州俱乐部](https://github.com/masterai-top/TexasHoldem-Poker-Complete-Solution)
- [德州扑克赛事平台](https://github.com/masterai-top/Texas-Holdem-Poker-Tournament-Event-Platform)
- [德州金币大厅](https://github.com/masterai-top/Texas-Hold-em-Points-Lobby)
- [德州扑克 AI](https://github.com/masterai-top/cfr-poker-ai-masterai)
## 聯絡方式


如有任何問題或合作意向，歡迎聯絡：


- Telegram：`@xuzongbin001`
- Email：`masterai918@gmail.com`


## Star History


如果這個專案對您有幫助，請給予一個 Star 支持。


## 關鍵字


捕魚原始碼、捕魚遊戲原始碼、街機捕魚原始碼、Cocos 捕魚遊戲、多人捕魚伺服器、捕魚營運後台、arcade fishing game source code、fish shooting game、Cocos game client、Python game server、C++ game server、Node.js admin dashboard。

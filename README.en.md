[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md)

# OceanRaid Multiplayer Arcade Fishing Game Platform

> A multiplayer arcade fishing game platform featuring a Cocos client, Python/C++ game servers, and a Node.js operations console.


![Cocos](https://img.shields.io/badge/client-Cocos-55C2E1)
![Python](https://img.shields.io/badge/server-Python-3776AB?logo=python&logoColor=white)
![C++](https://img.shields.io/badge/core-C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![Node.js](https://img.shields.io/badge/admin-Node.js-339933?logo=nodedotjs&logoColor=white)
![License](https://img.shields.io/badge/license-commercial-orange)


OceanRaid is a full-stack arcade fishing game project for mobile and arcade entertainment products. It covers the game client, real-time game services, an operations management console, and access to multiple game modes. This repository is intended for lawful software evaluation, technical research, secondary development, and commercial licensing discussions.


> **Current public scope:** `server-python/`, `server-cpp/`, `admin/`, `database/`, and the tests form a runnable `0.1.0` foundation scaffold. The public `client/src/` currently contains Lua modules for friends, login, and settings plus selected Windows runtime libraries; it is not a complete Cocos client that can be rebuilt independently from a clean environment. Modes, screenshots, and historical operating figures are product material. Complete commercial delivery must be verified against a written inventory and acceptance results. See [PUBLIC-SCOPE.md](PUBLIC-SCOPE.md).


## Core Fishing Modes


### 1. Classic Mode


| Scene | Multiplier Range |
| --- | --- |
| Kraken Vortex | 1x–30,000x |
| Rookie Beach | 1x–30,000x |
| Deep-Sea Giants | 1x–30,000x |
| Ghost Captain | 1x–30,000x |


### 2. Tournament Mode


- Real-time multiplayer competition
- Leaderboard system
- Reward system


### 3. Jade Field


| Scene | Multiplier Range |
| --- | --- |
| Undead Ruins | 5,000x–10,000x |
| Celestial Palace Clash | 5,000x–10,000x |


### 4. Thrill Zone


| Game | Type |
| --- | --- |
| Warhead Treasure Hunt | Casual competition |
| Four Kingdoms | Strategy battle |
| Gem Maze | Match and level progression |
| Dou Dizhu | Card game |
| Mahjong | Tile game |
| Pin Shi | Card game |
| Champion Records | Competitive game |
| Water Margin | Slot game |
| Lucky Streak | Wheel game |
| Dragon Tiger | Card game |
| Red vs Black | Card game |


## Additional Casual Games


Warhead Treasure Hunt, Four Kingdoms, Gem Maze, Dou Dizhu, Mahjong, Pin Shi, Champion Records, Water Margin, Lucky Streak, Dragon Tiger, and Red vs Black.


> Game names, multipliers, and available modules depend on the version delivered and applicable local laws. Any features involving payments, virtual items, probabilities, competitions, or rewards must undergo legal, platform-policy, and minor-protection reviews for the target market before launch.


## Product Capabilities


- Hundreds of fish species and multiple sets of bosses, creatures, and ocean scenes
- Multiple rooms, multiple cannons, real-time multiplayer synchronization, and tournament workflows
- Activities, missions, rankings, configuration, logs, and operations data management
- Cocos client, Python/C++ servers, and Node.js operations console
- A foundation for secondary development targeting Android, iOS, and customized terminals
- Extension points for role-based administrator permissions, parameter configuration, operation logs, and risk controls


## Technical Architecture


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


The actual databases, middleware, deployment versions, and external dependencies must be verified against the configuration and deployment documentation included with the source code. This overview alone must not be interpreted as a guarantee of one-click deployment.


## Project Structure


```text
client/                 # Cocos client source code
server-python/          # Python business services
server-cpp/             # C++ real-time game and room services
admin/                  # Node.js operations console
database/               # Database schemas and migrations (production data removed)
config.example/         # Sanitized configuration examples
scripts/                # Build and deployment helper scripts
docs/                   # GitHub Pages product and technical documentation
tests/                  # Automated tests and validation cases
.github/workflows/      # CI and GitHub Pages workflows
```


## Product Screenshots


| Game Lobby | Classic Lobby | Classic Fishing |
| --- | --- | --- |
| ![OceanRaid arcade fishing game lobby](docs/assets/screenshots/lobby.png) | ![OceanRaid classic fishing lobby](docs/assets/screenshots/jingdian.png) | ![Classic fish-shooting gameplay](docs/assets/screenshots/classic-mode.png) |


| Tournament Mode | Sea Demon Lobby | Sea Demon Assault |
| --- | --- | --- |
| ![Multiplayer fishing tournament mode](docs/assets/screenshots/tournament-mode.png) | ![Sea Demon Assault lobby](docs/assets/screenshots/haimo.png) | ![Sea Demon Assault fishing gameplay](docs/assets/screenshots/haimo.png) |


| Jade Lobby | Jade Field | Fishing Battle |
| --- | --- | --- |
| ![Jade Field fishing lobby](docs/assets/screenshots/yushidating.png) | ![Jade Field fishing gameplay](docs/assets/screenshots/jade-arena.jpg) | ![Multiplayer fishing battle](docs/assets/screenshots/zhandou2.jpg) |


| Battle Scene | Mini-Game Menu 1 | Mini-Game Menu 2 |
| --- | --- | --- |
| ![Arcade fishing battle scene](docs/assets/screenshots/zhandou3.jpg) | ![Fishing hall mini-game menu](docs/assets/screenshots/xiaoyouxi1.png) | ![Casual mini-game selection](docs/assets/screenshots/xiaoyouxi2.png) |


## Operation Data


| Metric | Data |
| --- | ---: |
| Daily turnover | ¥6,500,000+ |
| Daily active users | 50,000+ |
| Peak concurrent users | 8,000+ |
| Paying-user rate | 18.6% |
| ARPU | ¥130+ |


## Public Scaffold Validation


- Python 3.11+: FastAPI gateway and pytest tests under `server-python/`.
- CMake 3.20+ and C++17: room/fishing engine example under `server-cpp/`.
- Node.js 20+: Express operations API and Node Test under `admin/`.
- On Windows PowerShell, run `./scripts/validate.ps1` for the combined checks.


These commands validate only the public scaffold; they do not certify the complete historical product for production.


## Contact


For questions or business inquiries, please contact:


- Telegram: `@xuzongbin001`
- Email: `masterai918@gmail.com`


## Star History


If this project is useful to you, please support it with a Star.


## Keywords


Arcade fishing game source code, fishing game source code, fish-shooting game source code, Cocos fishing game, multiplayer fishing server, fishing game operations console, Cocos game client, Python game server, C++ game server, Node.js admin dashboard.

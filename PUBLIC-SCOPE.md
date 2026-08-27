# Public Repository Scope

This file separates the product material from source that is currently verifiable in the public repository.

## Verifiable public source

- `client/src/`: Lua modules for friends, login, and settings, plus selected Windows runtime libraries and helper batch files.
- `server-python/`: OceanRaid gateway scaffold `0.1.0`, Python 3.11+, FastAPI, configuration, room catalog, and pytest tests.
- `server-cpp/`: CMake 3.20+, C++17 fishing/room engine example and a CTest executable.
- `admin/`: private Node.js 20+ Express operations API scaffold with configuration validation and Node Test.
- `database/`: schema and development seed examples.
- `config.example/`, `scripts/`, and `tests/integration/`: sanitized configuration, helper scripts, and repository-contract tests.
- `docs/assets/screenshots/`: product screenshots supplied by the project owner.

## Not verified as complete

- A cleanly rebuildable full Cocos client, including complete scenes, assets, engine metadata, build profiles, and platform projects.
- Complete historical production Python/C++ services, operations console, databases, middleware, deployment manifests, and observability stack.
- Full implementations of every fishing mode, mini-game, multiplier, payment, reward, ranking, or tournament shown in product material.
- Independent verification of historical revenue, DAU, concurrency, conversion, or ARPU figures.
- A production security, fairness, privacy, performance, or regulatory audit.

Recommended description: “Arcade fishing product material with a partial Lua client archive and runnable Python, C++, Node.js, database, configuration, and test scaffolds.”

Do not represent the public tree as a complete, audited, one-click production release until a clean environment can build and test the complete delivery.

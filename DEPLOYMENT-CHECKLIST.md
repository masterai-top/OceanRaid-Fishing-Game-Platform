# Deployment Checklist

## Source and licensing

- Confirm a written inventory of client, server, admin, database, assets, SDKs, fonts, audio, and platform projects.
- Verify ownership and redistribution rights for every binary and media asset.
- Review `LICENSE` and the commercial agreement before use beyond evaluation or authorized demonstration.

## Build and testing

- Pin Python, C++, Node.js, database, Cocos/Lua, and operating-system versions.
- Build all components from a clean environment; do not rely on bundled DLLs as proof of reproducibility.
- Run Python, C++, Node.js, and repository-contract tests, then add protocol, load, reconnect, settlement, and failure tests.
- Record checksums and generate a software bill of materials for releases.

## Security, fairness, and operations

- Scan the complete Git history for credentials, production endpoints, personal data, and payment records.
- Keep game state, fish hits, rewards, balances, and settlement authoritative on reviewed server code.
- Review randomness, probabilities, administrator controls, bots, anti-cheat, and audit logs independently.
- Add authentication, least privilege, rate limits, encryption, monitoring, alerts, backups, restore tests, and rollback procedures.

## Legal and platform review

- Obtain target-market advice for game classification, competitions, prizes, payments, virtual items, probability disclosure, age limits, privacy, taxation, and consumer protection.
- Review Apple, Google, payment-provider, advertising, and regional distribution policies.

This checklist is not legal, security, fairness, or production certification.

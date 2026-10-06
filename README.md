<img src="github_cover.webp" width="100%">

## Ashutosh Sao

Backend and infrastructure engineer. I build real-time systems and runtimes for AI agents, and run them myself on Kubernetes (GKE).

Engineering Resident at **Super30 (100xSchool)** · contract engineer on a live, paid product · 16 merged PRs at **Palisadoes Foundation** (Talawa) · Superteam SuperDevs finalist

### Projects

Both are live in production, self-hosted on GKE.

- **[Orin](https://orin.ashutoshsao.com)**: AI app builder. Describe an app and an agent writes and runs it in a cloud sandbox, with a live preview over SSE.
  - Provider-agnostic agent loop (OpenAI-compatible and Claude Messages API)
  - Crash-safe builds: every agent round is git-snapshotted to R2, so a dropped connection or dead sandbox resumes or rewinds to any earlier step (181 restorable checkpoints across 19 user-built apps)
  - Invite, guest-link and bring-your-own-key tiers with atomically enforced step budgets
  - [source](https://github.com/ashutoshsao/orin)
- **[Nebula](https://nebula.ashutoshsao.com/trade/BTC-PERP)**: perpetual-futures exchange.
  - Single-writer in-memory matching engine fed typed Redis Stream commands, with margin, liquidation and funding-rate settlement
  - **200k+ orders/sec, p99 under 40µs** over 1M orders (in-process benchmark)
  - Found and fixed a bug that left filled orders in the book: **30× throughput** (11k → 320k orders/sec), with regression tests
  - Deterministic snapshot/replay recovery via R2; live order book over WebSockets; 6 services on GKE
  - [source](https://github.com/ashutoshsao/nebula)

**Stack:** TypeScript, Bun, Rust, Python · PostgreSQL, TimescaleDB, Redis · Docker, Kubernetes, Cloudflare R2

[ashutoshsao.com](https://ashutoshsao.com) · [ashutoshsao17@gmail.com](mailto:ashutoshsao17@gmail.com) · [x.com/ashutosh_sao](https://x.com/ashutosh_sao)

<!---
ashutoshsao/ashutoshsao is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

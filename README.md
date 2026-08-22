# Raji Muhammed Robiu

Computational linguist turned LLM systems & infrastructure engineer — I build free-tier-first, failure-aware routing and agent systems that stay reliable when individual providers don't.

**B.A. Linguistics** (syntax, HCI, Computational Linguistics; AI thesis) · **Fortinet NSE 1–3** · **Cisco CyberOps**

## Infrastructure I run

Ansible-provisioned VPS (30-min full stack on any cloud): Nginx reverse proxy, PostgreSQL, MariaDB, Redis, Docker containers, Prometheus/Grafana monitoring, fail2ban, WireGuard VPN, automated backups. Self-hosted: Vaultwarden, Firefly III, Searx, Focalboard, Monica CRM.

## LLM Systems

- [flippy](https://github.com/Rawbeew/flippy) — Multi-provider LLM failover router + Loomweaver agent harness. Semantic cache (TF-IDF cosine), quota-aware routing with exponential cooldown, multi-key rotation, hedged requests. Stdlib-only core. 147 tests including failure injection.
- [dont-get-rekt](https://github.com/Rawbeew/dont-get-rekt) — Crypto signal engine: multi-chain ingestion (Dexscreener/ccxt, 90+ chains) → SQLite → LLM judge → paper trades. 30-day pre-registered evaluation running.
- [verysketchy.lol](https://verysketchy.lol) — Memecoin exposure auction on Cloudflare Workers. On-chain payment verification across Solana/Ethereum/Base/Monad.
- [just-hired](https://github.com/Rawbeew/just-hired) — Job ingestion pipeline: Cloudflare Worker cron → content-hash dedup → last-12h board + ATS resume builder.

## Full Stack

| Layer | Technologies |
|---|---|
| **Languages** | Python, Bash/Shell, SQL, JavaScript |
| **Infrastructure** | Ansible, Docker, Vagrant, Nginx, WireGuard |
| **Databases** | PostgreSQL, MariaDB, Redis, SQLite |
| **Monitoring** | Prometheus, Grafana, Alertmanager |
| **LLM Providers** | OpenRouter, Groq, NVIDIA NIM, Cloudflare Workers AI, freeinference.org |
| **Deployment** | Cloudflare Workers, Netlify, Docker Compose, GH Actions CI |
| **Security** | fail2ban, WireGuard, Blocky DNS, SSRF guards, path jails, key rotation |

## How I work differently

Most people treat LLMs as black-box APIs. Most infra people don't understand language models. Most NLP people don't provision servers. I sit at the intersection.

- Router core has **zero pip dependencies** — if it needs a framework to work, I redesign
- Evaluation protocols commit success criteria **before results are known**
- Agent tool restrictions enforced at dispatch, not suggested in prompts
- Post-mortems written for real bugs found ([POSTMORTEMS.md](https://github.com/Rawbeew/flippy/blob/master/POSTMORTEMS.md))
- $0 infrastructure cost by design

## Looking for

AI Engineer / LLM Infrastructure / MLOps / Backend Engineer with AI focus (remote). Teams building their LLM stack that also need someone who can provision the servers it runs on.

---

[LLM.txt](https://raw.githubusercontent.com/Rawbeew/portfolio/master/LLM.txt)

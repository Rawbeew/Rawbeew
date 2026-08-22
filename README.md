# Raji Muhammed Robiu

Computational linguist turned LLM systems engineer — I build free-tier-first, failure-aware routing and agent systems in pure Python.

**B.A. Linguistics** (syntax, HCI, Computational Linguistics; AI thesis) · **Fortinet NSE 1–3** · **Cisco CyberOps**

## LLM Systems

- [flippy](https://github.com/Rawbeew/flippy) — Multi-provider LLM failover router + agent harness. Semantic cache (TF-IDF cosine), quota-aware routing with exponential cooldown, multi-key rotation, failure-injection tests. Stdlib-only core. 147 tests.
- [dont-get-rekt](https://github.com/Rawbeew/dont-get-rekt) — Crypto signal engine: multi-chain ingestion (Dexscreener/ccxt) → SQLite → LLM judge → paper trades. 30-day pre-registered evaluation running.
- [verysketchy.lol](https://verysketchy.lol) — Memecoin exposure auction on Cloudflare Workers. On-chain payment verification across Solana/Ethereum/Base/Monad.
- [just-hired](https://github.com/Rawbeew/just-hired) — Job ingestion: Cloudflare Worker cron → content-hash dedup → last-12h board + ATS resume builder.

## Stack

| Layer | Technologies |
|---|---|
| Languages | Python, SQL, Bash, JavaScript |
| Deployment | Docker, Cloudflare Workers, Netlify, GitHub Actions CI |
| Data | SQLite (schema design, indexed queries, FK constraints) |
| Security | SSRF guards, path jails, env stripping, key redaction, input validation |

## How I work differently

Most people treat LLMs as black-box APIs. Most NLP people don't ship working code. I sit in the middle.

- Router core has **zero pip dependencies** — if it needs a framework to work, I redesign
- Evaluation protocols commit success criteria **before results are known**
- Agent tool restrictions enforced at dispatch, not suggested in prompts
- Post-mortems written for real bugs found ([POSTMORTEMS.md](https://github.com/Rawbeew/flippy/blob/master/POSTMORTEMS.md))

## Looking for

AI Engineer / LLM Application Engineer roles (remote). Teams building their LLM stack who need reliable routing, honest evaluation, and clean Python.

---

[LLM.txt](https://raw.githubusercontent.com/Rawbeew/portfolio/master/LLM.txt)

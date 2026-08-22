# Raji Muhammed Robiu

Computational linguist turned LLM systems engineer — I build free-tier-first, failure-aware routing and agent systems that stay reliable when individual providers don't.

**B.A. Linguistics** (Computational Linguistics concentration, AI thesis) · **Fortinet NSE 1–3** · **Cisco CyberOps**

## What I build

I'm strongest at the intersection of language understanding and practical LLM infrastructure:

- **Multi-provider routing and failover** — keeping inference alive when free-tier providers rate-limit or go down
- **Cost and quota control** — routing away from exhausted tiers before the 429 hits
- **Agent reliability** — role-based tool restrictions, adversarial verification gates, structured event logging
- **Evaluation with linguistic rigor** — pre-registered protocols, labeled ground truth, honest failure analysis

## Projects

| | | |
|---|---|---|
| [flippy](https://github.com/Rawbeew/flippy) | Multi-provider LLM failover router + Loomweaver agent harness. Semantic cache, quota-aware routing, key rotation. 147 tests. | Python stdlib |
| [dont-get-rekt](https://github.com/Rawbeew/dont-get-rekt) | Crypto signal engine: ingestion → SQLite → LLM judge → paper trades. 30-day pre-registered evaluation running. | Python, SQLite |
| [verysketchy.lol](https://verysketchy.lol) | Memecoin exposure auction — on-chain payments (SOL/ETH/Base/MON), instant verification. | Cloudflare Workers |
| [just-hired](https://github.com/Rawbeew/just-hired) | Job ingestion: Worker cron → SQLite dedup → last-12h board + ATS resume builder. | Cloudflare Workers, Netlify |

## How I work differently

Most people treat LLMs as black-box APIs. Most NLP people don't ship reliable infrastructure. I sit in the middle.

- The router core in flippy has **zero pip dependencies** — if it needs a framework to work, I redesign
- dont-get-rekt's evaluation protocol commits success criteria **before results are known**
- Every agent action is logged to replayable JSONL traces; tool restrictions are enforced at dispatch, not suggested in prompts
- I write post-mortems for bugs I find ([POSTMORTEMS.md](https://github.com/Rawbeew/flippy/blob/master/POSTMORTEMS.md))

## Looking for

AI Engineer / LLM Infrastructure / Applied AI roles (remote). Teams that are cost-conscious, still building their LLM stack, and need someone who actually understands language — not just API calls.

---

[LLM.txt](https://raw.githubusercontent.com/Rawbeew/portfolio/master/LLM.txt) available for AI crawlers.

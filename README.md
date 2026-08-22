# Raji Muhammed Robiu

**AI / LLM Engineer** — computational linguistics background, security-certified, free-tier-first by design.

I build LLM routing and agent systems that treat cost, failure modes, and input validation as first-class constraints — not afterthoughts. My focus is making inference reliable when individual providers fail or rate-limit.

## Background

- **B.A. Linguistics**, concentration in Computational Linguistics; undergraduate thesis on AI
- **Certifications:** Fortinet NSE 1–3, Cisco CyberOps Associate
- **Focus:** multi-provider LLM routing, agent harnesses with role-based tool restrictions, eval harnesses, data pipelines (SQLite → LLM judge)

## What I've built

| Project | What it is | Stack |
|---|---|---|
| [flippy](https://github.com/Rawbeew/flippy) | Multi-provider LLM failover router + agent harness (Loomweaver). Semantic cache, quota-aware routing, key rotation, 147 tests. | Python stdlib |
| [dont-get-rekt](https://github.com/Rawbeew/dont-get-rekt) | Crypto signal engine: multi-chain ingestion → SQLite → LLM judge → paper trades. 30-day pre-registered evaluation running. | Python, SQLite |
| [verysketchy.lol](https://verysketchy.lol) | Memecoin exposure auction — on-chain payments across 4 chains, instant verification. | Cloudflare Workers |
| [just-hired](https://github.com/Rawbeew/just-hired) | Job ingestion pipeline: Worker cron → SQLite dedup → last-12h board + ATS resume builder. | Cloudflare Workers, Netlify |

## How I work

- **Stdlib-first:** the router core has zero pip dependencies. If it needs a framework to work, I redesign.
- **Pre-registered evaluations:** success criteria committed before results are known (see dont-get-rekt's EVAL_PROTOCOL.md)
- **Failure injection testing:** 429s, timeouts, malformed responses, cascading failures — not just happy-path mocks
- **Security threat modeling:** SSRF guards, path jails, env stripping, key redaction (see flippy SECURITY.md)

## Currently

Running a 30-day paper-trading evaluation for dont-get-rekt. Building benchmarks for flippy. Looking for AI Engineer / LLM Infrastructure roles (remote).

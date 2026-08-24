# promptcracka

computational linguist turned llm systems engineer — i build free-tier-first, failure-aware routing and agent systems that stay reliable when individual providers don't.

**B.A. Linguistics** (syntax, hci, computational linguistics; AI thesis) · **Fortinet NSE 1–3** · **Cisco CyberOps**

## what i build

- [flippy](https://github.com/Rawbeew/flippy) — multi-provider llm failover router + agent harness. semantic cache, quota-aware routing, key rotation. stdlib-only core. 147 tests.
- [dont-get-rekt](https://github.com/Rawbeew/dont-get-rekt) — crypto signal engine: multi-chain ingestion → sqlite → llm judge → paper trades. 30-day pre-registered evaluation running.
- [verysketchy.lol](https://verysketchy.lol) — memecoin exposure auction on cloudflare workers. on-chain payments across solana/eth/base/monad.
- [just-hired](https://github.com/Rawbeew/just-hired) — job ingestion: worker cron → sqlite dedup → last-12h board + ats resume builder.

## stack

| layer | technologies |
|---|---|
| languages | python, sql, bash, javascript |
| deployment | docker, cloudflare workers, netlify, github actions ci |
| data | sqlite (schema design, indexed queries, FK constraints) |
| security | ssrf guards, path jails, env stripping, key redaction |

## how i work differently

- router core has **zero pip dependencies** — if it needs a framework to work, i redesign
- evaluation protocols commit success criteria **before results are known**
- post-mortems written for real bugs found ([POSTMORTEMS.md](https://github.com/Rawbeew/flippy/blob/master/POSTMORTEMS.md))

## find me

- x/twitter: [@promptcracka](https://x.com/promptcracka)
- youtube/tiktok/ig: [@promptkracka](https://youtube.com/@promptkracka)
- github: [Rawbeew](https://github.com/Rawbeew)

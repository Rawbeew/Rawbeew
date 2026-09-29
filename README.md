# Rabiu Raji

Computational linguist building small language models for tasks where large ones are overkill. Currently shipping open-source mT5 fine-tunes for cross-lingual authorship attribution, paper-mode evaluation pipelines, and a Hugging Face presence under the Chaiir organisation.

**B.A. Linguistics** (syntax, HCI, computational linguistics; AI thesis) · **MA Linguistics** (Trinity Western University, in progress) · **Fortinet NSE 1–3** · **Cisco CyberOps**

## research (current focus)

- **stylometric-slm** — open-source mT5 fine-tunes for cross-lingual authorship attribution. Two models on Hugging Face (`Chaiir/stylometric-cls-v1`, `Chaiir/stylometric-mt5-v1`), 91.2% evaluation accuracy on the full 705-passage held-out split (14 authors × 4 languages).
- **Voice or Mask?** — preprint on Zenodo (DOI 10.5281/zenodo.22725022). Documents the engineering choices behind a small classifier and the snags I hit along the way, including the mT5 TiedWeight pickle-save bug and a front-matter leakage that pushed grad_norm to 4369.
- **HuggingFace:** [Chaiir](https://huggingface.co/Chaiir) — open model + tokenizer + training script.

## what I'm shipping now (Sept 2026)

- **Jobint** — sister-targeted job-search helper: paste a posting, get a tailored cover letter + resume tweaks + fit score. Multi-provider LLM failover. Now also ships as a static frontend on GitHub Pages.
- **campus-access** — privacy-preserving entry/exit counter for campus buildings, queryable in English.
- **flippy** — multi-provider LLM failover router + agent harness. Semantic cache, quota-aware routing, key rotation. Stdlib-only core. 147 tests.
- **dont-get-rekt** — crypto signal engine: multi-chain ingestion → sqlite → LLM judge → paper trades. 30-day pre-registered evaluation running.
- **just-hired** — fresh-only direct-employer job board. Cloudflare Worker fetches Job Bank + UHN every 2h, last-12h only. Static site + ATS resume/cover-letter generator.
- **technocore-chat** — HTTP-native chat and notes for agents whose sandbox only allows webfetch. Every write is a plain GET.

## stack

| layer | technologies |
|---|---|
| languages | python, sql, bash, javascript |
| deployment | docker, cloudflare workers, github actions ci, github pages |
| data | sqlite (schema design, indexed queries, FK constraints) |
| security | ssrf guards, path jails, env stripping, key redaction |
| NLP | mT5, HuggingFace transformers, sentence-transformers, stylometry |

## how I work

- Router core has **zero pip dependencies** — if it needs a framework to work, I redesign.
- Evaluation protocols commit success criteria **before results are known**.
- Post-mortems written for real bugs found (`POSTMORTEMS.md` in flippy).
- Models ship with full training journals, not just accuracy numbers — every published artifact has a paper/, scripts/, and a reproducible Colab walkthrough.

## find me

- github: [Rawbeew](https://github.com/Rawbeew)
- huggingface: [Chaiir](https://huggingface.co/Chaiir)
- email: raji.rawbeew@gmail.com

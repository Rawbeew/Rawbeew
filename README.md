# Rabiu Raji

Computational linguist building small language models for tasks where large ones are overkill. Shipping open-source mT5 fine-tunes for cross-lingual authorship attribution, adversarial-evaluation research infrastructure, and free-tier-first LLM orchestration. Hugging Face presence under the Chaiir organisation.

**B.A. Linguistics** (syntax, HCI, computational linguistics; AI thesis) · **Fortinet NSE 1–3** · **Cisco CyberOps** · ORCID 0009-0007-8968-8620

## research

- **stylometric-slm** — open-source mT5 fine-tunes for cross-lingual authorship attribution. Two models on Hugging Face (`Chaiir/stylometric-cls-v1`, `Chaiir/stylometric-mt5-v1`), 91.2% evaluation accuracy on the full 705-passage held-out split (14 authors × 4 languages). Apache-2.0, with training journal, corpus rebuild path, and reproducible Colab.
- **Voice or Mask?** — preprint on Zenodo ([DOI 10.5281/zenodo.22725022](https://doi.org/10.5281/zenodo.22725022)). Stylometric forensic analysis distinguishing human poetry from LLM imitation. Documents the engineering snags: the mT5 TiedWeight pickle-save bug and a front-matter leakage that pushed grad_norm to 4369.
- **Beyond the Mask** (in preparation) — adversarial authorship attribution: a multi-agent pipeline generates author-conditioned LLM mimicry at scale, then a fine-tuned classifier measures which stylometric features survive imitation by every model. Closed-loop: mapped human baselines → constrained generation → hijack/detection/repair evaluation.
- **HuggingFace:** [Chaiir](https://huggingface.co/Chaiir) — open model + tokenizer + training script.

## what I'm shipping now (Oct 2026)

- **flippy** — multi-provider LLM failover router + agent harness. Adaptive provider ordering (EWMA success/latency scoring), in-provider retry with backoff, quota ledger, multi-key rotation, TF-IDF semantic cache, hedged requests, OpenAI-compatible HTTP server, 9 security-guarded agent tools, multi-agent armada fleets, 5 eval suites including a multi-step agent benchmark. Stdlib-only core. 173 tests.
- **stylometric-slm** — see research above; the flagship artifact.
- **dont-get-rekt** — crypto signal engine: multi-chain ingestion → sqlite → LLM judge → paper trades. 30-day pre-registered evaluation running.
- **just-hired** — fresh-only direct-employer job board. Cloudflare Worker fetches Job Bank + UHN every 2h, last-12h only. Static site + ATS resume/cover-letter generator.
- **ican-prep** — ICAN exam prep platform: 2,506 past exam questions across 25 diets (2018–2026) and 3 levels, parsed from official PDFs with a custom multi-era extractor. Works offline (service worker). Live on Cloudflare Pages.
- **Jobint** — job-search helper: paste a posting, get a tailored cover letter + resume tweaks + fit score. Multi-provider LLM failover.
- **campus-access** — privacy-preserving entry/exit counter for campus buildings, queryable in English.

## stack

| layer | technologies |
|---|---|
| languages | python, sql, bash, javascript |
| deployment | docker, cloudflare workers + pages, github actions ci |
| data | sqlite (schema design, indexed queries, FK constraints) |
| security | ssrf guards, path jails, env stripping, key redaction |
| NLP/ML | mT5, HuggingFace transformers, stylometry, TF-IDF retrieval, eval harnesses |

## how I work

- Router core has **zero pip dependencies** — if it needs a framework to work, I redesign.
- Evaluation protocols commit success criteria **before results are known**.
- Post-mortems written for real bugs found (`POSTMORTEMS.md` in flippy).
- Models ship with full training journals, not just accuracy numbers — every published artifact has a paper/, scripts/, and a reproducible path.
- Every claim on a public artifact gets verified against the source API before publishing (ask me about the time my own model card pointed at the wrong Zenodo DOI — I caught it with a one-line curl).

## find me

- github: [Rawbeew](https://github.com/Rawbeew)
- huggingface: [Chaiir](https://huggingface.co/Chaiir)
- email: raji.rawbeew@gmail.com

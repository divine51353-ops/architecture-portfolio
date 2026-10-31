# Architecture Portfolio — Divine Supreme

**Divine Supreme — Founder, SupremeOS | AI Workflow Architect | AI Implementation & Knowledge Systems | Agent Skills, MCP & AI-Assisted Product Development**

I design AI workflows that people can check: where every fact came from, who approved what, what's out of date, and how the next person picks the work up. This repository is the public, readable layer of that work. Product source lives in a private repository; what's here is architecture, design documents and links to public demonstrations, each labelled with how mature it actually is.

## Customer problems I work on

| Problem | What goes wrong today | What the architecture does about it |
| --- | --- | --- |
| AI drafts that sound like everyone else | Generic phrasing, invented details, no record of what the person actually said | Voice profiles built from the person's own writing, with quoted evidence, calibration and a facts check before anything ships |
| Small organizations losing their memory | Decisions, claims and deadlines live in one volunteer's head or inbox | A governed record: sourced facts, named approvals, stale-work detection, a handoff the next person can read |
| Overclaiming to funders and buyers | Numbers drift from their source; "approved" is said before anyone approved | Claim status tied to sources, holds on unsupported numbers, approvals bound to the exact version reviewed |
| Work that dies between AI sessions | Each chat starts from zero; summaries can't be checked | Checksummed (optionally signed) handoffs that software can verify before resuming |

More in [docs/09_customer_problems.md](docs/09_customer_problems.md).

## Maturity, stated plainly

| Label | Meaning |
| --- | --- |
| **Architecture** | Design documents and diagrams; nothing runs |
| **Workflow design** | Prompts, schemas and routing for an agent workflow; not run here as a system |
| **Prototype** | Code that runs, with little or no automated testing |
| **Tested release candidate** | Automated tests and a clean-install rehearsal pass; no customer has used it yet |
| **Observed customer result** | Real people used it, with consent and records. *None yet* |

| Work | Where | Label | Evidence checked on 2026-10-31 |
| --- | --- | --- | --- |
| Supreme Core engine, MCP server, Nonprofit Desk app | Private repository | Tested release candidate (local-first) | 60 engine/skill/release tests and 7 app tests pass; production build passes; clean install from the release archive passes. No hosted accounts, billing or encryption |
| Voice DNA Early Access (first product) | Private repository; summary in [docs/13_voice_dna.md](docs/13_voice_dna.md) | Tested release candidate | Deterministic tests in two languages and a packaged clean-install rehearsal pass. Host test in Claude Code not yet run; no customer sessions |
| [companion-core-python](https://github.com/divine51353-ops/companion-core-python) | Public | Prototype | Installs; demo runs; 2 tests pass; several modules are placeholders |
| [universal-shell-html](https://github.com/divine51353-ops/universal-shell-html) | Public | Prototype | Single-file, config-driven HTML shell; demo mode only verified by reading; live (BYOK) mode not verified |
| [book-forge-workflow](https://github.com/divine51353-ops/book-forge-workflow) | Public | Workflow design | Six agent prompts and seven JSON schemas (all valid JSON); no runnable code |
| [nonprofit-formation-assistant](https://github.com/divine51353-ops/nonprofit-formation-assistant) | Public | Workflow design | Six prompts and five JSON schemas (all valid JSON); not legal or tax advice |
| This repository's docs 01–08 | Public | Architecture | Concept and product-family documents |

Details and the checks behind each label: [docs/12_evidence_and_maturity.md](docs/12_evidence_and_maturity.md).

## How the work is built

- **Product and workflow architecture** — one engine, many products: each product is a configuration (stages, records, rules) on shared machinery. [docs/01](docs/01_system_overview.md), [docs/04](docs/04_agent_workflow_blueprint.md)
- **AI-assisted implementation** — built with Claude Code and Claude Skills, with tests written for every repaired failure and claims kept to what tests show. [docs/10_ai_assisted_implementation.md](docs/10_ai_assisted_implementation.md)
- **Review, recovery and operator handoff** — approvals, holds, stale-work detection, backups and verified handoffs. [docs/11_review_recovery_handoff.md](docs/11_review_recovery_handoff.md)
- **Agent Skills and MCP** — the same rules exposed as installable Claude Skills and as an MCP server for MCP clients.

## Runnable demonstrations

| Demo | How to run | What you'll see |
| --- | --- | --- |
| Companion Core foresight demo | `pip install .` then `python examples/run_foresight_demo.py` in companion-core-python (Python 3.11+) | A 20-entry kernel map, a contradiction scan and a path gate verdict |
| Universal shell | Open `shells/index.html` from universal-shell-html in a browser | The config-driven shell in demo mode |
| Voice DNA walkthrough | On request: a three-minute screen demo using a fictional consultant's synthetic samples | Permission, sufficiency, quoted profile, calibration, a checked draft, export and resume |

## Source organization and evidence boundaries

- Public repositories hold architecture, schemas, prompts and prototypes. Product source, customer material and private operating rules stay private.
- No README sentence counts as proof here. Labels above come from running or reading the code on the date shown.
- No client names, revenue figures, testimonials or production-scale claims appear because none have been recorded.

## Reading order

1. [docs/09_customer_problems.md](docs/09_customer_problems.md)
2. [docs/12_evidence_and_maturity.md](docs/12_evidence_and_maturity.md)
3. [docs/13_voice_dna.md](docs/13_voice_dna.md)
4. [docs/10_ai_assisted_implementation.md](docs/10_ai_assisted_implementation.md)
5. [docs/11_review_recovery_handoff.md](docs/11_review_recovery_handoff.md)
6. Architecture background: [docs/01](docs/01_system_overview.md) through [docs/08](docs/08_product_ecosystem.md)

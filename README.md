# zq-dev (zqpmo)

> 围绕**实际工作流程**做**可控、可审计**的自动化工具：规则优先、状态机门禁、默认 dry-run、人工复核边界写清楚。

**Focus:** workflow automation you can audit — rule-first engines, explicit state gates, dry-run defaults, and honest maturity labels.

## Featured projects

| Project | What it is | Maturity | Boundary |
|---|---|---|---|
| [agentic-task-dispatcher](https://github.com/zqpmo/agentic-task-dispatcher) | Deterministic multi-board task controller: contract checks, reconciliation, dry-run default | **Architecture prototype** | Not a production scheduler; lock/CAS/executor-ack are documented limitations, not guaranteed |
| [file-flow](https://github.com/zqpmo/file-flow) | Rule-first file inbound engine: scan → classify → move → journal, optional LLM pending drain | **Usable offline tool** (stdlib Python) | Local file moves only; `--ai` sends filenames/paths to *your* LLM endpoint; default is dry-run (`--execute` to move) |
| [policy-review-workbench](https://github.com/zqpmo/policy-review-workbench) | Offline policy-review flow: parse → compare → QC → export with CASE acceptance tests | **Offline prototype / flow demo** | Mock parse (does **not** read file bodies); exports are text/CSV/JSON drafts — not final legal conclusions |

## Principles

1. **Dry-run first** — previews before destructive moves or production writes.
2. **Human in the loop** — semantic judgments stay out of the control path.
3. **Honest README** — if it is a prototype, the README says so.
4. **Sanitized public surface** — no secrets, no real business paths in current trees; history may still show earlier sample names where noted.

## Contact

Open an issue on the relevant repo.
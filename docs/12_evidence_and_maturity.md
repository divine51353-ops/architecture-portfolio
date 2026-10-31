# Evidence and maturity, repository by repository

Checked on 2026-10-31 by cloning each repository and running or reading it. Where a README claims more than the code shows, the code wins.

## Public

### companion-core-python — Prototype
- `pip install .` succeeds (Python 3.11+ required by `pyproject.toml`; checked with 3.14).
- `examples/run_foresight_demo.py` runs: prints a 20-entry kernel map, a "Bloodline" verdict, a contradiction scan and a path-gate result.
- `tests/test_engine.py`: 2 tests, both pass with pytest.
- The README lists several modules as placeholder-but-runnable; that matches the code. Two TODO/placeholder markers remain in `src`.

### universal-shell-html — Prototype
- `shells/index.html` and a ~40 KB single-file shell with config-driven product identity and rooms.
- Live mode calls the Anthropic Messages API directly from the browser with a user-supplied key. It does not send the header the API requires for direct browser access, so live mode is expected to fail until that's added; it was not run here.
- Example configs for three verticals are valid JSON.

### book-forge-workflow — Workflow design
- Six agent prompts, seven JSON output schemas (all valid JSON), node layout and state-variable docs, sample request and outputs.
- No runnable code; deployment notes describe an agent-builder setup that was not run here.

### nonprofit-formation-assistant — Workflow design
- Six agent prompts, five JSON schemas (all valid JSON), a workflow diagram and delivery modes.
- Not legal, tax or filing advice (stated in the repository and repeated here).

### architecture-portfolio (this repository) — Architecture
- Docs 01–08 are concept and product-family documents. Terms such as "deployable" or "production" in them describe design intent, not deployed systems.

## Private (summarized, source not public)

### Supreme Core 1.2.0 + MCP server + Nonprofit Desk 0.2.0 — Tested release candidate
- 61 automated tests (engine, trust regressions, MCP server, skills, product library, release packaging, Voice DNA) and 7 web-app tests pass; production build passes.
- Tested on Node 20.14, 20.20, 22, 24 and 25; skill scripts on Python 3.9.6 and 3.14.1.
- A release archive installs cleanly into an empty folder and passes its tests there.
- Local-first: no user accounts, tenant authorization, encryption at rest, billing or remote MCP.

### Voice DNA Early Access 1.1.0 — Tested release candidate
- See [13_voice_dna.md](13_voice_dna.md).

## Observed customer results
None recorded yet.

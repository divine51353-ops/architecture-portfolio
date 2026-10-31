# AI-assisted implementation

How the products are built, and how claims about them are kept honest.

## Tools
- **Claude Code** for implementation, refactoring and test writing in the repository.
- **Claude Skills** as a delivery format: instructions plus small scripts that enforce rules in code.
- **MCP (Model Context Protocol)** to expose the same engine as tools to MCP clients.
- **Node.js** for the engine, MCP server and web app; **Python** (standard library only) for scripts inside skills.

## Working rules
1. **A failure becomes a test first.** In the October 2026 release, each audited defect (holds that didn't block approval, stale work that stayed "accepted", unchecked source text, approvals not bound to a version, unvalidated handoffs) was reproduced as a regression test before the fix.
2. **Two implementations, one answer.** Where a rule exists in JavaScript (engine) and Python (skill script), tests require both to give the same result.
3. **Status is earned, not typed.** A product's status in the internal library is computed from recorded evidence (tests, evaluations, consented sessions, payments, owner sign-off). Operator-entered records are labelled as such; they are not independent certification.
4. **Runtimes are tested, not assumed.** Supported versions are the ones actually run (for example, a Node floor was corrected after a test showed an API missing on the advertised minimum).
5. **Packages are rehearsed.** Releases are built from tracked files only, scanned for secrets, given a SHA-256 manifest, and installed from the archive into an empty folder before they are called installable.
6. **Model output is judged, not trusted.** Model evaluations keep prompts, model and outputs; where an evaluation couldn't run, it's recorded as not run.

## What AI assistance is not used for
- Inventing customer results, testimonials, credentials or metrics.
- Approving work on a person's behalf.
- Declaring something production-ready without the tests and records to show it.

# Customer problems addressed

Each problem below is described from the buyer's side. "Status" says how far the work has actually gone.

## 1. "AI writing doesn't sound like me"
**Who:** consultants, founders and creators who write with AI.
**What happens now:** drafts drift into generic phrasing, add details the person never gave, and there's no shared definition of their voice to hand a writer or tool.
**Approach:** build a voice profile only from writing the person owns or has permission to use; quote evidence for every trait; check two short calibration passages with them; write from confirmed facts; lint for generic phrasing and flag unconfirmed numbers, dates, names and claim words; require the person's review; export a reusable voice guide and a verifiable handoff.
**Status:** Voice DNA Early Access 1.1.0 — tested release candidate, no customer sessions yet. See [13_voice_dna.md](13_voice_dna.md).

## 2. "Our organization forgets everything when someone leaves"
**Who:** small nonprofits and community organizations.
**What happens now:** mission language, board decisions, impact numbers and grant deadlines are scattered across inboxes and one volunteer's memory.
**Approach:** one governed record with sources, claim status, named approvals of exact versions, holds on unsupported impact numbers, and a handoff file.
**Status:** Nonprofit Desk — local web app, tested; no pilot run yet.

## 3. "We said more than we can prove"
**Who:** grant writers, founders, anyone writing to funders or buyers.
**What happens now:** a number moves from a report to a proposal and changes on the way; "the board approved" appears before a vote.
**Approach:** claims carry status (verified by a named person with a supporting excerpt, asserted, assumed, unknown, in conflict); a changed source marks everything built on it as out of date.
**Status:** implemented and tested in the private engine; not yet a separate product.

## 4. "Every AI session starts from zero"
**Who:** anyone running long work across several chats or tools.
**What happens now:** a summary is pasted into the next chat, and nobody can tell if it was edited or is still current.
**Approach:** a structured handoff with checksums (and, with a key, signatures) that software checks before resuming; the readable Markdown version says it is a summary, not verified state.
**Status:** implemented and tested in the private engine and in the Voice DNA skill.

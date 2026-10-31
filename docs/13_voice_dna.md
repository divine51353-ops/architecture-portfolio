# Voice DNA Early Access — first SupremeOS product

*Sound like yourself at full strength.*

**Buyer:** a consultant, founder or creator with writing they own or have permission to use.
**First result:** a reviewed voice profile, two short calibration passages, and one useful draft, delivered with a reusable handoff.
**Delivery:** an installable Claude Skill package, with optional assisted setup.

## The journey
1. Explain prerequisites; confirm permission to use the samples.
2. Collect and identify samples (numbered, counted, fingerprinted).
3. Measure sufficiency: at least 300 words across at least two distinct samples. Duplicates count once. This is a rule of thumb for having enough material, not a validated accuracy threshold.
4. Label the profile EXTRACTED (enough material, every trait quoted) or DESIGNED (partly chosen).
5. Build a proposed profile; every quote is checked against its sample.
6. Write two short calibration passages.
7. Capture the person's corrections and acceptance; acceptance is tied to the exact profile.
8. Write one draft from facts the person confirmed.
9. Lint for generic phrasing and banned phrases; flag numbers, dates, names and claim words the facts don't contain; the person reviews.
10. Export the profile, a voice guide, the draft, settings and a checksummed handoff.
11. Resume in a new session; every exported file is checked.

## Who decides what
| Deterministic (scripts) | Model judgment | The person |
| --- | --- | --- |
| Word counts, duplicates, sufficiency, schema, quote matching, fingerprints, lint, facts check | Traits, calibration passages, draft wording, reading against drift notes | Permission, calibration verdicts, acceptance, draft approval |

## Evidence so far
- Deterministic tests in JavaScript and Python agree on every rule above, including malformed inputs, duplicate samples, invalid phrase patterns, changes after acceptance, and export/resume in a fresh process.
- The customer package installs from its archive into an empty folder, and the full journey runs on a synthetic example.
- One host test in Claude Code (three scripted turns, synthetic example) passed all 13 automated checks. It also showed the limit those checks share: the draft added a small unconfirmed phrase that only a human review would catch.
- **Not yet:** a test of the Claude.ai or desktop upload path, and any customer session. A two-person pilot packet is ready.

## Price
$49 is a proposed early-access price to test. No billing is built.

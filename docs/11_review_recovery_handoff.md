# Review, recovery and operator handoff

## Review
- **Generated is not accepted.** Every record starts as a draft. A named person approves one exact version; the approval records the version and a content fingerprint.
- **Names are not identities.** In the local-first products, approver names are typed by the operator and labelled that way. They are not logins or electronic signatures.
- **Holds stop the work they cover.** An unsupported impact number or a flagged input opens a hold; held work can't be approved or built on until a person releases it with a resolution. Repairs (fixing sources, redrafting) stay open.

## Staying current
- A changed source marks every claim and record built on it as out of date, down the whole chain, with the reason.
- Updating a source is an explicit action with a reason; earlier versions are kept.

## Recovery
- Project files carry checksums (signatures with a key) and a hash-chained event log; edited files are refused with the reason.
- Two sessions saving the same project can't silently overwrite each other.
- Backups are plain folders; operations notes cover data locations, key custody, backup and restore.

## Handoff
- **For software:** a JSON handoff checked for structure, checksum, signature (when keyed), product version and ledger before resuming. Incompatible product versions are refused unless explicitly declared compatible.
- **For people:** a Markdown summary that says it is a summary and can't be restored.
- **For writers and other AI tools:** in Voice DNA, a plain-text voice guide that works anywhere.

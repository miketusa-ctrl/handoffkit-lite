# Handoff Record Schema

`handoff.schema.json` (JSON Schema 2020-12) defines one handoff record.

## Required fields
- `handoff_id` — `HO-YYYYMMDD-short-slug`
- `from_agent` and exactly one of `to_agent` / `to_human`
- `timestamp` — ISO 8601 with offset
- `goal`, `context_summary`, `next_action` — plain sentences; next action starts with a verb
- `owner` — who is accountable for the next action
- `priority` — low / normal / high / urgent
- `quiet_hours_respect` — true if the receiver should wait for working hours
- `approval_needed` — true when the next step touches money, legal, deletion or external messages

## Optional fields
`artifacts[]` (name, location, note), `blockers[]` (description, owner, since), `approval_category`, `cost_so_far` (amount, currency), `decisions_ref`, `lessons_ref`.

## Rules of thumb
- Summaries say what changed, not the whole history; link to decisions.md for why.
- Every blocker has an owner. A blocker with no owner is just a complaint.
- Never paste keys, tokens or personal data into a record; reference where they live instead.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

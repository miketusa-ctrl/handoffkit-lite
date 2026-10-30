# Template: Agent-to-Human Handoff

Use when an agent needs a person to read, decide or approve.

## Message shape (keep under 120 words)
1. **Ask** — one line: what you need from them (approve / decide / unblock).
2. **Why now** — deadline or cost of waiting.
3. **Options** — A / B (recommended marked).
4. **What happens next** — what the agent does after each answer.
5. **Record** — link to the handoff record and blocked-on-human.md entry.

## Fields
Same as the schema, with `to_human` set and, if relevant, `approval_needed: true` plus `approval_category`.

## Do not
- Bundle unrelated asks across days; batch per run instead.
- Message during the person's quiet hours unless priority is urgent and the matrix allows it.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

# Lite: Start Here

## What is inside
- `schema/handoff.schema.json` — the record format
- 3 templates — agent-to-agent, agent-to-human, escalation
- `state/` — handoff.md, decisions.md, lessons.md, blocked-on-human.md, run-log.md
- 2 fictional examples (support → billing, research → writer)

## Ten-minute setup
1. Copy `state/` into your repo.
2. Add one line to your agent instructions: "At the end of every run, update state files and write a handoff record."
3. Validate records with any JSON Schema 2020-12 validator.

Pro adds orchestration patterns, an approval matrix, instruction snippets and a linter.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

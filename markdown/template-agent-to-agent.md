# Template: Agent-to-Agent Handoff

Use when one agent passes work to another agent.

```
handoff_id: HO-YYYYMMDD-slug
from_agent:
to_agent:
timestamp:
goal: <one sentence: what done looks like>
context_summary: <what was done this run, what changed, 3–6 lines>
artifacts:
  - name:      location:
next_action: <verb-first, one step the receiver does first>
blockers:
  - description:      owner:
owner: <who owns the next action>
priority: normal
quiet_hours_respect: true
approval_needed: false
cost_so_far: {amount: 0, currency: USD}
decisions_ref: decisions.md#
lessons_ref: lessons.md#
```

## Sender checklist
- [ ] State files updated (handoff.md, decisions.md, run-log.md)
- [ ] Next action is a single concrete step
- [ ] Blockers each have an owner
- [ ] No secrets in the record

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

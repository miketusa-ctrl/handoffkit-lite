# Template: Escalation

Use when a blocker passes its wait time or a risk appears.

```
ESCALATION  HO-YYYYMMDD-slug
Severity: S1 | S2 | S3
Trigger: <what happened>
Tried: <what the agent already did>
Impact if ignored: <cost / deadline>
Needs: <decision or approval>  from: <role>
Hold during quiet hours: yes|no
Re-escalate to: <role> if no answer by <time>
```

## Before escalating
- Run the linter (Pro) or check state files by hand.
- Confirm the blocker is in blocked-on-human.md with an owner.
- One bundled escalation per run, not one message per issue.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

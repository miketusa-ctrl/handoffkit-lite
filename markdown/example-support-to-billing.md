# Example: Support Agent to Billing Agent

All names and values are fictional.

```json
{
  "handoff_id": "HO-20261102-refund-check",
  "from_agent": "support-desk-bot",
  "to_agent": "billing-bot",
  "timestamp": "2026-11-02T10:15:00-07:00",
  "goal": "Decide whether order #A-1043 at Pinecone Candle Co. qualifies for a partial refund.",
  "context_summary": "Customer 'Customer 1' reports a cracked jar on arrival with a photo. Policy allows refunds within 30 days; order is 9 days old.",
  "artifacts": [
    {
      "name": "ticket",
      "location": "helpdesk://tickets/5521",
      "note": "fictional"
    }
  ],
  "next_action": "Check order total and draft a refund proposal for human approval.",
  "blockers": [],
  "owner": "billing-bot",
  "priority": "normal",
  "quiet_hours_respect": true,
  "approval_needed": true,
  "approval_category": "money",
  "cost_so_far": {
    "amount": 0.04,
    "currency": "USD"
  },
  "decisions_ref": "decisions.md#2026-11-02",
  "lessons_ref": "lessons.md"
}
```

## Why this record works
- Next action is one verb-first step.
- Every blocker has an owner.
- approval_needed is set when the next step touches money, legal, deletion or external messages.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

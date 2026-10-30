# Example: Research Agent to Writer Agent

All names and values are fictional.

```json
{
  "handoff_id": "HO-20261103-blog-brief",
  "from_agent": "research-bot",
  "to_agent": "writer-bot",
  "timestamp": "2026-11-03T08:00:00Z",
  "goal": "Ship a 900-word draft on composting for the fictional Fernbrook Garden blog.",
  "context_summary": "Collected 5 sources and an outline with 4 sections. Tone guide is in artifacts.",
  "artifacts": [
    {
      "name": "outline",
      "location": "docs/outline-compost.md"
    },
    {
      "name": "sources",
      "location": "docs/sources.md"
    }
  ],
  "next_action": "Write the first draft from the outline and log open questions.",
  "blockers": [],
  "owner": "writer-bot",
  "priority": "low",
  "quiet_hours_respect": true,
  "approval_needed": false,
  "approval_category": "none",
  "cost_so_far": {
    "amount": 0.12,
    "currency": "USD"
  }
}
```

## Why this record works
- Next action is one verb-first step.
- Every blocker has an owner.
- approval_needed is set when the next step touches money, legal, deletion or external messages.

> Harlo: operational templates; no guarantee of agent reliability or safety; keep a human approval gate for money, legal, deletion and external messages.

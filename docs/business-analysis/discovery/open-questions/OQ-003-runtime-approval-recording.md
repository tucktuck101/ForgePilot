# OQ-003: How will runtime approvals be recorded?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-003 |
| Document type | Open Question |
| Status | Answered; design validation pending |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation, Product Owner answer dated 2026-06-25, and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-004](../evidence/EVD-004-user-research-gap.md) |
| Related objects | [Open Questions Index](index.md), [Approval Gate Operating Policy](../approval-gates/operating-policy.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Question

How will runtime approvals be recorded?

## Resolution

- Answer: GitHub issues and pull requests are the primary runtime approval records. Repository documents retain the current approval status and durable links to those records.
- Decision: Use a GitHub-native approval trail rather than creating a dedicated repository Markdown decision record for every runtime approval.
- Decision date: 2026-06-25.
- Decision reference: Product Owner selected option B in the Codex open-question working session dated 2026-06-25.

## Recording Rules

- Use a GitHub issue for runtime gates not inherently tied to a pull request, and the pull request for merge or review-specific approvals.
- The primary record must contain the approver, decision date, approve/revise/reject outcome, approved boundary, decision reference, and resulting permitted or blocked activity.
- The relevant repository gate, decision, delivery, or project-state document must mirror the status and link to the primary GitHub record.
- This runtime model does not replace the existing GATE-001, GATE-002, or GATE-003 repository records.
- Chat acknowledgement alone does not satisfy an approval gate.
- Approved solution design must validate link durability, offline or unavailable-GitHub behaviour, and how stale repository status is detected before the workflow-state design is finalised.

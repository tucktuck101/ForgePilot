# NFR-018: Clear Approval Requests

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-018 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

Approval requests must be explicit, evidence-aware, actionable, and durably recorded.

## Details

Each request must identify what is being approved, why the gate exists, the recommendation, credible alternatives, evidence and evidence gaps, risks and trade-offs, and the consequence of approve, revise, or reject.

Approval records must contain status, approver, approval date, and decision reference. Missing decision metadata means the gate remains pending.

## Acceptance Criteria

- Approval requests present approve, revise, and reject outcomes.
- The next permitted and blocked activities are explicit.
- Approval state is stored in the relevant GATE object.
- No document creation, chat acknowledgement, or inferred intent substitutes for a recorded approval.

## Notes

Product direction, product brief, and prototype scope use GATE-001, GATE-002, and GATE-003 respectively.

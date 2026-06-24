# FR-020: Request prototype scope approval

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-020 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

ForgePilot shall require explicit approval of atomic prototype-scope objects before implementation.

## Details

The scope collection must classify each item as in scope, out of scope, or deferred and define its boundary. The decision must be recorded in GATE-003 with approver, date, decision reference, and approve/revise/reject outcome.

Backlog execution, prototype construction, and implementation must remain blocked until both GATE-002 and GATE-003 are approved.

## Acceptance Criteria

- All scope objects are reviewed through GATE-003.
- Deferred and out-of-scope items are visible in the approval request.
- Implementation does not begin while GATE-002 or GATE-003 is pending, rejected, or requires revision.
- Approved scope drives subsequent backlog and sprint planning.

## Notes

Scope approval is distinct from product-brief approval and both decisions must be recorded.

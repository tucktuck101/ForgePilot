# FR-034: Use larger sprints for low-risk work

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-034 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

When tasks are well-defined, low-risk, and follow established patterns, ForgePilot should allow Codex to plan larger sprints to reduce overhead and accelerate progress.

## Details

Scenarios for larger sprints include:

- Tasks that are repetitive or templated.
- Simple documentation or configuration updates.
- Minor feature additions that follow existing patterns.
- Implementation within a mature codebase with strong testing and conventions.

Larger sprints reduce the number of PRs and issue management overhead while still maintaining quality.

## Acceptance Criteria

- Low-risk tasks are grouped into larger sprints when appropriate.
- The sprint scope and rationale are documented.
- Tests and documentation are still updated as required.

## Notes

This requirement complements FR-032 and FR-033, ensuring that the system remains efficient by adjusting sprint size to the nature of the work.

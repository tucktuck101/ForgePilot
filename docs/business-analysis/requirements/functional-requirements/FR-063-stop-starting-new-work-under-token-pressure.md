# FR-063: Stop starting new work under token pressure

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-063 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall stop starting new work when token pressure is detected.

## Details

Once token pressure is detected, Codex must not initiate new tasks or steps. It should focus on completing or safely pausing the current atomic task and then enter the context recovery workflow. This ensures that work is not interrupted mid-task when the context window is about to be exhausted.

## Acceptance Criteria

- Codex stops beginning new tasks when token pressure is present.
- Codex finishes or safely pauses the current atomic task.
- Codex proceeds to write a resume brief and update project memory as part of the context recovery workflow.

## Notes

Stopping new work under token pressure helps maintain continuity and prevents partial implementations.

# FR-065: Update project memory before stop

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-065 |
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

The system shall update `docs/project-memory.md` when stable project state changes before stopping due to token pressure.

## Details

Before pausing work because of token limits, Codex must ensure that the project memory file reflects the current objective, phase, approved scope, active sprint, stack and tooling, key constraints, pending approval gates, major decisions with ADR links, risks/blockers, and next recommended action. Keeping project memory up to date allows subsequent Codex sessions to quickly regain context without reading all artefacts.

## Acceptance Criteria

- The `docs/project-memory.md` file is updated with stable project state before work stops due to token pressure.
- The project memory remains concise, structured, and limited to stable facts.
- The context recovery workflow reads from this file when resuming.

## Notes

Updating project memory ensures that long-running or paused work can be resumed effectively, reducing context loss and confusion.

# FR-036: Maintain sprint history

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-036 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall archive completed sprint notes in `docs/business-analysis/delivery/sprint-history.md`. This provides a chronological record of what was done in each sprint.

## Details

- When a sprint is completed, Codex should move or append the contents of `current-sprint.md` into `sprint-history.md`.
- Each sprint entry should include the sprint goal, tasks completed, tests run, decisions made, and any unresolved issues.
- Entries should be clearly separated (e.g., with headings or separators) to distinguish between sprints.

Maintaining a history of sprints helps track progress, support retrospectives, and provide context for future work or troubleshooting.

## Acceptance Criteria

- A `sprint-history.md` file exists under `docs/business-analysis/delivery/`.
- Completed sprint notes are preserved in the history file after each sprint.
- Entries are clearly separated and include essential information about the sprint.

## Notes

This requirement ensures transparency and accountability by keeping a record of work done across the life of the project.

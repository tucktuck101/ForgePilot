# FR-036: Maintain sprint history

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
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

# FR-038: Update project memory

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

ForgePilot shall maintain a compact project memory file (`docs/business-analysis/project-memory.md`) and update it whenever stable project state changes. This file summarises the current objective, phase, scope, sprint, stack, constraints, approval gates, major decisions, risks, and next actions.

## Details

- The project memory is not a diary or detailed log; it should summarise essential facts and link to detailed documents.
- Each time the project enters a new phase or sprint, the memory file should be updated to reflect the new state.
- When decisions, constraints, or risks change, the memory file should be updated accordingly.
- The memory file should remain compact (target 1,000–1,500 words) and token efficient.

## Acceptance Criteria

- `docs/business-analysis/project-memory.md` exists and is kept current.
- The file includes sections for the current objective, phase, scope, sprint, stack, constraints, approval gates, major decisions, risks, and next action.
- Updates reflect the latest approved project state without duplicating detailed content.

## Notes

This requirement supports token efficiency and helps Codex resume context quickly across sessions or after hitting token limits.

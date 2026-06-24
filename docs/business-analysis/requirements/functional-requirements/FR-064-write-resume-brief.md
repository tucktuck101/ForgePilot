# FR-064: Write resume brief

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall create or update `docs/delivery/resume-brief.md` before stopping due to token pressure.

## Details

When stopping work because of context or token limits, Codex must write a resume brief capturing the current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, repository status, decisions made, pending approval gates, and the exact next instruction for the next Codex run. This file allows subsequent Codex sessions to resume work seamlessly.

## Acceptance Criteria

- The `docs/delivery/resume-brief.md` file is created or updated when work stops due to token pressure.
- The resume brief includes the required fields: current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, repository status, decisions made, pending approval gates, and exact next instruction.
- The context recovery workflow references this file as part of the next-run instructions.

## Notes

Maintaining a clear resume brief ensures that long-running tasks can be paused and resumed without losing context.

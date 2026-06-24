# FR-066: Include required resume information

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

The system shall ensure that the resume brief includes the current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, current repo status, decisions made, pending approval gates, and exact next instruction.

## Details

The resume brief serves as a continuation note for the next Codex run. It must contain all necessary information to resume the project without confusion. The brief should not include extraneous details that can be found in other artefacts. It should concisely capture the state of work at the point of pausing.

## Acceptance Criteria

- The resume brief includes the specified fields: current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, current repo status, decisions made, pending approval gates, and exact next instruction.
- Information is accurate, concise, and sufficient to resume work.
- The next-run instructions are clear and actionable without requiring additional context.

## Notes

Including required information in the resume brief helps ensure continuity and clarity across Codex sessions.

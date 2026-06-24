# FR-066: Include required resume information

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-066 |
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

The system shall ensure that the resume brief includes the current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, current repo status, decisions made, pending approval gates, and exact next instruction.

## Details

The resume brief serves as a continuation note for the next Codex run. It must contain all necessary information to resume the project without confusion. The brief should not include extraneous details that can be found in other artefacts. It should concisely capture the state of work at the point of pausing.

## Acceptance Criteria

- The resume brief includes the specified fields: current phase, sprint goal, completed work, incomplete work, files changed, commands/tests run, current repo status, decisions made, pending approval gates, and exact next instruction.
- Information is accurate, concise, and sufficient to resume work.
- The next-run instructions are clear and actionable without requiring additional context.

## Notes

Including required information in the resume brief helps ensure continuity and clarity across Codex sessions.

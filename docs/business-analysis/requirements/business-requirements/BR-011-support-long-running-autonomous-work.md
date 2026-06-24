# BR-011: Support long-running autonomous work

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-011 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall support long-running autonomous workflows and handle context limits through planned continuity mechanisms.

## Details

Codex sessions may hit token/context limits. ForgePilot must provide mechanisms to summarise the current state, pause work safely, and resume later. This includes storing the current phase, sprint goal, completed work, pending tasks, changed files, commands run, decisions made, and next actions in dedicated Markdown files (`project-memory.md`, `current-sprint.md`, and `resume-brief.md`). The system should treat context limits as a normal part of operation rather than a failure state.

## Acceptance Criteria

- Codex can detect token pressure and stop starting new work.
- Codex updates `current-sprint.md` and writes `resume-brief.md` with all required resume information.
- `project-memory.md` records stable facts about the project state.
- A subsequent Codex run can resume by reading these files.

## Notes

Long-running workflows require resilience to LLM context constraints. This requirement ensures continuity across sessions.

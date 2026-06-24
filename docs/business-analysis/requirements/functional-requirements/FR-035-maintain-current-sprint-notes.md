# FR-035: Maintain current sprint notes

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

ForgePilot shall have Codex maintain an up-to-date log of the current sprint’s work in `docs/business-analysis/delivery/current-sprint.md`. This file tracks progress, decisions, and context for the ongoing sprint.

## Details

- At the start of each sprint, Codex should create or update `current-sprint.md` with the sprint goal, tasks, and planned approach.
- During implementation, Codex records work performed, files changed, tests run, obstacles encountered, and decisions made.
- When the sprint concludes, `current-sprint.md` is finalised and archived in `sprint-history.md`.

The current sprint notes help maintain continuity, especially across sessions or when token limits are encountered.

## Acceptance Criteria

- `docs/business-analysis/delivery/current-sprint.md` exists and is updated during each sprint.
- The file includes a clear overview of the sprint goal, tasks, work performed, and pending tasks.
- The notes are concise and do not duplicate detailed content available elsewhere.

## Notes

This requirement supports context retention and clarity, especially for token-limit recovery and handoff between human and AI agents.

# FR-035: Maintain current sprint notes

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-035 |
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

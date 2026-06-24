# FR-067: Maintain compact project memory

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-067 |
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

The system shall maintain `docs/project-memory.md` as a concise, structured record of stable project information.

## Details

Project memory should contain only stable facts necessary to resume work or make decisions, such as the current objective, phase, approved scope, active sprint, stack and tooling, key constraints, pending approval gates, major decisions with ADR links, risks/blockers, and next recommended action. It should avoid logs or transcripts and remain limited to about 1,000–1,500 words. When project state changes materially, stale information should be overwritten rather than appended.

## Acceptance Criteria

- `docs/project-memory.md` remains concise, structured, and limited to stable facts.
- The file is updated by overwriting stale information rather than appending long histories.
- The project memory links to detailed artefacts instead of duplicating content.
- The file is referenced by the context recovery workflow for re-entry into the project.

## Notes

Maintaining a compact project memory file ensures efficient context usage and faster recovery after long-running tasks.

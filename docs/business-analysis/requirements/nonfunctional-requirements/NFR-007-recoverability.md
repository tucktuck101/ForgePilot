# NFR-007: Recoverability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-007 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

The system must support recovery across Codex sessions.

## Details

ForgePilot should persist enough project state across sessions to allow Codex to resume work without re-reading the entire repository. It should maintain a concise `docs/project-memory.md`, `docs/delivery/current-sprint.md`, and `docs/delivery/resume-brief.md` as continuity files. When token limits are reached, the system must pause safely, update these files, and provide clear next instructions. The next run should continue from these files without losing context.

## Notes

Recoverability is critical for long-running tasks that exceed a single session or context window.

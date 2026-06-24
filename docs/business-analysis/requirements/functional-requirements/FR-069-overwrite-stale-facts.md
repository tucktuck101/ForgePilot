# FR-069: Overwrite Stale Facts

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-069 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this requirement changes materially |

## Summary

Project memory should overwrite outdated information rather than accumulating long logs or transcripts.

## Details

The project memory file (`docs/project-memory.md`) is intended to capture stable facts about the current state of the prototype. To keep this file concise and useful, Codex must overwrite stale or outdated facts instead of appending new entries indefinitely. This ensures that the memory remains focused on the latest known truth rather than becoming a long diary.

## Acceptance Criteria

- The system updates `docs/project-memory.md` by replacing outdated facts with the latest information.
- The memory file remains concise and under the token budget specified in the brief.
- Sprint notes and resume briefs remain separate and are not merged into project memory.

## Notes

This requirement supports the nonfunctional requirement of token efficiency and maintainability.

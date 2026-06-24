# FR-070: Link to Detailed Artefacts

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-070 |
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

Project memory and other summaries should link to detailed artefacts rather than duplicating their content.

## Details

To maximise token efficiency and avoid duplication, the system must place detailed information in dedicated documents under `docs/` and link to them from summary files such as project memory, sprint notes, and resume briefs. This ensures that long descriptions or decisions are stored in the appropriate artefact (for example, solution design files, ADRs, or sprint notes) while summary documents reference them by relative link. Codex should avoid copying large sections of text into multiple places.

## Acceptance Criteria

- Project memory entries link to relevant discovery, design, delivery, and decision artefacts rather than duplicating their content.
- Sprint notes summarise decisions and reference the full details by link.
- Resume briefs contain links to relevant files instead of repeating their content.

## Notes

This requirement supports token efficiency and maintainability across long-running sessions.

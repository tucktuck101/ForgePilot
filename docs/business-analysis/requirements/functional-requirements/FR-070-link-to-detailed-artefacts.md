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
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md), [SC-010](../../discovery/success-criteria/SC-010-token-efficient-documentation-retrieval.md) |
| Update rule | Update when this requirement changes materially |

## Summary

Project memory and other summaries should link to detailed artefacts rather than duplicating their content.

## Details

To maximise token efficiency and avoid duplication, the system must place detailed information in dedicated documents under `docs/` and link to them from summary files such as indexes, project memory, sprint notes, and resume briefs. Issues and indexes should act as retrieval entry points so Codex loads only the directly relevant linked objects. Human-facing summaries should provide orientation and then link to the same authoritative detail. Codex should avoid copying large sections of text into multiple places or loading the full documentation corpus by default.

## Acceptance Criteria

- Project memory entries link to relevant discovery, design, delivery, and decision artefacts rather than duplicating their content.
- Sprint notes summarise decisions and reference the full details by link.
- Resume briefs contain links to relevant files instead of repeating their content.
- Compact indexes and issues provide bounded retrieval paths to directly relevant objects.
- Human-facing summaries and Codex retrieval paths resolve to the same detailed Markdown artefacts.

## Notes

This requirement supports token efficiency and maintainability across long-running sessions.

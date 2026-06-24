# NFR-014: Doc-Object Consistency

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-014 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md), [QLT-014](../../discovery/quality-checks/QLT-014-documentation-consumption-readiness.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

All ForgePilot documents must follow a consistent doc‑object style.

## Details

Each formal artefact created by ForgePilot—such as requirements, personas, user stories, briefs, and ADRs—must contain a document metadata table with fields like Document type, Status, Owner/audience, Source, Linked artefacts, and Update rule. Documents should use predictable headings, stable IDs, compact indexes, and relative links. This consistency enables selective Codex retrieval, human navigation, and later rendering from the same Markdown without requiring duplicated content.

## Acceptance Criteria

- Live objects use the collection's metadata and heading conventions.
- Stable IDs and indexes provide predictable retrieval and navigation.
- Relative links connect summaries, traceability records, and detailed objects.
- A future presentation layer can interpret the structure without changing the authoritative source.

## Notes

A standardised document structure reduces confusion and promotes reuse across different projects.

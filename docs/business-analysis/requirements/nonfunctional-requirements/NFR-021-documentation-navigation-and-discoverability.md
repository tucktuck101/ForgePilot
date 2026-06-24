# NFR-021: Documentation Navigation and Discoverability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-021 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, users, reviewers, maintainers, Codex |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [US-038](../../user-stories/US-038-navigate-forgepilot-documentation.md), [SC-009](../../discovery/success-criteria/SC-009-human-readable-documentation-consumption.md), [QLT-014](../../discovery/quality-checks/QLT-014-documentation-consumption-readiness.md) |
| Update rule | Update when the documentation navigation or discoverability quality changes materially |

## Summary

ForgePilot documentation shall make major artefacts and their relationships easy to find for both humans and Codex.

## Details

Indexes, headings, summaries, stable IDs, metadata, and relative links must support orientation from a high-level entry point to authoritative detail. Search capability may be supplied by repository tooling or a later approved presentation layer, but discoverability must not depend on a second manually maintained content store.

## Acceptance Criteria

- Every major collection and singleton artefact is reachable from the Business Analysis or Discovery index.
- A reader can identify an artefact's purpose, status, and related objects without scanning the complete corpus.
- A fresh Codex session can start from an issue, index, or summary and retrieve directly relevant objects.
- Broken links, orphaned live objects, and unindexed major artefacts fail documentation readiness.

# FR-050: Validate doc-object metadata

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-050 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

The system shall validate live doc-object metadata, collection structure, IDs, priorities, traceability links, and approval state.

## Details

Validation must scan live discovery, persona, user-story, and requirement objects. Templates are checked for field definitions but are excluded from live-value checks.

Required checks include unique IDs; valid MoSCoW priority; non-empty source, source needs, evidence, related objects, and update rule; required collection index and template files; index-to-object consistency; and resolvable relative links.

## Acceptance Criteria

- Validation reports duplicate or missing object IDs.
- Validation reports invalid or unassigned priorities.
- Validation reports missing source-need, evidence, or related-object links.
- Validation reports missing collection indexes, templates, or live objects.
- Validation reports broken relative links and clearly identifies the source file.
- Approval objects with pending status cannot be interpreted as approval.

## Notes

Placeholder values are permitted in templates but not in live objects.

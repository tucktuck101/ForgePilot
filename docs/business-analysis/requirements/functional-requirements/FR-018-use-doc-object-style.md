# FR-018: Use doc-object style

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-018 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

All major BA artefacts shall use a consistent, atomic doc-object structure.

## Details

Each live object must include a unique object ID, document type, status, MoSCoW priority, owner/audience, source, source-need links, evidence links, related-object links, and update rule.

Collections must use stable IDs and contain an index, template, and one Markdown file per atomic object. Indexes remain compact and must not duplicate the full object body.

## Acceptance Criteria

- All live discovery, persona, story, and requirement objects contain the required metadata.
- Related objects are expressed as direct relative links.
- Templates document the same metadata contract.
- Multi-entry traceable entities are represented as collections rather than monolithic lists.

## Notes

Explanatory sections such as symptoms, root causes, and impacts may remain within a singleton analysis document when they are not independently governed objects.

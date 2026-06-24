# FR-027: Keep Markdown as the knowledge source

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-027 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Requirements Index](../index.md) |
| Related objects | [Requirements Index](../index.md), [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md), [SC-012](../../discovery/success-criteria/SC-012-documentation-source-of-truth-preservation.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall use repository Markdown as the canonical source of product, design, delivery, decision, and documentation knowledge. Issues and any future human-facing presentation shall reference or derive from that source.

## Details

- Product briefs, requirements, personas, user stories, solution designs, sprints, and ADRs are stored as Markdown files in the `docs/` directory.
- GitHub Issues should link to these documents rather than replicate their content.
- Updates to core information should happen in the Markdown files first, with issues or comments referencing the changes.
- Any later generated portal must consume the repository Markdown and must not require a separately edited authoritative copy.
- Generated or published views are presentation artefacts; they do not replace repository history, metadata, traceability, or approval state.

## Acceptance Criteria

- All key artefacts exist as Markdown files within `docs/business-analysis`.
- Issues and PRs reference these files via relative links.
- Duplicate or conflicting information in Issues is minimised.
- Any future portal identifies repository Markdown as its source and does not introduce a manually maintained duplicate.

## Notes

This separation ensures clarity between long-lived knowledge and transient work logs, and supports token-efficient operations.

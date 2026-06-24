# BR-010: Use Markdown as the project knowledge base

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-010 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md), [OPT-006](../../discovery/options/OPT-006-generated-documentation-portal.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall use repository Markdown as the source of truth for product, design, delivery state, decision records, handoff information, Codex retrieval, and human documentation presentation.

## Details

All core project artefacts—including discovery artefacts, solution designs, delivery state, ADRs, sprint notes, test reports, release notes, and handoff documents—shall be captured in Markdown files within the repository. Compact indexes and links support selective Codex retrieval and human navigation from the same source. GitHub Issues track work execution, and a future portal may render the Markdown for human consumption, but neither becomes a competing knowledge store.

## Acceptance Criteria

- Product briefs, designs, delivery plans, decisions, and handoff docs are stored as Markdown.
- Markdown files follow the doc-object format with metadata.
- Documentation is organised under `docs/` in clear subfolders.
- Human-facing views are derived from repository Markdown rather than maintained separately.
- Issues, generated views, and publication surfaces link back to or identify the authoritative Markdown source.

## Notes

This requirement centralises knowledge in a portable, version-controlled format.

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
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall use Markdown files as the source of truth for product, design, delivery state, decision records, and handoff information.

## Details

All core project artefacts—including discovery artefacts, solution designs, delivery state, ADRs, sprint notes, test reports, release notes, and handoff documents—shall be captured in Markdown files within the repository. This ensures that both humans and Codex can read and update the information easily. GitHub Issues track work execution, but the knowledge base resides in Markdown.

## Acceptance Criteria

- Product briefs, designs, delivery plans, decisions, and handoff docs are stored as Markdown.
- Markdown files follow the doc-object format with metadata.
- Documentation is organised under `docs/` in clear subfolders.

## Notes

This requirement centralises knowledge in a portable, version-controlled format.

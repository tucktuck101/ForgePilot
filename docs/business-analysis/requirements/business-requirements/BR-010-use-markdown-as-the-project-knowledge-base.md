# BR-010: Use Markdown as the project knowledge base

## Document Metadata

| Field | Value |
|---|---|
| Document type | Business Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index.md](index.md) |
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

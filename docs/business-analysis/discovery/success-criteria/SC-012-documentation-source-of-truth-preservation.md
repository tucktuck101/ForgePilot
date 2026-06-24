# SC-012: Documentation source-of-truth preservation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | SC-012 |
| Document type | Success Criterion |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, reviewers, maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-005](../stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [BR-010](../../requirements/business-requirements/BR-010-use-markdown-as-the-project-knowledge-base.md), [FR-027](../../requirements/functional-requirements/FR-027-keep-markdown-as-knowledge-source.md), [OPT-007](../options/OPT-007-github-wiki-separate-documentation-store.md) |
| Update rule | Update when the documentation authority or publication model changes materially |

## Criterion

Repository Markdown remains the authoritative source for both Codex retrieval and every human-facing documentation presentation.

## Measurement

Inspect documentation changes and any later generated output. Target: authoritative edits occur in repository Markdown, generated views identify their source, and no manually maintained portal or Wiki copy contains competing project truth.

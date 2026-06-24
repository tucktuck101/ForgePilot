# OPT-005: Markdown-only documentation consumption

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-005 |
| Document type | Option |
| Status | Not recommended as the sole human-consumption path |
| Priority | Could |
| Owner/audience | Product Owner, users, reviewers, maintainers, Codex |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-006](OPT-006-generated-documentation-portal.md), [OPT-007](OPT-007-github-wiki-separate-documentation-store.md), [GATE-001](../approval-gates/GATE-001-options-and-direction-approval.md) |
| Update rule | Update when documentation-consumption evidence or constraints change materially |

## Description

Keep repository Markdown, indexes, and GitHub file browsing as the only human-facing documentation experience.

## Analysis

- Benefits: no publication mechanism, dependency, generated output, or separate hosting surface is required.
- Costs: navigation, search, visual hierarchy, and cross-document orientation depend on repository browsing conventions.
- Risks: non-technical readers may struggle to discover or consume the granular knowledge graph.
- Conclusion: retain as the minimum viable and fallback consumption path, but do not treat it as sufficient evidence that the human-consumption need is met.

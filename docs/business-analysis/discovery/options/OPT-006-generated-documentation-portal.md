# OPT-006: Human-friendly portal generated from repository Markdown

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-006 |
| Document type | Option |
| Status | Recommended; pending approval |
| Priority | Must |
| Owner/audience | Product Owner, users, reviewers, maintainers, Codex |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-005](OPT-005-markdown-only-documentation-consumption.md), [OPT-007](OPT-007-github-wiki-separate-documentation-store.md), [OQ-006](../open-questions/OQ-006-documentation-portal-implementation-approach.md), [GATE-001](../approval-gates/GATE-001-options-and-direction-approval.md) |
| Update rule | Update when documentation-consumption evidence, constraints, or the later implementation decision changes materially |

## Description

Provide a future human-friendly documentation portal generated from the authoritative repository Markdown.

## Analysis

- Benefits: preserves one version-controlled source while enabling improved reading, navigation, search, and presentation for humans.
- Costs: later solution design must define generation, information architecture, publication controls, maintenance, and validation.
- Risks: publishing generated documentation may expose sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information.
- Recommendation: adopt the generated-portal direction at the BA level, subject to approval, while deferring implementation design and tooling selection.

## Deferred Implementation Decision

MkDocs and GitHub Pages are candidate mechanisms, not approved selections. The later design must compare them with credible alternatives, address publication safety, and preserve Markdown as the sole source of truth before implementation begins.

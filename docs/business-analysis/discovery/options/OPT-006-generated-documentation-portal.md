# OPT-006: Human-friendly portal generated from repository Markdown

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-006 |
| Document type | Option |
| Status | Approved direction |
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
- Recommendation: adopt the generated‑portal direction at the BA level; this direction has been approved via GATE‑001; implementation design and tooling selection remain deferred to solution design.

## Deferred Implementation Decision

[OQ-006](../open-questions/OQ-006-documentation-portal-implementation-approach.md) records MkDocs Material with GitHub Pages as the Product Owner's preferred proposal after comparison with Docusaurus. This preference is not an approved architecture, dependency, publication target, or implementation boundary. Approved solution design must address publication safety and preserve Markdown as the sole source of truth before implementation begins.

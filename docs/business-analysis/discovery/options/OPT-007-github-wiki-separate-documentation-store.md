# OPT-007: GitHub Wiki as a separate documentation store

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-007 |
| Document type | Option |
| Status | Not recommended |
| Priority | Could |
| Owner/audience | Product Owner, users, reviewers, maintainers, Codex |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-005](OPT-005-markdown-only-documentation-consumption.md), [OPT-006](OPT-006-generated-documentation-portal.md), [GATE-001](../approval-gates/GATE-001-options-and-direction-approval.md) |
| Update rule | Update when documentation-consumption evidence or source-of-truth constraints change materially |

## Description

Maintain human-facing documentation in a GitHub Wiki separate from the repository Markdown knowledge graph.

## Analysis

- Benefits: provides a familiar browsable interface with low initial setup.
- Costs: creates a second editing location and requires synchronization with repository documentation.
- Risks: duplicate facts, broken traceability, inconsistent approvals, and drift between Codex and human views.
- Conclusion: do not use a separate Wiki as the authoritative or manually duplicated documentation store. A generated presentation of repository Markdown is preferred.

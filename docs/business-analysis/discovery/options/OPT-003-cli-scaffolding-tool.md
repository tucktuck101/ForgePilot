# OPT-003: CLI or scaffolding tool

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-003 |
| Document type | Option |
| Status | Not recommended for prototype |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-003](../stakeholder-needs/SN-003-repository-onboarding.md), [SN-006](../stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-002](../evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [GATE-001](../approval-gates/GATE-001-options-and-direction-approval.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Description

Build a command-line installer that detects repository state, writes ForgePilot assets, and performs validation.

## Analysis

- Benefits: stronger installation control and repeatability.
- Costs: adds executable product scope, packaging, compatibility, and support obligations.
- Risks: premature implementation before validating the repository-template model.
- Conclusion: consider after the template workflow is validated.

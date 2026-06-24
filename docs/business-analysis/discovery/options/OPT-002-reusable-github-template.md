# OPT-002: Reusable GitHub template

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OPT-002 |
| Document type | Option |
| Status | Pending approval |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-001](../stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-003](../stakeholder-needs/SN-003-repository-onboarding.md), [SN-005](../stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-008](../stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-010](../stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [GATE-001](../approval-gates/GATE-001-options-and-direction-approval.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Description

Package durable instructions, atomic BA objects, templates, validation conventions, and delivery workflows in a reusable GitHub repository template.

## Analysis

- Benefits: Git-native, portable, inspectable, version-controlled, and aligned with the documented operating model.
- Costs: requires careful conflict handling and maintenance of template conventions.
- Risks: repository instructions alone may not provide enough orchestration for every stack.
- Recommendation: approve as the primary direction for the prototype, subject to GATE-001.

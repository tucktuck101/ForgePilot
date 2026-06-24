# PH-002: Indexed objects reduce context load

## Document Metadata

| Field | Value |
|---|---|
| Object ID | PH-002 |
| Document type | Prototype Hypothesis |
| Status | Unvalidated |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-005](../stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-008](../stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-005](../evidence/EVD-005-measurement-baseline-gap.md) |
| Related objects | [SC-006](../success-criteria/SC-006-context-efficient-navigation.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Hypothesis

Compact indexes plus atomic related objects allow Codex to retrieve sufficient context without loading large monolithic documents.

## Test

Measure the files and tokens required for representative discovery, approval, and resume tasks against a monolithic baseline.

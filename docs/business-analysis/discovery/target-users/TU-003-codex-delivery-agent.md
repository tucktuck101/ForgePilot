# TU-003: Codex Delivery Agent

## Document Metadata

| Field | Value |
|---|---|
| Object ID | TU-003 |
| Document type | Target User |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-004](../stakeholder-needs/SN-004-adaptive-environments-and-stacks.md), [SN-005](../stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](../stakeholder-needs/SN-006-repeatable-quality-validation.md), [SN-007](../stakeholder-needs/SN-007-secrets-and-security-safety.md), [SN-008](../stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-002](../evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [persona-002](../../personas/persona-002-codex-delivery-agent.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

The autonomous repository agent that reads compact indexes, loads related objects, conducts discovery, and executes approved delivery work.

## Goals and Context

- Retrieve only the context needed for the current decision.
- Act autonomously within explicit safety boundaries.
- Preserve traceability and resumable state.

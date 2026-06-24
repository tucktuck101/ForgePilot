# SN-002: Safe autonomous operation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | SN-002 |
| Document type | Stakeholder Need |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-007](../evidence/EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [ASM-006](../assumptions/ASM-006-explicit-stage-context-improves-codex-operation.md), [RSK-008](../risks/RSK-008-wrong-stage-codex-behaviour.md), [OQ-007](../open-questions/OQ-007-stage-aware-guidance-representation.md), [SC-013](../success-criteria/SC-013-stage-appropriate-codex-operation.md), [Stakeholder Needs Index](index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Need

Users need routine work to proceed autonomously while material product, risk, cost, credential, deployment, merge, and acceptance decisions remain explicitly human-approved.

## Stage-Aware Process Need

ForgePilot should provide enough operating context for Codex to identify the current type of work and apply suitable behaviours, outputs, constraints, review criteria, quality gates, approval gates, and stop conditions.

The need spans discovery and business analysis, product scope shaping, solution-design preparation, implementation sprints, validation and QA, pull-request readiness, and context recovery. These work types require materially different behaviour. For example, business analysis should reduce ambiguity, improve traceability, and avoid premature design or implementation, while approved implementation work should make scoped changes, run relevant checks, update affected documentation, and prepare review-ready delivery evidence.

A single generic instruction set may be insufficient because it can encourage wrong-stage behaviour, including premature implementation, unapproved design choices, missed gates, inconsistent output quality, or unsafe continuation.

This need does not approve an implementation. [OQ-007](../open-questions/OQ-007-stage-aware-guidance-representation.md) records concise `AGENTS.md` workflow routing, reusable skills, and issue-level execution metadata as the preferred representation, subject to approved solution design and validation.

## Acceptance or Validation

The broader safe-autonomy need remains represented by linked stories and requirements. The preferred stage-aware representation must still be validated through [SC-013](../success-criteria/SC-013-stage-appropriate-codex-operation.md); no representation or implementation is accepted by this discovery object.

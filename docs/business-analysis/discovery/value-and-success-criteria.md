# DISC-007: Value and Success Definition

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-007 |
| Document type | Value and Success Definition |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, future maintainers |
| Source | Linked needs, value hypotheses, prototype hypotheses, and success criteria |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](stakeholder-needs/SN-006-repeatable-quality-validation.md), [SN-008](stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-009](stakeholder-needs/SN-009-complete-prototype-handoff.md), [SN-010](stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-004](evidence/EVD-004-user-research-gap.md), [EVD-005](evidence/EVD-005-measurement-baseline-gap.md) |
| Related objects | [Value Hypotheses](value-hypotheses/index.md), [Success Criteria](success-criteria/index.md), [Prototype Hypotheses](prototype-hypotheses/index.md), [Scope](scope.md) |
| Update rule | Update when a capability, value hypothesis, measurement, or prototype boundary changes |

## Value Model

| Major capability | Value recipient | Value type | Value hypothesis | Observable success | Prototype learning |
|---|---|---|---|---|---|
| Guided discovery and approval-ready scope | Solo Builder / Product Owner | Speed, quality, learning | [VH-001](value-hypotheses/VH-001-faster-path-to-approved-scope.md) | [SC-001](success-criteria/SC-001-complete-discovery-package.md), [SC-005](success-criteria/SC-005-discovery-cycle-measurement.md) | Whether structured discovery reduces elapsed effort and avoidable revision cycles |
| Explicit material approval gates | Approval Authority and Product Owner | Risk reduction, control | [VH-003](value-hypotheses/VH-003-safer-autonomous-decisions.md) | [SC-004](success-criteria/SC-004-approval-gate-compliance.md) | Whether gates prevent unapproved material action without creating routine approval noise |
| Autonomous routine workflow and backlog handoff | Product Owner and Codex | Time saving, throughput | [VH-002](value-hypotheses/VH-002-less-routine-micromanagement.md) | Pilot interaction classification and linked issue acceptance evidence | Whether routine planning and delivery can proceed with materially fewer supervision interactions |
| Indexed, traceable repository knowledge | Codex, reviewer, maintainer | Maintainability, reuse, auditability | [VH-004](value-hypotheses/VH-004-maintainable-and-resumable-delivery.md) | [SC-002](success-criteria/SC-002-complete-traceability-coverage.md), [SC-003](success-criteria/SC-003-zero-broken-document-links.md), [SC-006](success-criteria/SC-006-context-efficient-navigation.md) | Whether a fresh session or reviewer can recover context without loading the full corpus |
| Repeatable validation and complete handoff | Product Owner, reviewer, maintainer | Quality, confidence, continuity | [VH-003](value-hypotheses/VH-003-safer-autonomous-decisions.md), [VH-004](value-hypotheses/VH-004-maintainable-and-resumable-delivery.md) | [SC-007](success-criteria/SC-007-repeatable-factory-validation.md), [SC-008](success-criteria/SC-008-complete-prototype-handoff.md) | Whether defects, missing context, and unsafe state are exposed before release or continuation |

## Prototype Value Threshold

The prototype is valuable if it demonstrates all of the following without claiming market validation:

1. A vague idea can be converted into a complete, linked, approval-ready pre-solution package.
2. Every material decision encountered is either explicitly approved or remains visibly blocked.
3. A delivery issue can be generated from approved scope with enough context to execute safely and resume later.
4. A fresh reviewer can follow the evidence-to-need-to-requirement-to-scope path and identify current approval state.
5. Validation exposes missing files, metadata, traceability, broken links, and unsafe secret patterns.

## Measurement Rules

- Structural pass results prove repository conformance only; they do not prove user value.
- Improvement claims require a recorded baseline and comparable pilot observations.
- Unvalidated hypotheses remain labelled `Unvalidated` until supporting evidence is linked.
- Failed or inconclusive pilot results must update the affected hypothesis, risk, scope, or option rather than being omitted.
- Product-brief approval confirms the value model is acceptable to test; it does not validate the hypotheses.

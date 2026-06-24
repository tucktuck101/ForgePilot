# DISC-005: BA Quality Assessment

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-005 |
| Document type | BA Quality Assessment |
| Status | Not ready |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-003](evidence/EVD-003-repository-gap-observation.md), [EVD-004](evidence/EVD-004-user-research-gap.md), [EVD-005](evidence/EVD-005-measurement-baseline-gap.md) |
| Related objects | [Quality Checks](quality-checks/index.md), [Approval Gates](approval-gates/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Passing Rule

- No mandatory check may score 0.
- Problem framing, measurable outcomes, options analysis, end-to-end traceability, and approval readiness must each score 2.
- Overall score must be at least 80%.

## Assessment

| Check | Area | Score | Assessment evidence |
|---|---|---:|---|
| [QLT-001](quality-checks/QLT-001-problem-framing.md) | Problem framing | 2 | Problem statement separates required concepts. |
| [QLT-002](quality-checks/QLT-002-current-state-understanding.md) | Current-state understanding | 2 | Current-state actors, flow, constraints, and gaps are explicit. |
| [QLT-003](quality-checks/QLT-003-root-cause-separation.md) | Root-cause separation | 2 | Causes are separated from symptoms and proposed direction. |
| [QLT-004](quality-checks/QLT-004-evidence-quality.md) | Evidence quality | 1 | Repository and stakeholder evidence exist; external research is absent. |
| [QLT-005](quality-checks/QLT-005-target-user-clarity.md) | Target-user clarity | 2 | Six target-user objects link to canonical personas. |
| [QLT-006](quality-checks/QLT-006-measurable-outcomes.md) | Measurable outcomes | 2 | Criteria define checks, targets, or baseline actions. |
| [QLT-007](quality-checks/QLT-007-options-analysis.md) | Options analysis | 2 | Four option objects include recommendation, alternatives, costs, and risks. |
| [QLT-008](quality-checks/QLT-008-scope-clarity.md) | Scope clarity | 2 | Atomic in-scope, out-of-scope, and deferred items exist. |
| [QLT-009](quality-checks/QLT-009-prioritisation.md) | Prioritisation | 2 | MoSCoW is assigned across stories, requirements, and discovery objects. |
| [QLT-010](quality-checks/QLT-010-end-to-end-traceability.md) | End-to-end traceability | 2 | Needs map to evidence, users, stories, requirements, and criteria. |
| [QLT-011](quality-checks/QLT-011-risk-and-assumption-management.md) | Risk and assumption management | 2 | Atomic objects include owners or validation actions. |
| [QLT-012](quality-checks/QLT-012-approval-readiness.md) | Approval readiness | 1 | Gate objects are complete but all required decisions remain pending. |
| [QLT-013](quality-checks/QLT-013-link-and-index-integrity.md) | Link and index integrity | 2 | Collections and relative links are validated. |

## Result

- Score: **24/26 (92%)**.
- Readiness: **Not ready for solution design or implementation**.
- Blocking condition: QLT-012 scores 1 because GATE-001, GATE-002, and GATE-003 are pending.
- Evidence caution: value hypotheses remain unvalidated because external user research and quantitative baselines are absent.

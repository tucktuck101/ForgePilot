# Discovery Index

## Document Metadata

| Field | Value |
|---|---|
| Document type | Index |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | Discovery objects linked below |
| Linked artefacts | [Personas](../personas/index.md), [User Stories](../user-stories/index.md), [Requirements](../requirements/index.md) |
| Update rule | Update when discovery structure, object state, or approval state changes |

## Purpose

Provide compact navigation to pre-solution evidence and decisions. Load this index first, then only the directly related objects needed for the current task. The same linked Markdown source is also intended to support a future human-friendly documentation presentation without becoming a second source of truth.

## Singleton Documents

| Document | Purpose | Status | Link |
|---|---|---|---|
| Product brief | Consolidated product intent and recommendation | Approved | [product-brief.md](product-brief.md) |
| Problem statement | Problem, symptoms, causes, impact, and outcome | Draft | [problem-statement.md](problem-statement.md) |
| Current state | Existing workflow, constraints, and gaps | Draft | [current-state.md](current-state.md) |
| Stakeholder map | Roles, accountability, authority, and trade-offs | Draft | [stakeholder-map.md](stakeholder-map.md) |
| Value and success definition | Capability-to-value and learning model | Draft | [value-and-success-criteria.md](value-and-success-criteria.md) |
| Prototype scope | Consolidated in/out/deferred boundary and dependencies | Approved | [scope.md](scope.md) |
| Workflows | Current/target flows, handoffs, exceptions, and operations | Draft | [workflows.md](workflows.md) |
| Traceability matrix | Need-to-outcome mapping | Draft | [traceability-matrix.md](traceability-matrix.md) |
| BA quality assessment | Supplied-rubric review attempts and final decision | Passed | [ba-quality-assessment.md](ba-quality-assessment.md) |

## Object Collections

| Collection | ID prefix | Link |
|---|---|---|
| Target users | TU | [target-users/index.md](target-users/index.md) |
| Stakeholder needs | SN | [stakeholder-needs/index.md](stakeholder-needs/index.md) |
| Evidence | EVD | [evidence/index.md](evidence/index.md) |
| Prototype hypotheses | PH | [prototype-hypotheses/index.md](prototype-hypotheses/index.md) |
| Value hypotheses | VH | [value-hypotheses/index.md](value-hypotheses/index.md) |
| Success criteria | SC | [success-criteria/index.md](success-criteria/index.md) |
| Scope items | SCP | [scope-items/index.md](scope-items/index.md) |
| Options | OPT | [options/index.md](options/index.md) |
| Risks | RSK | [risks/index.md](risks/index.md) |
| Assumptions | ASM | [assumptions/index.md](assumptions/index.md) |
| Open questions | OQ | [open-questions/index.md](open-questions/index.md) |
| Approval gates | GATE | [approval-gates/index.md](approval-gates/index.md) |
| Definition of done | DOD | [definition-of-done/index.md](definition-of-done/index.md) |
| BA quality checks | QLT | [quality-checks/index.md](quality-checks/index.md) |

## Mandatory Sequence

1. Discovery and options analysis may proceed while gates are pending.
2. Product direction is finalised by approved [GATE-001](approval-gates/GATE-001-options-and-direction-approval.md).
3. Solution Design may begin because [GATE-002](approval-gates/GATE-002-product-brief-approval.md) is approved.
4. The approved prototype scope is recorded by [GATE-003](approval-gates/GATE-003-prototype-scope-approval.md); backlog preparation and implementation planning must still follow Design, Plan, and later material approval gates.
5. Later material decisions follow the [approval gate operating policy](approval-gates/operating-policy.md); an earlier approval does not pre-approve a later gate.

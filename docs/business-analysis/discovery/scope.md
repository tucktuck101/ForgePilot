# DISC-008: Prototype Scope

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-008 |
| Document type | Prototype Scope |
| Status | Approved |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, future maintainers |
| Source | Existing scope items, requirements, stories, hypotheses, constraints, and open questions |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-003](stakeholder-needs/SN-003-repository-onboarding.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](stakeholder-needs/SN-006-repeatable-quality-validation.md), [SN-008](stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-009](stakeholder-needs/SN-009-complete-prototype-handoff.md), [SN-011](stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-004](evidence/EVD-004-user-research-gap.md), [EVD-006](evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [Scope Items](scope-items/index.md), [GATE-003](approval-gates/GATE-003-prototype-scope-approval.md), [Traceability Matrix](traceability-matrix.md) |
| Update rule | Update when GATE-003 records revision or approval, or when a dependency invalidates the proposed boundary |

## Scope Objective

Test the repository-native ForgePilot operating model as a bounded template prototype. The prototype should prove the discovery-to-handoff control flow and its traceability; it is not a production orchestration platform and does not need to prove broad stack or deployment compatibility.

## Proposed In-Scope Capability Slices

| Slice | Included outcome | Requirement boundary | Completion evidence |
|---|---|---|---|
| P1. Repository operating skeleton | Durable instructions, separated project artefacts, and safe intake rules exist | FR-001, FR-002, FR-005, FR-006, FR-011–FR-014 | Required files exist; a fixture conflict is reported without overwrite and records the required approval path |
| P2. Pre-solution discovery | Chat-led discovery produces problem, users, needs, value, options, risks, workflows, requirements, and scope | FR-015–FR-020; NFR-002, NFR-013–NFR-015, NFR-018 | A sample discovery package passes the BA gate and remains pending where human approval is absent |
| P3. Controlled design and backlog handoff | Approved scope can hand off to bounded design and executable issues without bypassing gates | FR-021, FR-023–FR-029, FR-031, FR-041–FR-045; NFR-005, NFR-016 | A gated issue contains required context; no implementation issue is executable while GATE-002 or GATE-003 is pending |
| P4. Validation and safety | Repeatable checks cover required structure, metadata, links, traceability, and secret safety | FR-047–FR-052, FR-054, FR-058–FR-060; NFR-004, NFR-012, NFR-017, NFR-019 | Validation produces deterministic pass/fail output and reports seeded fixture failures |
| P5. Resumption and handoff | Work can pause, resume, and finish with compact state and acceptance information | FR-062–FR-067, FR-070, FR-077–FR-080; NFR-006, NFR-007 | A fresh-session exercise resumes from the documented state and a reviewer completes the handoff checklist |

## Explicitly Out of Scope for the Prototype

- [SCP-006](scope-items/SCP-006-hosted-orchestration-platform.md): hosted control plane, account system, or managed execution service.
- [SCP-007](scope-items/SCP-007-mandatory-paid-services.md): paid services required for core operation.
- [SCP-008](scope-items/SCP-008-production-platform-guarantees.md): production scale, uptime, compliance, or support guarantees.
- Real credentials, production data, external/public deployment, or production resources.
- Automatic merging, inferred approval, or destructive conflict resolution.
- Full compatibility claims across all operating systems, stacks, package managers, CI systems, and deployment targets.
- Material UX flows, significant architecture choices, or vendor selections that have not received their specific human approval.
- Documentation portal design or implementation, including MkDocs configuration, GitHub Pages, site information architecture, publication workflows, generated output, or new documentation-tooling dependencies.

## Deferred Product Requirements

Requirements not listed in the proposed slices remain valid product-backlog candidates but are not part of the first prototype unless GATE-003 explicitly adds them. In particular, broad multi-stack automation, optional Codex configuration, labels/milestones, larger-sprint optimisation, deployment artefact generation, completed example packs, version-release automation, and implementation of the human-friendly documentation portal are deferred. FR-081, FR-082, NFR-021, and NFR-022 record product intent and quality boundaries; they do not add portal implementation to the pending prototype scope.

## Dependencies and Constraints

| Type | Item | Consequence |
|---|---|---|
| Approval | GATE-001, GATE-002, and GATE-003 | Direction, brief, and scope have been approved; solution design may proceed; implementation may begin after design is recorded and remains subject to later gates for architecture, UX/product flows, external services, credentials, destructive actions, deployment, merge, and final acceptance |
| Decision | [OQ-002](open-questions/OQ-002-minimum-supported-stack-set.md) | The expanded Node/TypeScript, Python, Go, static-site, Docker, and unknown-stack fixture set is proposed; GATE-003 must confirm whether it is included |
| Decision | [OQ-003](open-questions/OQ-003-runtime-approval-recording.md) | GitHub issues and pull requests are the proposed primary approval records; approved solution design must validate durable linking and stale-state handling |
| Decision | [OQ-004](open-questions/OQ-004-factory-validation-automation-boundary.md) | The automated-check boundary is proposed; GATE-003 must confirm it before implementation planning |
| Decision | [OQ-006](open-questions/OQ-006-documentation-portal-implementation-approach.md) | MkDocs Material with GitHub Pages is preferred, but portal tooling, structure, publication controls, and implementation remain deferred to approved solution design |
| Research | [OQ-005](open-questions/OQ-005-representative-pilot-audience.md) | The target audience is selected, but value hypotheses remain unvalidated until 3–5 representative participants complete recorded pilots |
| Platform | Git and GitHub-compatible workflow | A non-GitHub operating model requires scope and options review |
| Safety | No secrets, paid services, production resources, deployment, merge, or destructive action without approval | The affected activity remains blocked and must be represented by a gate decision |

## Acceptance Boundary

GATE-003 has approved this scope. Approval makes the listed slices eligible for solution design and backlog preparation; implementation remains subject to later gates governing architecture, material UX/product flow, external services, credentials, deployment, destructive actions, merge, and final acceptance. Revisions to this scope require re-approval.

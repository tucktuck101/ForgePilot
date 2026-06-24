# DISC-009: Current and Target Workflows

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-009 |
| Document type | Workflow Analysis |
| Status | Draft; pending product-brief approval |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, operators, reviewers |
| Source | Problem statement, current state, target users, stories, requirements, and approval rules |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-003](stakeholder-needs/SN-003-repository-onboarding.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-008](stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-009](stakeholder-needs/SN-009-complete-prototype-handoff.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-003](evidence/EVD-003-repository-gap-observation.md) |
| Related objects | [Current State](current-state.md), [Approval Policy](approval-gates/operating-policy.md), [Scope](scope.md) |
| Update rule | Update when a handoff, exception, gate, or actor responsibility changes |

## Current Workflow and Pain Points

| Step | Actor | Current activity | Pain or failure mode |
|---|---|---|---|
| 1 | Product Owner | Communicates an idea and preferences in conversation | Intent may be vague, solution-led, or trapped in chat |
| 2 | Product Owner/Codex | Manually converts intent into artefacts | Completeness, priority, evidence, and traceability vary |
| 3 | Codex/reviewer | Locates context across Markdown files | Large or weakly indexed corpora increase reconstruction cost |
| 4 | Approval Authority | Reviews decisions when prompted | Approval triggers and durable records may be implicit |
| 5 | Delivery actors | Convert documents into work | Issues may lack business context or may be created before scope approval |
| 6 | Later session/reviewer | Reconstructs state and decisions | Context limits and missing handoff state cause rework |

## Target Workflow

| Stage | Responsible actor | Input | Output/handoff | Entry/exit control |
|---|---|---|---|---|
| 1. Repository intake | Repo Bootstrapper/Codex | Repository state and existing conventions | Intake findings, conflicts, constraints | Conflicting existing files require explicit approval before resolution |
| 2. Discovery | Codex with Product Owner | Vague idea, evidence, stakeholder answers | Problem, users, needs, value, risks, workflows, options, requirements, candidate scope | Facts, assumptions, recommendations, and open questions remain distinct |
| 3. Direction decision | Approval Authority | Options, evidence limits, risks, recommendation | GATE-001 approve/revise/reject record | Product direction remains provisional while pending |
| 4. Product-brief decision | Approval Authority | Complete discovery package and BA gate result | GATE-002 approve/revise/reject record | Solution design remains blocked while pending |
| 5. Prototype-scope decision | Approval Authority | Consolidated scope, dependencies, exclusions, traceability | GATE-003 approve/revise/reject record | Backlog execution and implementation remain blocked while pending |
| 6. Solution design | Codex with reviewer | Approved brief and scope | Options, decision records, acceptance design | Material UX, architecture, stack, or external-service choices use the relevant runtime gate |
| 7. Backlog handoff | Codex | Approved scope and sufficient design | Gated, traceable delivery issues | Issue is not executable unless prerequisite gates are approved |
| 8. Delivery and verification | Codex | One approved issue/sprint | Tested change, state updates, draft PR | Destructive actions, credentials, deployment, and merge require their gates |
| 9. Resume or handoff | Codex/reviewer | Current sprint state and evidence | Resume brief or final handoff | Final prototype acceptance remains a human decision |

## Exceptions and Failure Paths

| Trigger | Required response | Blocked until |
|---|---|---|
| Required context or evidence is missing | Record an assumption or open question; request focused input if necessary | The missing context is supplied or scope is revised to exclude it |
| Existing file conflicts with ForgePilot content | Preserve the file, document options and consequences, request conflict approval | A recorded approve/revise/reject decision exists |
| Product brief or prototype scope is revised | Update affected needs, requirements, scope, traceability, and issue drafts | The relevant gate is re-approved |
| Validation fails because of current work | Fix within approved scope and rerun validation | Required checks pass |
| Validation exposes unrelated failure | Record evidence and impact; do not conceal or broaden scope silently | Human direction is required only if it changes approved scope or risk |
| Token/context pressure threatens safe completion | Stop new work, update compact memory and resume brief | A later session resumes from the recorded state |
| Material UX, architecture, external service, credential, destructive, deployment, merge, or acceptance decision arises | Prepare a decision request under the approval policy | Human approval is durably recorded |
| Approval is rejected | Stop the dependent path and preserve the rejection rationale | A revised proposal receives approval or the work is closed |

## Operational and Maintainer Workflow

The ForgePilot Maintainer treats the reusable template as a product: assess change impact, update affected templates and examples separately from live truth, run factory validation, record version consequences, and request approval when a change alters product direction, compatibility, safety policy, or a hard-to-reverse repository convention.

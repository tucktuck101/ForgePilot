# DISC-006: Stakeholder Map

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-006 |
| Document type | Stakeholder Map |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | Linked target users, personas, stakeholder needs, and approval rules |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Target Users](target-users/index.md), [Personas](../personas/index.md), [Approval Policy](approval-gates/operating-policy.md) |
| Update rule | Update when accountability, consultation, or approval authority changes |

## Roles and Authority

| Stakeholder | Role in ForgePilot | Primary need | Decision authority | Participation |
|---|---|---|---|---|
| [TU-001 Solo Builder / Product Owner](target-users/TU-001-solo-builder-product-owner.md) | Problem owner and value owner | Rapid progress with low routine coordination | Accountable for problem framing, value, priorities, and proposed scope; may also act as approval authority | Leads discovery and reviews outcomes |
| [TU-002 Client / Approval Authority](target-users/TU-002-client-approval-authority.md) | Human control point | Safe, informed, reversible decisions | Sole authority for the material gates in the [approval operating policy](approval-gates/operating-policy.md) | Approves, requests revision, or rejects |
| [TU-003 Codex Delivery Agent](target-users/TU-003-codex-delivery-agent.md) | BA, planning, and delivery operator | Clear context and executable boundaries | May recommend and execute approved routine work; cannot approve its own work or infer approval | Responsible for artefacts, traceability, verification, and escalation |
| [TU-004 Technical Reviewer / Future Maintainer](target-users/TU-004-technical-reviewer-future-maintainer.md) | Independent reviewer and handoff recipient | Verifiable decisions and maintainable outputs | Consulted on material technical trade-offs; no default product approval authority | Reviews design, validation evidence, and handoff |
| [TU-005 Repo Bootstrapper](target-users/TU-005-repo-bootstrapper.md) | Installation and intake operator | Non-destructive onboarding | May perform reversible intake; conflicts require approval authority decision | Responsible for repository assessment and conflict reporting |
| [TU-006 ForgePilot Maintainer](target-users/TU-006-forgepilot-maintainer.md) | Template product operator | Controlled evolution and reuse | May recommend template changes; release, compatibility, or destructive changes require the relevant human gate | Maintains templates, validation, versioning, and examples |

## Accountability by Artefact

| Artefact or decision | Responsible | Accountable/approver | Consulted | Informed |
|---|---|---|---|---|
| Problem, current state, and needs | Codex | Product Owner | Target users | Reviewer, maintainer |
| Options and recommended direction | Codex | Approval Authority through GATE-001 | Product Owner, reviewer | Maintainer |
| Product brief | Codex | Approval Authority through GATE-002 | Product Owner, target users | Reviewer, maintainer |
| Prototype scope | Codex | Approval Authority through GATE-003 | Product Owner, reviewer, maintainer | Delivery actors |
| Material UX, architecture, external service, credential, conflict, destructive, deployment, merge, and acceptance decisions | Codex prepares decision request | Approval Authority | Relevant reviewer/operator | Affected stakeholders |
| Routine approved delivery and verification | Codex | Product Owner | Reviewer as needed | Approval Authority |

## Visible Trade-offs

| Tension | Stakeholders affected | Working rule |
|---|---|---|
| Autonomy versus human control | Product Owner, Approval Authority, Codex | Codex proceeds on reversible routine work and stops at the explicit material gates. |
| Breadth versus prototype focus | Product Owner, maintainer, reviewer | Product requirements may describe the intended product; only the pending [prototype scope](scope.md) controls the first build. |
| Context efficiency versus documentation completeness | Codex, reviewer, maintainer | Use compact indexes and atomic objects, with direct links instead of duplicated prose. |
| Portability versus implementation complexity | Bootstrapper, maintainer, Product Owner | Validate a bounded representative set first; broader compatibility remains deferred until supported by evidence and approval. |

## Evidence Limitation

The roles and authority model reflect recorded stakeholder intent, not external organisational research. If a real project separates product ownership, budget authority, security authority, or technical approval, the map must be revised before its gates are used.

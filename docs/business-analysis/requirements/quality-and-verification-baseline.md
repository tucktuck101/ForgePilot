# Requirements Quality and Verification Baseline

## Document Metadata

| Field | Value |
|---|---|
| Object ID | REQ-QA-001 |
| Document type | Requirements Quality Baseline |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, reviewers |
| Source | Live requirement objects, discovery traceability, and proposed prototype scope |
| Source need(s) | [SN-001](../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-005](../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md), [SN-007](../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md), [SN-008](../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-009](../discovery/stakeholder-needs/SN-009-complete-prototype-handoff.md), [SN-010](../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md), [SN-011](../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-003](../discovery/evidence/EVD-003-repository-gap-observation.md), [EVD-006](../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Requirements Index](index.md), [Traceability Matrix](../discovery/traceability-matrix.md), [Prototype Scope](../discovery/scope.md) |
| Update rule | Update when requirement quality, priority, verification, or prototype inclusion changes |

## Quality Rule

A live requirement is ready for controlled handoff only when it has one dominant obligation, a valid MoSCoW priority, a source need, evidence, an observable acceptance or verification method, and a trace to proposed or deferred scope. Product priority does not by itself include a requirement in the first prototype; [DISC-008](../discovery/scope.md) is the authoritative approved prototype boundary.

Business and functional requirement objects contain local acceptance criteria. User stories contain actor goals and local acceptance criteria. The following matrix supplies the explicit verification missing from the nonfunctional requirement objects without changing their intended product decisions.

## Nonfunctional Verification Matrix

| Requirement | Observable verification |
|---|---|
| NFR-001 Environment agnostic | On each approved pilot environment, required checks either run successfully or report a documented supported alternative; no undocumented OS, shell, or package-manager assumption blocks the workflow. |
| NFR-002 Chat-driven operation | A pilot completes discovery and approval requests through supported Codex chat/CLI interaction without requiring a separate product UI. |
| NFR-003 Balanced-to-aggressive autonomy | A pilot interaction log shows routine approved work proceeding without approval prompts and every material trigger stopping for approval. |
| NFR-004 Safe defaults | Default paths are reversible/local/free where feasible; paid, external, destructive, or irreversible choices remain blocked pending approval. |
| NFR-005 Approval-gated risk | Audit all triggered gates against the operating policy; target: zero material actions before a complete approval record. |
| NFR-006 Token efficiency | A fresh-session navigation test completes the assigned task from an issue, compact index, or summary and directly linked objects without loading the full documentation corpus or omitting required context. |
| NFR-007 Recoverability | A new session resumes a paused task from project memory and resume state without an undocumented mandatory reconstruction step. |
| NFR-008 Maintainability | Repository responsibilities are separated by documented location; a maintainer can identify where to change instructions, skills, artefacts, scripts, and release records. |
| NFR-009 Portability | Approved empty and existing-repository fixtures complete intake without destructive overwrite; unsupported platform assumptions are reported. |
| NFR-010 Multi-stack adaptability | Each stack in the GATE-003-approved pilot set is detected or safely classified unknown, with applicable commands or a documented escalation. |
| NFR-011 Open-source bias | Any proposed paid/proprietary dependency includes an open/local alternative analysis and remains pending until explicit approval. |
| NFR-012 Factory quality | Repeatable validation reports required-file, metadata, duplicate-ID, link, template/example, and unsafe-secret fixture failures. |
| NFR-013 Documentation quality | Formal artefacts pass agreed heading, metadata, status, link, summary, and human-readability checks; placeholder content is excluded from live truth. |
| NFR-014 Doc-object consistency | Every indexed live object contains its required metadata and collection-specific content; duplicate IDs, unindexed live objects, and inconsistent retrieval structures fail validation. |
| NFR-015 Decision traceability | Every live story and requirement resolves through a source need and evidence; scope and decisions identify the affected requirement set. |
| NFR-016 Delivery traceability | Each executable issue links approved scope and requirements; its PR, sprint state, tests, and handoff preserve the same chain. |
| NFR-017 Secrets safety | Secret-pattern checks pass; examples use placeholders; no real credential value is written to tracked docs or issue content. |
| NFR-018 Clear approval requests | Each sampled request contains decision, recommendation, alternatives, evidence gaps, risks, outcomes, blocked/permitted actions, and durable record location. |
| NFR-019 Repeatable validation | Two unchanged validation runs produce equivalent results; seeded failures identify the failing check and corrective context. |
| NFR-020 Versioned evolution | Each approved release-level template change updates the version and changelog with scope and rationale. |
| NFR-021 Documentation navigation and discoverability | A representative human and a fresh Codex session can each start from the relevant index or summary, locate a requested major artefact, identify its status, and follow links to authoritative detail without scanning the full corpus. |
| NFR-022 Documentation publication safety | Review a proposed publication manifest and generated output; target: the intended audience and content boundary are explicit, restricted information is absent, and any uncertain exposure remains blocked pending approval. |

## Consistency and Feasibility Rules

- `Must`, `Should`, and `Could` express product importance; prototype inclusion is separately controlled by DISC-008 and GATE-003.
- `Shall` or `must` denotes a mandatory outcome; `should` denotes a preferred outcome unless a linked constraint records an exception.
- Requirement acceptance may be demonstrated by inspection, automated validation, pilot observation, or a recorded approval decision.
- A requirement affected by an unresolved contradiction or infeasible dependency returns to Draft and blocks dependent handoff.
- Solution design may refine implementation acceptance detail, but may not silently change the need, priority, scope boundary, or human approval rule.

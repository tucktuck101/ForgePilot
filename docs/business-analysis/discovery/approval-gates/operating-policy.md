# Approval Gate Operating Policy

## Document Metadata

| Field | Value |
|---|---|
| Document type | Approval Policy |
| Status | Draft |
| Priority | Must |
| Owner/audience | Approval Authority, Product Owner, Codex, reviewers, maintainers |
| Source | Human approval rules and linked stakeholder needs |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-007](../stakeholder-needs/SN-007-secrets-and-security-safety.md), [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [GATE-001](GATE-001-options-and-direction-approval.md), [GATE-002](GATE-002-product-brief-approval.md), [GATE-003](GATE-003-prototype-scope-approval.md), [NFR-018](../../requirements/nonfunctional-requirements/NFR-018-clear-approval-requests.md), [NFR-022](../../requirements/nonfunctional-requirements/NFR-022-documentation-publication-safety.md) |
| Update rule | Update when a material approval trigger, authority, outcome, or recording rule changes |

## Authority and Outcomes

Only the human Approval Authority may grant a material approval. Codex may prepare a recommendation and execute work after approval, but must not infer approval from silence, document creation, prior approvals, or ambiguous chat.

Every gate supports exactly three outcomes:

- **Approve** — record the approver, date, decision reference, approved boundary, and next permitted activity.
- **Revise** — record requested changes; the dependent activity remains blocked until resubmission and approval.
- **Reject** — record rationale and consequence; the dependent path stops unless a materially revised proposal is submitted.

Missing approver, date, decision reference, or approved boundary means the gate is **Pending**.

## Gate Register

| Gate trigger | Status before trigger | Required decision input | Blocked activity while pending | Durable record |
|---|---|---|---|---|
| Options and product direction | Pending | Problem, users, evidence limits, alternatives, recommendation, risks | Treating a direction as final | [GATE-001](GATE-001-options-and-direction-approval.md) |
| Product brief | Pending | Complete brief, value model, workflows, risks, questions, BA gate result | Finalising the brief or starting solution design | [GATE-002](GATE-002-product-brief-approval.md) |
| Prototype scope | Pending | In/out/deferred scope, dependencies, requirement trace, acceptance boundary | Finalising scope, backlog execution, or implementation | [GATE-003](GATE-003-prototype-scope-approval.md) |
| Material UX or product flow | Not triggered | User impact, workflow options, evidence, prototype implications | Implementing the material flow | ADR/decision object plus approval reference |
| Significant architecture or technology stack | Not triggered | Constraints, alternatives, trade-offs, reversibility, cost | Committing to or implementing the significant choice | ADR plus approval reference |
| External/paid service, API, auth, analytics, AI provider, or hosted database | Not triggered | Purpose, alternatives, data/privacy/security/cost implications, exit path | Adding or configuring the service | ADR/decision object plus approval reference |
| Real credential, key, token, OAuth client, cloud account, or production resource | Not triggered | Exact resource, purpose, handling method, exposure and revocation plan | Accessing or using the real resource | Security/config decision record without secret values |
| Existing-repository conflict resolution | Not triggered | Conflicting files, preserve/merge/replace options, diff and reversibility | Overwriting, deleting, or materially changing the conflict | Intake/conflict decision record |
| Destructive or hard-to-reverse action | Not triggered | Exact action, impact, backup/recovery path, safer alternatives | Performing the action | Issue or decision record with approval reference |
| External or public prototype/application deployment | Not triggered | Target, cost, runtime exposure, data, rollback, validation | Deployment or public runtime exposure | Deployment decision record |
| Static documentation publication with restricted-information exposure | Not triggered | Intended audience, content boundary, information classification, generated-output review, withdrawal path | Publishing content that would expose, or may reasonably expose, restricted information | Documentation publication decision record |
| Pull-request merge | Not triggered | PR scope, checks, review state, known limitations | Merge | PR approval/merge record |
| Final prototype acceptance | Not triggered | Approved scope comparison, test evidence, limitations, handoff checklist | Treating the prototype as accepted or complete | Final acceptance decision |

## Documentation Publication Distinction

Publishing a static documentation presentation generated from repository Markdown is documentation publication, not prototype or application deployment. The deployment gate is therefore not triggered solely because documentation becomes externally accessible.

Documentation publication still requires an explicit approval record when the intended output would expose, or may reasonably expose, sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information. The approval decision must define the intended audience and content boundary. Selecting portal tooling, hosting, site structure, or workflows remains a separate solution-design decision and is not approved by this policy.

## Required Approval Request Content

Every material request must state:

1. the exact decision and why it is required now;
2. the recommendation and at least one credible alternative, including doing nothing where relevant;
3. evidence, assumptions, open questions, risks, cost, and reversibility;
4. the affected requirements, scope, issues, or decisions;
5. what becomes permitted and what remains blocked for each outcome;
6. where the durable decision will be recorded.

## Re-approval

A prior approval does not cover a material change to its boundary. Scope expansion, changed risk, new external dependency, changed data exposure, or a materially different option returns the affected gate to Pending until re-approved.

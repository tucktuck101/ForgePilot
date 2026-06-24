---
name: Gated delivery work
about: Create a traceable, resumable issue from approved scope
title: "[DELIVERY] "
labels: ""
assignees: ""
---

> Do not execute this issue until the necessary design and architecture approvals are granted. Drafting an issue does not grant approval.

## Goal

State one bounded outcome and the value or risk it addresses.

## Context and Linked Artefacts

- Approved product brief:
- Approved prototype scope item:
- Source need(s):
- Requirement(s):
- User story/stories:
- Design or decision record:

## Acceptance Criteria

- [ ] Add specific, observable completion conditions.

## Dependencies

- Prerequisite issues or decisions:
- Repository/environment assumptions:

## Risk Level

- Level: Low / Medium / High
- Risks and mitigations:

## Approval Gates

- GATE-002 product brief: Approved — decision reference: ChatGPT conversation approval instruction (2026-06-25).
- GATE-003 prototype scope: Approved — decision reference: ChatGPT conversation approval instruction (2026-06-25).
- Additional material gate triggers: material UX/product flow, significant architecture/stack decisions, external services/credentials/resources, conflict/destructive/deployment/merge, final prototype acceptance.
- Work that remains blocked: Implementation work that relies on unapproved design, architecture, stack, external service, or destructive actions remains blocked until the respective gate is approved.

## Test Expectations

- Automated checks:
- Manual or review checks:
- Failure/rollback expectations:

## Definition of Done

- [ ] Acceptance criteria are met.
- [ ] Required tests and validation pass, or unrelated failures are documented.
- [ ] Documentation, traceability, and current-state files are updated.
- [ ] No secret, unapproved service, destructive action, deployment, or merge was introduced.
- [ ] The work is resumable and the PR remains draft until ready for human review.

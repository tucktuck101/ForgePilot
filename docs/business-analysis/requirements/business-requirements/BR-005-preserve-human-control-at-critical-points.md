# BR-005: Preserve human control at critical points

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-005 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall require human approval at defined critical decision points.

## Details

The system must ensure that a human remains in control of important project decisions. Approval gates must exist for product brief approval, scope approval, material UX flows, significant architecture or stack decisions, use of external services, use of credentials and secrets, resolution of file conflicts in existing repositories, destructive/high-risk actions, deployment, merge of pull requests, and final acceptance. Codex should stop and request approval when any of these gates are reached.

## Acceptance Criteria

- Approval gates are defined and documented in the project brief and operating guidelines.
- Codex interrupts autonomous execution to request approval at each gate.
- The user can approve, revise, or reject decisions at each gate.

## Notes

This requirement ensures that control over product direction, risk, cost, and exposure remains with the user.

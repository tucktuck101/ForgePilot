# BR-005: Preserve human control at critical points

## Document Metadata

| Field | Value |
|---|---|
| Document type | Business Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index.md](index.md) |
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

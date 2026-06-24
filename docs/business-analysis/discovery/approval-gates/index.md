# Approval Gate Index

## Document Metadata

| Field | Value |
|---|---|
| Document type | Index |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | Objects indexed in this collection |
| Linked artefacts | [Discovery Index](../index.md), [Operating Policy](operating-policy.md), [Template](template.md) |
| Update rule | Update when an object is added, removed, renamed, or materially reclassified |

## Objects

| ID | Title | Classification | Priority | Status | Link |
|---|---|---|---|---|---|
| GATE-001 | Options and recommended direction approval | Product direction | Must | Approved | [GATE-001-options-and-direction-approval.md](GATE-001-options-and-direction-approval.md) |
| GATE-002 | Product brief approval | Pre-solution | Must | Approved | [GATE-002-product-brief-approval.md](GATE-002-product-brief-approval.md) |
| GATE-003 | Prototype scope approval | Pre-implementation | Must | Approved | [GATE-003-prototype-scope-approval.md](GATE-003-prototype-scope-approval.md) |

## Runtime Gate Policy

[operating-policy.md](operating-policy.md) defines the mandatory gate triggers for material UX/product flows, architecture or stack, external services, credentials, existing-repository conflicts, destructive actions, deployment, merge, and final acceptance. Those gates are `Not triggered` until their decision arises and become `Pending` before the dependent activity can proceed.

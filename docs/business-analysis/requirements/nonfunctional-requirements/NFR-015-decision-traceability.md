# NFR-015: Decision Traceability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-015 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

Material product and delivery decisions must be traceable from need and evidence through outcome and approval.

## Details

Traceability must connect stakeholder needs, evidence, target users, stories, business requirements, functional requirements, nonfunctional requirements, success criteria, options, risks, and approval decisions.

Significant solution decisions must additionally use ADRs or equivalent decision objects that record context, alternatives, consequences, and related links.

## Acceptance Criteria

- Every story and requirement links to at least one source need and evidence object.
- The discovery traceability matrix covers every live story and requirement.
- Options and approvals link to their supporting evidence, risks, and outcomes.
- Broken or generic-only traceability is treated as a quality failure.

## Notes

Conversation provenance may remain recorded, but it cannot be the only traceability information.

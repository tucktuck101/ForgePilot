# FR-017: Produce discovery artefacts

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-017 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [Index](index.md), [Discovery Index](../../discovery/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

ForgePilot shall produce a token-efficient, collection-based discovery knowledge base before solution design.

## Details

The discovery package must live under `docs/business-analysis/discovery/`. Singleton documents cover the product brief, problem statement, current state, traceability matrix, and BA quality assessment.

Every repeatable traceable entity must use an atomic collection containing `index.md`, `template.md`, and one file per object. Required collections are target users, stakeholder needs, evidence, prototype hypotheses, value hypotheses, success criteria, scope items, options, risks, assumptions, open questions, approval gates, definition-of-done items, and BA quality checks.

Existing persona, user-story, and requirement collections remain canonical and are linked rather than duplicated.

## Acceptance Criteria

- All required singleton documents exist under the discovery folder.
- Every required collection contains an index, template, and at least one live object.
- Indexes provide compact navigation and individual objects contain direct related-object links.
- The product brief, scope, options, hypotheses, evidence, outcomes, and approval state are mutually traceable.

## Notes

The collection model limits context retrieval by allowing Codex to load an index and only the related objects needed for the current decision.

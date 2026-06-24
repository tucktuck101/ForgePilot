# QLT-014: Documentation consumption readiness

## Document Metadata

| Field | Value |
|---|---|
| Object ID | QLT-014 |
| Document type | BA Quality Check |
| Status | Active |
| Priority | Must |
| Owner/audience | Product Owner, Codex, reviewers, maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [SC-009](../success-criteria/SC-009-human-readable-documentation-consumption.md), [SC-010](../success-criteria/SC-010-token-efficient-documentation-retrieval.md), [NFR-022](../../requirements/nonfunctional-requirements/NFR-022-documentation-publication-safety.md) |
| Update rule | Update when documentation-consumption or publication-readiness criteria change materially |

## Criterion

Documentation is ready for complementary Codex and human consumption when:

- collections and major artefacts are indexed and discoverable;
- related authoritative artefacts are connected by valid relative links;
- human-facing summaries provide orientation where needed;
- detailed objects are followed by link rather than duplicated;
- guidance reinforces selective retrieval instead of full-corpus ingestion by default; and
- any future publication is required to exclude sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information.

## Scoring

- **0 — Missing:** one or more required consumption or publication-safety conditions are absent or contradicted.
- **1 — Partial:** the dual-purpose model is present but navigation, summaries, selective retrieval, source authority, or publication safety is incomplete.
- **2 — Complete:** the criteria are explicit, indexed, traceable, internally consistent, and ready for their current BA decision.

## Failure Condition

This mandatory check fails readiness when scored 0. The assessment must cite supporting artefacts and must not infer portal implementation approval from a passing BA score.

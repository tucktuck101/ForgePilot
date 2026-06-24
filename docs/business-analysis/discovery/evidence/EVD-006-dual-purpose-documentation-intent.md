# EVD-006: Dual-purpose documentation intent

## Document Metadata

| Field | Value |
|---|---|
| Object ID | EVD-006 |
| Document type | Evidence |
| Status | Recorded |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | Direct stakeholder instruction received on 24 June 2026 |
| Source need(s) | [SN-008](../stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-005](../options/OPT-005-markdown-only-documentation-consumption.md), [OPT-006](../options/OPT-006-generated-documentation-portal.md), [OPT-007](../options/OPT-007-github-wiki-separate-documentation-store.md) |
| Update rule | Update when the stakeholder intent or its documented scope boundary changes materially |

## Summary

ForgePilot documentation is intended to serve Codex and human readers through the same repository Markdown source.

## Details

- For Codex, the documentation should operate as a granular, indexed, linked knowledge graph that supports selective retrieval from issues, indexes, and directly related artefacts.
- For users, reviewers, and maintainers, the same source should support a readable, navigable, searchable documentation experience.
- Repository Markdown remains the source of truth. Any future portal is a presentation and publication layer, not a separate knowledge store.
- MkDocs and GitHub Pages are candidate implementation mechanisms only. Selecting, designing, and implementing a portal is deferred to later approved solution-design and implementation work.
- Future static documentation publication is documentation publication rather than prototype or application deployment. Its primary risk is exposure of sensitive or restricted information.

## Reliability and Limitations

- Provenance: direct Product Owner instruction received on 24 June 2026.
- Confidence: high for stakeholder intent and the BA-only scope boundary.
- Limitation: this evidence does not approve a portal design, tooling choice, publication target, workflow, deployment, or implementation.
- Limitation: human usability and retrieval efficiency remain unvalidated until tested with representative users and Codex tasks.

# BR-007: Support broad software prototype types

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-007 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall support prototyping across a wide range of software types.

## Details

The system must not be limited to web applications. It should support mobile apps, desktop apps, APIs, backend services, command-line tools, workflow automations, AI agents, data tools, integrations, internal tools, and other software experiments. ForgePilot should detect the type of project during discovery and repo inspection and adapt its templates, scripts, and validations accordingly.

## Acceptance Criteria

- ForgePilot can be applied to repositories intending to build any of the supported prototype types.
- Discovery and solution design artefacts accommodate different project types.
- Scripts and validation adjust to the detected or specified project type.

## Notes

Broad prototype support makes ForgePilot versatile and applicable to diverse software ideas.

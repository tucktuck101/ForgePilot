# BR-007: Support broad software prototype types

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

ForgePilot shall support prototyping across a wide range of software types.

## Details

The system must not be limited to web applications. It should support mobile apps, desktop apps, APIs, backend services, command-line tools, workflow automations, AI agents, data tools, integrations, internal tools, and other software experiments. ForgePilot should detect the type of project during discovery and repo inspection and adapt its templates, scripts, and validations accordingly.

## Acceptance Criteria

- ForgePilot can be applied to repositories intending to build any of the supported prototype types.
- Discovery and solution design artefacts accommodate different project types.
- Scripts and validation adjust to the detected or specified project type.

## Notes

Broad prototype support makes ForgePilot versatile and applicable to diverse software ideas.

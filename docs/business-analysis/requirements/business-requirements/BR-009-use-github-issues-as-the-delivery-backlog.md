# BR-009: Use GitHub Issues as the delivery backlog

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

ForgePilot shall use GitHub Issues as the source of truth for executable delivery work.

## Details

All scoped work should be represented as GitHub Issues. Issues should contain the goal, context, linked artefacts, acceptance criteria, dependencies, risk level, approval gates, and test expectations. Issues should be linked to the relevant documentation and associated pull requests. While documentation remains in Markdown files, the Issues drive the actual delivery workflow and sprint execution.

## Acceptance Criteria

- Each scoped piece of work is represented by a GitHub Issue.
- Issues link to relevant briefs, designs, ADRs, and acceptance criteria.
- Issues are ordered by dependency and value.
- Codex uses Issues to drive sprint planning and PR creation.

## Notes

Using GitHub Issues integrates the delivery workflow with the repository, enabling traceability and collaboration.

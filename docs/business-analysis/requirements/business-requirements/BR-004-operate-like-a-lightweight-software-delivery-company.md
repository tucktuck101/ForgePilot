# BR-004: Operate like a lightweight software delivery company

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

ForgePilot shall model a lightweight client-agency software delivery process within a repository.

## Details

The system should behave like a small software delivery company compressed into a GitHub repository. It must support product discovery, scope definition, solution design, sprint planning, implementation, testing, documentation, deployment preparation, and final handoff. Each phase should include clear checkpoints and, where necessary, approval gates. Codex should handle routine tasks autonomously and present well-defined outputs and decisions for human approval at appropriate points.

## Acceptance Criteria

- The delivery process includes phases for discovery, brief approval, solution design, scoped sprints, verification, deployment preparation, and acceptance review.
- Each phase produces the expected artefacts (e.g., briefs, designs, backlog issues, sprint notes, test reports).
- Codex operates autonomously within phases, stopping at approval gates.
- The process is documented and repeatable.

## Notes

This requirement establishes the overarching delivery process that ForgePilot must implement.

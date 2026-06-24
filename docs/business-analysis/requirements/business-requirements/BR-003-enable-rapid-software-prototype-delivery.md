# BR-003: Enable rapid software prototype delivery

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-003 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall help the user move from a vague software idea to a working prototype with minimal manual intervention.

## Details

The system is intended to accelerate prototype delivery by automating discovery, design, implementation, testing, documentation, issue management, and deployment preparation through Codex. It should streamline the path from concept to prototype, allowing the user to focus on defining product direction while Codex handles the implementation details. This includes generating discovery artefacts, designing solutions, breaking work into sprints, implementing features, running validations, and preparing deployment.

## Acceptance Criteria

- Codex can guide the user through discovery and create a product brief and scope.
- Codex can autonomously design and implement scoped sprints based on approved requirements and solution design.
- Codex can manage GitHub Issues and pull requests without constant human intervention.
- The user can receive a working prototype ready for acceptance review with minimal manual effort.

## Notes

Rapid delivery is a core goal of ForgePilot, enabling experimentation and iteration on software ideas.

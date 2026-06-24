# US-037: Keep Examples Separate from Truth

## Document Metadata

| Field | Value |
|---|---|
| Document type | User Story |
| Status | Draft |
| Owner/audience | ForgePilot Maintainer, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [User Stories Index](index.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the ForgePilot Maintainer need to distinguish examples from live project artefacts.

## Story

As a ForgePilot Maintainer, I want example artefacts clearly separated from live project artefacts so that Codex does not confuse examples with the project's actual state.

## Acceptance Criteria

- Examples live under `examples/`.
- Examples are clearly marked.
- AGENTS.md and skills warn not to treat examples as project truth.
- Factory validation checks example markings where practical.

## Notes

None.

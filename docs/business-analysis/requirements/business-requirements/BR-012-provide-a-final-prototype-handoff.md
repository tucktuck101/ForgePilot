# BR-012: Provide a final prototype handoff

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

ForgePilot shall produce a final prototype handoff package for review, testing, deployment, or continuation.

## Details

Upon completion of a prototype, Codex must prepare a comprehensive handoff package. This package should include the working prototype status, setup and run instructions, test instructions and latest results, deployment instructions or approved staging URL, links to the product brief, approved scope, architecture/tech-stack summary, key ADRs, known limitations, security and privacy notes, future backlog items, and an acceptance checklist. The handoff package lives under `docs/delivery/final-handoff.md`.

## Acceptance Criteria

- A `final-handoff.md` document is generated at the end of a project.
- The handoff includes all required information and links.
- The user can review the handoff to make a final acceptance decision or request further work.

## Notes

This requirement ensures that prototypes are delivered in a state that can be understood, tested, deployed, and iterated upon by humans.

# NFR-010: Multi-Stack Adaptability

## Document Metadata

| Field | Value |
|---|---|
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Nonfunctional Requirements Index](../index.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must adapt to multiple technology stacks.

## Details

The system should detect common stack signals such as Node/TypeScript, Python, Go, Docker, static sites, and GitHub Actions. Based on detection, scripts and workflows should invoke appropriate commands (e.g., npm, pip, go) or call existing repo scripts. When the stack is unknown, the system should fall back to documented assumptions and conservative defaults, requesting user input or approval when necessary. This adaptability ensures that the template remains useful across a wide range of projects.

## Notes

Supporting multiple stacks increases the reach of ForgePilot but requires careful detection and handling of edge cases.

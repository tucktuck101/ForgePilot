# NFR-010: Multi-Stack Adaptability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-010 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must adapt to multiple technology stacks.

## Details

The system should detect common stack signals such as Node/TypeScript, Python, Go, Docker, static sites, and GitHub Actions. Based on detection, scripts and workflows should invoke appropriate commands (e.g., npm, pip, go) or call existing repo scripts. When the stack is unknown, the system should fall back to documented assumptions and conservative defaults, requesting user input or approval when necessary. This adaptability ensures that the template remains useful across a wide range of projects.

## Notes

Supporting multiple stacks increases the reach of ForgePilot but requires careful detection and handling of edge cases.

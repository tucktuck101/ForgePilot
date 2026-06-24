# NFR-006: Token Efficiency

## Document Metadata

| Field | Value |
|---|---|
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot shall minimise token usage.

## Details

The system must optimise for minimal context consumption. Codex should read only the necessary files, link to detailed artefacts instead of duplicating content, maintain a compact project memory, and update memory by overwriting stale facts rather than appending logs. The system should summarise decisions and avoid copying large content into notes. When token pressure is detected, it must pause gracefully and create a resume brief rather than failing abruptly.

## Notes

Reducing token usage improves reliability and efficiency, especially for long-running tasks that span multiple Codex sessions.

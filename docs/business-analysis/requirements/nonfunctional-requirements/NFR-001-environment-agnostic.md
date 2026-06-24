# NFR-001: Environment Agnostic

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

The system must be environment agnostic.

## Details

ForgePilot should operate across different development environments, including macOS, Linux, Windows, cloud environments, and Codespaces or devcontainers. It must avoid hard assumptions about the OS, shell, package manager, or deployment platform. Scripts and tooling should adapt to the host environment or provide cross-platform alternatives. When project-specific decisions require OS-specific handling, they should be isolated and documented.

## Notes

This requirement ensures portability and usability across different developer setups and CI environments.

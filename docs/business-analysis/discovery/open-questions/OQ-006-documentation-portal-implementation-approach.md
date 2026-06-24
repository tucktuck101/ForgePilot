# OQ-006: How should the human-friendly documentation portal be implemented?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-006 |
| Document type | Open Question |
| Status | Preferred proposal recorded; approvals pending |
| Priority | Should |
| Owner/audience | Product Owner, Approval Authority, Codex, maintainers |
| Source | ForgePilot business analysis conversation, Product Owner answer dated 2026-06-25, and linked evidence |
| Source need(s) | [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-006](../options/OPT-006-generated-documentation-portal.md), [RSK-007](../risks/RSK-007-documentation-publication-information-exposure.md), [Approval Gate Operating Policy](../approval-gates/operating-policy.md) |
| Update rule | Update when the later solution-design decision or its constraints change materially |

## Question

Which presentation, generation, hosting, navigation, search, and publication approach should provide the human-friendly documentation experience while preserving repository Markdown as the source of truth?

## Resolution

- Preferred proposal: Generate a MkDocs Material portal from the authoritative repository Markdown and publish it through GitHub Pages.
- Alternative considered: Docusaurus generated from the same Markdown source and published through GitHub Pages; not preferred because it introduces a larger Node-based documentation toolchain for the current need.
- Decision date: 2026-06-25.
- Decision reference: Product Owner selected option A in the Codex open-question working session dated 2026-06-25.

## Consequences and Approval Boundary

- Repository Markdown remains the sole authoritative source; generated site output must not become a separately maintained knowledge store.
- Approved solution design must define source mapping, information architecture, navigation, search, accessibility, generated-output handling, maintenance, cost, reversibility, and failure behaviour.
- GitHub Pages publication must include a reviewable content boundary and controls for sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information.
- Markdown-only repository browsing remains the fallback when generation or publication is unavailable.
- This is a preferred proposal, not architecture, dependency, publication, or implementation approval.
- Solution design and implementation remain blocked until GATE-002, applicable scope approval, any triggered architecture decision, and any required publication approval are recorded.

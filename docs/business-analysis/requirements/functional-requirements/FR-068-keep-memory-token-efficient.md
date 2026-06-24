# FR-068: Keep memory token-efficient

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-068 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall keep `project-memory.md` and other context files token-efficient by using bullet points, links, and minimal wording.

## Details

Because long context may impact performance and token limits, Codex should ensure that project memory and other context files remain concise and efficient. Project memory should target a length of approximately 1,000–1,500 words, use bullet points and lists instead of long paragraphs, and link to detailed documents instead of copying extensive content. Other context files, such as sprint notes and resume briefs, should also aim for brevity and clarity.

## Acceptance Criteria

- `project-memory.md` uses bullet points, short phrases, and structured sections instead of narrative text.
- The file stays within the target word count for memory efficiency.
- The file links to more detailed artefacts rather than duplicating content.
- Other context files maintain similar conciseness to avoid unnecessary token usage.

## Notes

Token-efficient context management helps Codex operate effectively within its context window while preserving essential project information.

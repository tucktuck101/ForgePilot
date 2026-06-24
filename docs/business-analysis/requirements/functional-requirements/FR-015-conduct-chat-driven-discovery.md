# FR-015: Conduct chat-driven discovery

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-015 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall have Codex conduct the initial discovery process through a chat-driven interview, using either the Codex CLI chat or the Codex chat window. This interactive interview collects essential information about the app idea.

## Details

During the discovery phase, Codex should:

- Ask the user focused questions one at a time (see FR-016).
- Use the chat interface to collect information about the product goal, users, problem statement, prototype hypothesis, scope, assumptions, constraints, and success criteria.
- Stop the interview when enough information is gathered to produce the product brief and prototype scope documents.
- Record the answers in the appropriate discovery artefacts under `docs/business-analysis`.

This interactive approach ensures that the user is neither overwhelmed nor left with an incomplete brief.

## Acceptance Criteria

- Discovery questions are delivered via chat.
- Codex collects responses and updates discovery documents accordingly.
- The interview stops once sufficient information is collected.
- The user is not asked unnecessary or repetitive questions.

## Notes

This requirement sets the stage for FR-016 (ask one question at a time) and FR-017 (produce discovery artefacts) to ensure a structured and user-friendly discovery process.

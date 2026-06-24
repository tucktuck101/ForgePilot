# FR-016: Ask one question at a time

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-016 |
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

During the discovery interview, Codex shall ask the user one focused question at a time instead of presenting multiple questions in a single prompt. This helps prevent cognitive overload and ensures the user can provide thoughtful answers.

## Details

- The discovery process should be broken into discrete questions covering the product goal, users, problem, hypothesis, scope, and acceptance criteria.
- Codex should wait for an answer before asking the next question.
- Each question should be clear, concise, and limited in scope.
- If a question leads to a dependency on previous answers, Codex should reference the relevant information to avoid repetition.

## Acceptance Criteria

- Users receive one question per message from Codex during discovery.
- Codex does not combine multiple topics into a single question.
- Responses are captured and used to formulate subsequent questions or documents.

## Notes

This requirement ensures user comfort and engagement while collecting sufficient information, supporting FR-015 (chat-driven discovery).

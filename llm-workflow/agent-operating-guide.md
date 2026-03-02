# Agent Operating Guide

This guide defines how to collaborate with an LLM agent during project planning and execution.

## Collaboration Model

- LLM drafts, decomposes, and proposes.
- Human reviews, decides, and approves.
- Both maintain traceability and documentation quality.

## Session Start Protocol

At the beginning of a session, provide:

1. objective for this session
2. relevant artifact links (PRD/ADR/tasks)
3. constraints (time, risk, architecture, dependencies)
4. expected output format

## Operating Rules

- Never implement without source artifact context.
- Keep IDs and section headers stable.
- Write requirements and acceptance criteria in EARS format only.
- Flag assumptions explicitly.
- If information is missing, ask concise critical questions before drafting.

## Required Outputs by Activity

- **Draft PRD section** -> include assumptions, risks, and EARS-formatted measurable criteria.
- **Draft ADR** -> include alternatives and consequences.
- **Task decomposition** -> one task per outcome slice, each with EARS-formatted acceptance criteria.
- **Review** -> findings first, severity ordered, then suggestions.

## Quality Gates

Before accepting any AI-generated artifact:

- [ ] Structure matches canonical template.
- [ ] Source links and IDs are present.
- [ ] Requirements/acceptance criteria are EARS-compliant and testable.
- [ ] Risks and tradeoffs are explicit.
- [ ] Out-of-scope boundaries are clear.

## Escalation Rules

Escalate to human decision when:

- tradeoff affects architecture direction
- requirement is ambiguous and impacts scope
- risk is high and mitigation is uncertain

## Anti-Patterns

- generating long prose without EARS-formatted acceptance criteria
- closing tasks without feedback to PRD/ADR
- introducing new terminology without convention updates
- mixing multiple unrelated decisions into one ADR

# Prompt Recipes

Use these prompts as reusable starting points for common planning operations.

## 1) Draft a PRD

```text
Create a first draft PRD using templates/prd-template.md.
Context:
- Project:
- Problem:
- Target users:
- Constraints:
- Non-goals:

Requirements:
- Keep canonical headings and metadata.
- Define EARS-formatted, measurable acceptance criteria for each core feature (use `R1`, `R2`, ...).
- Add out-of-scope and explicit risks.
- Propose success metrics with measurable targets.
```

## 2) Create ADR Options

```text
Draft ADR-XX using templates/adr-template.md for this decision:
<decision topic>

Context:
- Relevant PRD features:
- Constraints:
- Current architecture:

Requirements:
- Propose at least 2 alternatives plus selected option.
- Include explicit tradeoffs and risks.
- Any requirement statements included must be EARS-formatted with explicit system/component and `shall`.
- Include migration/rollout considerations.
```

## 3) Decompose Feature into Tasks

```text
Break PRD-XX feature F-YY into executable tasks using templates/task-template.md.

Requirements:
- Tasks should be independently testable.
- Include source links and dependencies.
- Keep each task small enough for one focused implementation cycle.
- Write all task acceptance criteria in EARS format only (`R1`, `R2`, ...).
- Include ADR/PRD update checklist items per task.
```

## 4) Scope-Slice for MVP

```text
From PRD-XX, propose an MVP slice that minimizes risk and time-to-value.

Requirements:
- Mark included vs excluded feature slices.
- State tradeoffs and deferred risks.
- Produce a prioritized task order.
```

## 5) Planning Review

```text
Review these artifacts for execution readiness:
- <artifact paths>

Review mode:
- findings first (ordered by severity)
- identify non-EARS requirements, missing acceptance criteria, broken traceability, and unresolved assumptions
- propose concrete fixes
```

## 6) Session Handoff Draft

```text
Generate a handoff summary using llm-workflow/handoff-template.md.

Include:
- completed work
- current state
- open decisions
- next recommended action list
- links to modified artifacts
```

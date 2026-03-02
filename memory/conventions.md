# Project Conventions

Use this file to maintain shared vocabulary and standards for the project.

## Naming and IDs

- PRD IDs: `PRD-01`, `PRD-02`, ...
- ADR IDs: `ADR-01`, `ADR-02`, ...
- Task IDs: `TASK-01`, `TASK-02`, ...
- Feature IDs in PRD: `F-01`, `F-02`, ...

## Status Vocabularies

- PRD status: `draft`, `review`, `approved`, `superseded`
- ADR status: `proposed`, `accepted`, `rejected`, `deprecated`, `superseded`
- Task state: folder lifecycle (`todo`, `in-progress`, `done`)

## Documentation Conventions

- Dates: `YYYY-MM-DD`
- Keep canonical section names from templates.
- Prefer links to source artifacts over plain-text references.
- Keep requirements and acceptance criteria EARS-formatted, observable, and testable.

## EARS Requirement Standard

Use EARS as the default for all requirements and acceptance criteria.

- IDs: `R1`, `R2`, ...
- One requirement per line/bullet.
- Always include explicit `<system>` and modal verb `shall`.
- Write behavior outcomes and invariants, not implementation tasks.

Canonical EARS patterns:

- Ubiquitous: `The <system> shall <response>.`
- State-driven: `While <precondition(s)>, the <system> shall <response>.`
- Event-driven: `When <trigger>, the <system> shall <response>.`
- Optional feature: `Where <feature/scope applies>, the <system> shall <response>.`
- Unwanted behavior: `If <unwanted condition>, then the <system> shall <mitigation>.`
- Complex: `While <precondition(s)>, when <trigger>, the <system> shall <response>.`

## Domain Terminology

Fill this table with project-specific terms early.

| Term | Meaning | Notes |
|---|---|---|
| ExampleTerm | Short definition | Optional context |

## Engineering Standards (Optional Seed)

- Branch naming:
- Commit style:
- Testing expectations:
- Release process:

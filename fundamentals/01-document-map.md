# Document Map

This file explains which artifact to create, when to create it, and how artifacts connect.

## Artifact Types

| Artifact | Purpose | Primary Owner | Update Frequency |
|---|---|---|---|
| Fundamentals | Defines planning rules, terminology, and system constraints | Tech/Product Lead | Low |
| PRD | Defines product scope, outcomes, and acceptance at feature level | Product + Engineering | Medium |
| ADR | Captures architecture-level decisions and tradeoffs | Engineering | Medium |
| Task | Defines executable units of work | Engineering | High |
| Memory | Captures learnings, conventions, and pitfalls | All contributors | High |

## Suggested Creation Order

1. **Fundamentals**: establish principles and vocabulary.
2. **PRD**: define outcomes, features, and boundaries.
3. **ADR**: define key implementation decisions.
4. **Tasks**: decompose work into execution units.
5. **Memory**: continuously capture execution learnings.

## Decision Tree: Which Document Do I Need?

- Need to define **what** should be built and why? -> PRD
- Need to decide **how** to build something with tradeoffs? -> ADR
- Need a concrete implementation unit? -> Task
- Learned something reusable or hit a recurring pitfall? -> Memory
- Need to update common vocabulary or long-lived rules? -> Fundamentals/Conventions

## Required Cross-Links

- PRD should link related fundamentals and ADRs.
- ADR should link related PRD features and relevant fundamentals.
- Task should cite source PRD/ADR IDs in frontmatter.
- Memory entry should cite source task and optionally PRD/ADR.

## Required Metadata Conventions

- IDs are mandatory and stable once assigned.
- Status values should use a fixed vocabulary:
  - PRD: `draft`, `review`, `approved`, `superseded`
  - ADR: `proposed`, `accepted`, `rejected`, `deprecated`, `superseded`
  - Task: lifecycle by folder plus optional `status` in frontmatter
- Dates use `YYYY-MM-DD`.

## Minimal Working Set for New Projects

At minimum, create:

- one PRD
- one or more ADRs for key architectural choices
- a seeded `tasks/todo/` backlog with EARS-formatted, measurable, testable acceptance criteria
- initialized memory files (`conventions`, `learnings`, `gotchas`)

This minimal set is enough for an LLM or human contributor to start executing safely.

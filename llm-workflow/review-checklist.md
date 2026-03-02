# Planning Review Checklist

Use this checklist to validate artifacts before execution begins.

## A) PRD Quality

- [ ] Problem statement is clear and bounded.
- [ ] Personas are concrete enough to guide decisions.
- [ ] Feature list has EARS-formatted, measurable, testable acceptance criteria.
- [ ] Out-of-scope is explicit.
- [ ] Success metrics are measurable and relevant.

## B) ADR Quality

- [ ] Decision is explicit and unambiguous.
- [ ] At least one alternative is documented.
- [ ] Consequences include positives, negatives, and risks.
- [ ] Impacted PRD features are linked.
- [ ] Status is correct and current.

## C) Task Quality

- [ ] Task references source PRD/ADR IDs.
- [ ] Scope is small and executable.
- [ ] Acceptance criteria are EARS-compliant and testable.
- [ ] Verification steps are specified.
- [ ] ADR/PRD update checklist is included.

## D) Traceability Integrity

- [ ] All active tasks map to PRD/ADR sources.
- [ ] PRD features map to planned or completed tasks.
- [ ] Decision changes are reflected in ADR statuses.
- [ ] Memory includes recent learnings/gotchas from completed work.

## E) LLM Collaboration Readiness

- [ ] Terminology is normalized in `memory/conventions.md`.
- [ ] Assumptions are explicit and flagged.
- [ ] Open questions are converted to decisions/tasks.
- [ ] Artifacts use canonical headings for reliable parsing.
- [ ] EARS wording patterns are used consistently (`shall`, explicit system/component, correct pattern type).

## Execution Readiness Decision

- **Ready** if all critical checks pass.
- **Conditionally ready** if only low-severity issues remain with owners assigned.
- **Not ready** if traceability, acceptance criteria, or decision quality is missing.

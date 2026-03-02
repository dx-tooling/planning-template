# PRD-XX: <Short Product Initiative Name>

**Version:** 0.1  
**Date:** YYYY-MM-DD  
**Status:** draft | review | approved | superseded  
**Owners:** <names/roles>

## Overview

Describe the problem, the opportunity, and the intended outcome in 1-3 short paragraphs.

## Key Principles

- Principle 1
- Principle 2
- Principle 3

## User Personas

### Persona A
- Context:
- Needs:
- Success definition:

### Persona B
- Context:
- Needs:
- Success definition:

## Core Features

### F-01: <Feature Name>

What this feature does and why it matters.

**Acceptance Criteria:**
- [ ] R1: When <trigger>, the <system> shall <response>.
- [ ] R2: While <state>, the <system> shall <response>.
- [ ] R3: If <unwanted condition>, then the <system> shall <mitigation>.

### F-02: <Feature Name>

What this feature does and why it matters.

**Acceptance Criteria:**
- [ ] R1: The <system> shall <response>.
- [ ] R2: Where <feature/scope applies>, the <system> shall <response>.

## Non-Functional Requirements

Write these as EARS requirements and keep IDs stable.

- R1 (Performance): While <load/state>, the <system> shall <response>.
- R2 (Reliability): If <failure condition>, then the <system> shall <mitigation>.
- R3 (Security/Privacy): When <security trigger>, the <system> shall <response>.
- R4 (Observability): When <operational trigger>, the <system> shall <response>.

## Out of Scope

- Item 1
- Item 2

## Assumptions and Open Questions

- Assumption:
- Open question:

Convert unresolved open questions into ADRs or tasks before implementation.

## Success Metrics

| Metric | Target | Measurement Method |
|---|---|---|
| Example metric | Target value | How measured |

## Dependencies

- Internal dependency:
- External dependency:

## Risks

- Risk:
  - Impact:
  - Mitigation:

## Related Documents

- [../fundamentals/00-planning-principles.md](../fundamentals/00-planning-principles.md)
- [../fundamentals/02-traceability-model.md](../fundamentals/02-traceability-model.md)
- [../architectural-decision-records/ADR-XX-example.md](../architectural-decision-records/ADR-XX-example.md)

---

## Notes for Template Users

- Keep feature IDs stable (`F-01`, `F-02`, ...).
- Acceptance criteria should be EARS-formatted, measurable, and testable by an independent reviewer.
- If scope changes materially, bump version and summarize change rationale.

# Gotchas

Capture pitfalls and failure modes so they are not repeated.

### Example: Missing Source Links Break Traceability (YYYY-MM-DD)

What happened: A completed task did not include PRD/ADR source references.  
Why it matters: Reviewers could not verify whether implementation matched intent.  
How to apply/avoid: Make `source` mandatory and block completion without it.  
Source: TASK-XX

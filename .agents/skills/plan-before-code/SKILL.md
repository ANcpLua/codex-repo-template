---
name: plan-before-code
description: Use for any new feature, refactor, repository structure change, multi-file edit, or UI change. Produce the plan before code.
---

# plan-before-code

Before touching code, write:

1. current state
2. target state
3. delta
4. exact files to touch
5. acceptance criteria

## Rules

- No fallback designs.
- No optional branches.
- No "we can improve this later" placeholders.
- State what will be deleted, not just what will be added.
- If frontend work is involved, use `frontend-direction` before code.

## Output

```md
## Current state

## Target state

## Delta

## Files

## Acceptance criteria
```

If the user explicitly asked for implementation in the same turn, produce the plan first and then continue into implementation.

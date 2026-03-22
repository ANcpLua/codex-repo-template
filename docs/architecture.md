# Architecture

## Problem

Most agent repositories mix product nouns, transport nouns, and compatibility nouns at the root. That makes growth easy in the short term and confusing in the long term.

## This template

- `AGENTS.md` is the repository-wide contract loaded before work.
- `.agents/skills/` holds progressive-disclosure instructions.
- `.codex/agents/` holds project-scoped custom subagents.
- `tests/` holds prompt contracts grouped by primitive.

## Rejected shapes

- root `skills/`
- root `agents/`
- `hooks/` for a Codex-only repository
- mirrored platform folders
- harness-first test layout
- fallback instructions in multiple places

## Scaling rule

New capability means one of three things:

1. a new skill
2. a new agent
3. a new prompt contract

If it needs a new root category, the design is probably wrong.

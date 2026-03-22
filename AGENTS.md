# AGENTS.md

## Purpose

This repository is a Codex-only repository template.

It exists to keep Codex behavior predictable, composable, and low-noise by using only official Codex extension points:

- `AGENTS.md`
- `.agents/skills/`
- `.codex/agents/`

## Hard boundaries

- Codex only. Do not add Claude, Cursor, Gemini, OpenCode, or generic multi-platform directories.
- Repository instructions live only in `AGENTS.md`.
- Skills live only in `.agents/skills/<skill>/SKILL.md`.
- Custom agents live only in `.codex/agents/<agent>.toml`.
- Documentation lives only in `README.md` and `docs/architecture.md`.
- Tests live only in `tests/`, grouped by product primitive first.
- Do not add `hooks/`, `plugins/`, `commands/`, or alternate skill locations.
- Do not add fallbacks, shims, compatibility layers, mirrored docs, or optional directory splits.

## Workflow

1. Read `AGENTS.md`.
2. Check for a relevant repo skill.
3. For feature work, use `plan-before-code` before editing.
4. For frontend work, use `frontend-direction` before writing UI code.
5. Use custom agents only for bounded plan review or code review.

## Repository invariants

- Every skill does exactly one job.
- Every agent has one reason to exist.
- Every directory name must be a product noun, not a transport noun.
- New capabilities extend existing axes. They do not invent new root categories.
- If a new file does not fit the tree, the tree is wrong or the file should not exist.

## Naming

- Prefer literal names over clever names.
- Prefer verbs for skills.
- Prefer roles for agents.

## Frontend bias

Frontend work must declare:

1. visual thesis
2. content plan
3. interaction thesis

before code.

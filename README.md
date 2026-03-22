# codex-repo-template

Codex-only repository template.

This template encodes three official Codex control surfaces:

- `AGENTS.md` for repository instructions loaded before work
- `.agents/skills/` for progressive-disclosure skills
- `.codex/agents/` for project-scoped custom agents

## Structure

```text
AGENTS.md
.agents/skills/
.codex/agents/
.codex/config.toml
docs/architecture.md
tests/
```

## Included primitives

- `plan-before-code`: forces current state, target state, delta, and exact files before code
- `frontend-direction`: forces art direction before frontend code
- `plan-reviewer`: rejects vague or branchy plans
- `code-reviewer`: reviews correctness, drift, and regression risk

## Non-goals

- multi-platform plugin support
- hooks as instruction injection
- duplicate root `skills/` or `agents/` folders
- verbose process documentation

## Sources

- https://developers.openai.com/codex/skills
- https://developers.openai.com/codex/subagents

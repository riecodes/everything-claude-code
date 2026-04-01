---
name: add-new-skill-or-agent
description: Workflow command scaffold for add-new-skill-or-agent in everything-claude-code.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-new-skill-or-agent

Use this workflow when working on **add-new-skill-or-agent** in `everything-claude-code`.

## Goal

Adds a new skill or agent to the codebase, including documentation and configuration.

## Common Files

- `skills/*/SKILL.md`
- `.agents/skills/*/SKILL.md`
- `agents/*.md`
- `.codex/agents/*.toml`
- `AGENTS.md`
- `.opencode/opencode.json`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Create a new SKILL.md file under skills/<skill-name>/ or .agents/skills/<agent-name>/
- Optionally add supporting agent definition files (e.g., agents/<agent-name>.md or .codex/agents/<agent-name>.toml)
- Update or create related documentation or configuration files (e.g., AGENTS.md, opencode.json)

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.
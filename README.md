# ai-skills

A personal collection of Agent Skills. Folders of instructions that teach LLM agents how to do a specific task the way I want it done.

## What's in here

| Skill | What it does |
| --- | --- |
| `detolstify` | Compress a document, note, or session artifact down to what a reader actually needs |

## Layout

Each skill lives in its own folder under `skills/`:

    skills/<skill-name>/
    ├── SKILL.md      # required: YAML frontmatter + instructions
    ├── scripts/      # optional: executable helpers
    ├── references/   # optional: docs loaded on demand
    └── assets/       # optional: templates, fonts, icons

`SKILL.md` starts with frontmatter containing `name` and `description`. The
description is what determines whether the skill gets picked up, so it should
say both what the skill does and when to reach for it.

## Using a skill

- **Claude Code / Cowork / Codex:** copy or symlink the skill folder into `~/.claude(or .codex)/skills/`
  for personal use, or `.claude(or .codex)/skills/` inside a project.
- **Claude.ai:** upload the skill from Settings → Capabilities → Skills.

## Adding a skill

1. `mkdir -p skills/<skill-name>`
2. Write `SKILL.md` with frontmatter and instructions.
3. Add a row to the table above.

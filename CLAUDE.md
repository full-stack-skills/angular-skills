# CLAUDE.md

## Project Overview

Angular Skills — a curated Agent Skills package for AI coding agents, part of the [Full Stack Skills](https://github.com/partme-ai/full-stack-skills) ecosystem maintained by PartMe.AI. Each skill is a self-contained `SKILL.md` file that AI agents load on-demand.

- **Language**: Markdown + YAML frontmatter (skills), JSON (plugin manifest)
- **License**: Apache 2.0
- **Install**: `npx skills add full-stack-skills/angular-skills`

## Skills (1)

| Skill | Directory | Description |
|-------|-----------|-------------|
| `angular` | `skills/angular/` | Angular framework: components, modules, DI, routing, forms, RxJS, CLI |

## Directory Structure

```
angular-skills/
├── .claude-plugin/plugin.json   # Claude Code discovery manifest
├── README.md / README.zh-CN.md  # Bilingual user-facing docs
├── AGENTS.md / AGENTS_EN.md     # Skill authoring guide (zh/en)
├── LICENSE                       # Apache 2.0
└── skills/
    └── angular/
        ├── SKILL.md              # Skill definition (YAML frontmatter + Markdown)
        └── LICENSE.txt           # Skill-level license
```

## SKILL.md Format

Every skill file has YAML frontmatter (`name`, `description`, optional `license`) followed by Markdown body:

```yaml
---
name: angular
description: One sentence. Include trigger phrases. Used by agents for relevance matching.
---
```

Body sections: When to use, How to use (numbered steps), Best Practices, Keywords.

## Skill Authoring Conventions

- **Directory naming**: `skills/<group>/<skill-name>/` where `<skill-name>` is `kebab-case`, matching the `name` field in frontmatter
- **SKILL.md filename**: Always uppercase, always exactly `SKILL.md`
- **Keep SKILL.md under 500 lines** — put detailed references in separate files
- **Progressive disclosure**: reference supporting files (`examples/`, `references/`, `scripts/`) that get read only when needed
- **Description specificity**: helps agents accurately decide when to load the skill
- **Scripts**: `#!/bin/bash` with `set -e`, status to stderr, data to stdout
- **Zip packaging**: `cd skills && zip -r <skill-name>.zip <skill-name>/`

## Key Docs

- `README.md` / `README.zh-CN.md` — user-facing install and skill listing
- `AGENTS.md` / `AGENTS_EN.md` — complete skill authoring guide for AI agents (500-line limit, context efficiency, script requirements, installation methods)
- `.claude-plugin/plugin.json` — name, version, skills array for Claude Code discovery

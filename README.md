# Top 20 Claude skills for software engineering

A weekly curated list. Software engineering only, no fluff.

Last updated: 2026-10-31 (v2)
Next curation: Saturday 2026-11-07, around 9am PT
Rule: always 20. One in, one out. Dropped skills move to archive, never deleted.

Browse it as a simple site: https://aiships.github.io/engineering-claude-skills/

This is an index, not a copy. Each entry links to its source repo. Read the source README and license before you install anything. Star counts below are from Oct 27-31 and change daily. Treat them as a popularity signal, not proof of quality.

## How to use this list

1. Start with one workflow framework from 1-6, not all six.
2. Add the official Anthropic skills you actually need from 7-12.
3. Add one skill per real pain point after that: UI, understanding code, context, tokens.
4. Install only what you will use. Every enabled skill costs context.

Install patterns (check the source repo first, commands change):

```bash
# Anthropic official marketplace
/plugin marketplace add anthropics/skills
/plugin install example-skills@anthropic-agent-skills
/plugin install document-skills@anthropic-agent-skills

# Most community skills: copy the skill folder, or use the repo's installer
# Global (all projects):
cp -r <skill-folder> ~/.claude/skills/
# Project only:
cp -r <skill-folder> .claude/skills/
```

## The Top 20

### Workflow and methodology

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 1 | Superpowers | [obra/superpowers](https://github.com/obra/superpowers), about 306k stars, checked Oct 28 on GitHub | Plan first, test-driven development, systematic debugging, subagent-driven work, verify before finishing | You want Claude Code to act like a disciplined senior engineer instead of jumping straight to code |
| 2 | Matt Pocock Skills | [mattpocock/skills](https://github.com/mattpocock/skills) | Small composable skills for real engineering work | You want bite-size skills you can adopt one at a time |
| 3 | Addy Osmani Agent Skills | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills), about 101k stars | Production-grade spec, build, test, ship workflows | You want a shipping workflow, not just a coding helper |
| 4 | gstack | [garrytan/gstack](https://github.com/garrytan/gstack), about 138k stars, checked Oct 31 on GitHub | Team-in-a-box process: slash-command roles for design, eng management, review, QA, security, and release | You want a full engineering-team process around your agent, not just a coding helper |
| 5 | BMAD-METHOD | [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) | Agile AI-driven development method | You want an agile, role-based method for bigger builds |
| 6 | Planning with Files | [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Breaks tasks into steps and tracks progress in files | Any coding task longer than a few minutes, where Claude loses track |

### Official Anthropic, software engineering only

Source: [anthropics/skills](https://github.com/anthropics/skills), about 184k stars, 19 skill folders, checked Oct 31 on GitHub. Only the engineering ones made the Top 20. Document, brand, art, and comms skills are in archive.

| # | Skill | What it does | When to use it |
|---|---|---|---|
| 7 | skill-creator | A skill that writes skills, following Anthropic's own authoring practice | Every time you catch yourself explaining the same procedure twice |
| 8 | mcp-builder | Guide for building good MCP servers | You need Claude to reach an API, database, or outside service |
| 9 | claude-api | Reference for the Claude API and SDKs: model ids, pricing, params, streaming, tool use, caching | You build with the Claude API and want current facts, not the model's memory |
| 10 | frontend-design | Distinctive, production-grade UI direction | You build web interfaces and want to avoid generic-looking pages |
| 11 | artifacts-builder | Build complex HTML artifacts with React, Tailwind, shadcn | You build interactive artifacts or web apps in Claude |
| 12 | webapp-testing | Test local web apps with Playwright for UI checks and debugging | You need browser-driven QA before shipping a web app |

### Frontend and UI

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 13 | UI-UX Pro Max | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Design intelligence: styles, palettes, UX rules | Your UI looks AI-made and you want a real design system |
| 14 | Impeccable | [pbakaus/impeccable](https://github.com/pbakaus/impeccable), about 98k stars, checked Oct 31 on GitHub | Design vocabulary for agents: polish, critique, audit commands plus 62 deterministic anti-slop detector rules | Your agent-built UI looks generic and you want concrete, checkable design feedback |

Honest caveat: independent blind tests in Oct 2026 ranked UI-UX Pro Max first on one test, and impeccable is this week's fastest riser, with deterministic detectors instead of LLM judgment. Some design skills burn a lot of tokens. Use one design skill at a time and judge on your own brief.

### Understanding, docs, context

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 15 | Understand-Anything | Search "Understand-Anything" on GitHub, see note below | Turns a codebase into an interactive knowledge graph you can explore and ask about | You are onboarding to an unfamiliar codebase |
| 16 | Context7 | [upstash/context7](https://github.com/upstash/context7) | Keeps current library docs in front of the model | Claude keeps using outdated library APIs |
| 17 | Claude-Mem | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | Persistent memory across sessions | Claude forgets your project between sessions |
| 18 | Diagram Design | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design), about 53k stars | Architecture, flow, org, and timeline diagrams, 44 types, exports to HTML, SVG, PNG | You need clean architecture diagrams from a codebase or a brief |

### Efficiency and harness

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 19 | Caveman | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Cuts output tokens hard while keeping technical accuracy | You are hitting usage limits and want shorter output |
| 20 | ECC | Search "ECC" or "affaan-m/ecc" on GitHub, see note below | Agent harness tuning: skills, memory, security, research-first workflow | You want one harness setup across Claude Code, Codex, Cursor, and similar tools |

Check the exact owner and repo for 15 and 20 before installing. These names have many mirrors. Do not install a fork without reading it.

## Watchlist for next Saturday

Did not make v2. First in line if a Top 20 slot opens:

- Hallmark (Nutlope/hallmark): anti-slop design with 50 themes and a browser lint, alternative to 13
- GitNexus: client-side knowledge graph with built-in RAG, alternative to 15
- Context Engineering / Context Mode: token and context optimization, alternative to 19
- open-gsd/gsd-core: the official successor to the archived GSD, install with npx @opengsd/gsd-core
- driving-seat (Tanmay-Ts/driving-seat): human decision gates before irreversible actions, new and unproven
- Pristine: UI critique skill, no verified repo yet
- playwright-cli skill: browser QA through an npm package, overlaps 12
- MCode Stack (MiniMax-AI/mcode-stack): harness engineering skills from the MiniMax Code team, MIT, 476 stars, 3 days old, no published evals. Standouts: independent-review, long-command-check, subagent-split-check

## Left out on purpose

See archive/ARCHIVED.md. Short version: algorithmic-art, canvas-design, brand-guidelines, internal-comms, slack-gif-creator, theme-factory, docx, pdf, pptx, xlsx. Real Anthropic skills, just not software engineering.

## Curation rules

Full rules in CURATION.md. Short version:

- Software engineering only.
- Maintained: a commit or release in the last 90 days, or an official Anthropic source that is still current.
- Installable and tested on a real task, not just starred.
- Stars help, they do not decide.
- Max 20. One in, one out. Archive, do not delete.
- Updated every Saturday morning, around 9am PT.
- Written like a human wrote it. Keyboard characters only, no AI-style symbols.

## License and attribution

This repo is a curated index with links. Each skill keeps its own license and owner. Do not copy a skill's files here without checking its license.

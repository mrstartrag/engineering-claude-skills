# Top 20 Claude Skills for Software Engineering

A weekly-curated list. Software engineering only. No fluff.

**Last curated:** 2026-10-27 (v1)
**Next curation:** Saturday 2026-10-31, ~9:00 AM PT
**Rule:** Always 20. One in, one out. Dropped skills move to `archive/`, they are never deleted.

This repo is a curated index, not a copy of the skills. Each entry links to its source repo. Read the source README and license before installing. Star counts below are as of 2026-10-27 / 2026-10-28 and change daily — treat them as a popularity signal, not a quality verdict.

## How to use this list

1. Start with one workflow framework from #1–#5, not all five.
2. Add the official Anthropic skills you actually need from #8–#12.
3. Add one skill per pain point after that: UI, understanding a codebase, context, or tokens.
4. Install only what you will use. Every enabled skill adds load to context.

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

### Workflow / methodology

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 1 | Superpowers | [obra/superpowers](https://github.com/obra/superpowers) — ~306k stars, checked 2026-10-28 via GitHub | Plan-first, test-driven development, systematic debugging, subagent-driven development, verification before completion | You want Claude Code to behave like a disciplined senior engineer, not jump straight to code |
| 2 | Matt Pocock Skills | [mattpocock/skills](https://github.com/mattpocock/skills) | Small, composable skills for real engineering | You want bite-size skills you can pick one at a time |
| 3 | Addy Osmani Agent Skills | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — ~101k stars | Production-grade spec, build, test, ship workflows | You want a production shipping workflow, not just a coding helper |
| 4 | GSD — Get Shit Done | [gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) | Spec-driven context engineering | You want a spec before code, and context kept tight |
| 5 | BMAD-METHOD | [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) | Agile AI-driven development method | You want an agile, role-based method for larger builds |

### Thinking / discipline

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 6 | Karpathy Skills | [anthropics/skills discussion / andrej-karpathy-skills](https://github.com/Anthropic-OpenSource/andrej-karpathy-skills) — see note below | Think before coding, simplicity first, surgical changes, goal-driven execution; bug fix = write a reproducing test first | You keep getting over-complicated, 1000-line fixes for 100-line problems |
| 7 | Planning with Files | [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Breaks tasks into discrete steps, tracks progress in files | Any coding task longer than a few minutes, where Claude loses track |

Note on #6: the Karpathy rules circulate as a single CLAUDE.md file in several mirrors. Verify the source you install from, and read it before use. It biases toward caution — do not run the full ritual on a typo fix.

### Official Anthropic — software engineering only

Source: [anthropics/skills](https://github.com/anthropics/skills) — ~184k stars, 19 skill folders as of 2026-10-21. Only the SWE ones are in the Top 20. Document, brand, art, and comms skills are in `archive/`.

| # | Skill | What it does | When to use it |
|---|---|---|---|
| 8 | skill-creator | A skill that writes skills, following Anthropic's authoring best practices | Every time you catch yourself explaining the same procedure twice |
| 9 | mcp-builder | Guide for creating high-quality MCP servers | You need Claude to connect to an API, database, or outside service |
| 10 | frontend-design | Distinctive, production-grade UI direction | You build web interfaces and want to avoid generic-looking pages |
| 11 | artifacts-builder | Build complex claude.ai HTML artifacts with React, Tailwind CSS, shadcn/ui | You build interactive artifacts / web apps in Claude |
| 12 | webapp-testing | Test local web apps with Playwright for UI verification and debugging | You need browser-driven QA before you ship a web app |

### Frontend / UI

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 13 | UI-UX Pro Max | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Design intelligence: styles, palettes, UX rules | Your UI looks AI-made; you want a searchable design system |
| 14 | Taste Skill | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | Strict anti-slop rules for landing pages | You want taste / restraint, not more components |

Caveat: independent blind tests in Oct 2026 ranked Taste last on one test and UI-UX Pro Max first, with high token cost for some design skills. Use one design skill at a time, and judge on your own brief.

### Understanding / docs / context

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 15 | Understand-Anything | [Understand-Anything](https://github.com/DerZyklop/Understand-Anything) — see source repo for exact owner | Turns a codebase into an interactive knowledge graph you can explore and ask questions about | You are onboarding to an unfamiliar codebase |
| 16 | Context7 | [upstash/context7](https://github.com/upstash/context7) | Keeps up-to-date library documentation available to the model | Claude keeps using outdated library APIs |
| 17 | Claude-Mem | [claude-mem](https://github.com/thedotmack/claude-mem) | Persistent context / memory across sessions | Claude forgets your project between sessions |
| 18 | Diagram Design | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — ~53k stars | Architecture, flow, org, and timeline diagrams, 44 types, exports HTML / SVG / PNG | You need deck-ready architecture diagrams from a codebase or brief |

### Efficiency / harness

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 19 | Caveman | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Cuts output tokens hard while keeping technical accuracy | You are hitting usage limits or cost, and want shorter output |
| 20 | ECC | [affaan-m/ecc](https://github.com/affaan-m/ecc) — see source repo for exact owner | Agent harness optimization: skills, memory, security, research-first workflows | You want one harness system across Claude Code, Codex, Cursor, and related tools |

Verify #15 and #20 owner/repo paths in the source list before installing — names are widely mirrored. Do not install a fork without reading it.

## Watchlist — candidates for next Saturday

These did not make v1, but are the first to test if a Top 20 slot opens:

- gstack (garrytan/gstack) — full team-in-a-box process
- Hallmark (Nutlope/hallmark) / Impeccable (pbakaus/impeccable) — anti-AI-slop design, alternative to #13 / #14
- GitNexus — client-side knowledge graph with built-in RAG agent, alternative to #15
- Context Engineering / Context Mode — token / context optimization, alternative to #19
- claude-api (Anthropic) — reference for building with the Claude API and SDKs

## What was deliberately left out

See `archive/ARCHIVED.md`. Short version: algorithmic-art, canvas-design, brand-guidelines, internal-comms, slack-gif-creator, theme-factory, and docx / pdf / pptx / xlsx. All real Anthropic skills, just not software engineering.

## Curation rules

Full rules in `CURATION.md`. Short version:

- SWE only.
- Maintained: a commit or release in the last 90 days, or a clear maintained status.
- Actually installable and tested on a real task, not just starred.
- Stars help, they do not decide.
- Max 20. One in, one out. Archive, do not delete.
- Updated every Saturday morning, ~9:00 AM PT.

## License / attribution

This repo is a curated index with links. Each skill keeps its own license and owner. Do not copy a skill's files here without checking its license.

# Curation rules

## Goal

A Top 20 list of Claude skills a software engineer must have, kept current every week. Not a dump of everything on GitHub.

## Scope: in

- Software engineering only: planning, coding, testing, debugging, refactoring, code review, architecture, docs for code, deployment, MCP, API and SDK work, frontend engineering, developer tooling.
- Skills that work in Claude Code, ideally also in Codex, Cursor, or compatible agents.
- Skills with a clear install path: plugin marketplace, npx skills add, or a SKILL.md folder you can copy.

## Scope: out

- Creative work for its own sake: generative art, posters, GIFs.
- Brand, internal comms, marketing, SEO, general writing.
- Document production (docx, pdf, pptx, xlsx) unless it is part of a dev workflow. Those live in archive.
- Skills with no maintained source, no README, or a broken install.

## How a skill gets in

All four must hold:

1. Useful on a real task. It solves a concrete pain: losing track on long tasks, generic UI, outdated docs, no tests, flaky debugging, token waste, forgotten context.
2. Maintained. A commit, release, or maintainer activity in the last 90 days, or an official Anthropic source that is still current.
3. Verifiable. Source repo, license, and install command can be checked. Star count is noted but proves nothing.
4. Distinct. It does not duplicate a Top 20 skill already in the list. If two skills do the same job, keep the better maintained one and archive the other.

## How a skill gets dropped

- Unmaintained for 90+ days, broken install, or replaced by a better skill.
- A new skill beats it on the same job in a head-to-head test.
- It drifts out of software engineering scope.

When dropped: move it to archive/ARCHIVED.md with date, reason, and what replaced it. Never delete the record.

## How we write

- Write like a person, not an assistant. Short sentences. Plain words.
- Keyboard characters only. No em dashes, no special symbols, no decorative unicode. A hyphen does the job.
- Minimalism: say it once, say it short. Essentialism: every line earns its place. Craftsmanship: get the details right, check the links, spell things correctly.

## Weekly process, every Saturday around 9am PT

1. Check the Top 20: stars, last commit, open issues, breaking changes.
2. Check the watchlist and new contenders from the past week: GitHub trending, Reddit r/ClaudeAI and r/programming, Dev.to, Hacker News.
3. Test-install any candidate before adding. Do not add untested skills.
4. Swap at most 3 per week, usually 0 to 1. Stability matters.
5. Update README.md (date, table, watchlist), CHANGELOG.md (what changed and why), archive/ARCHIVED.md (dropped skills).
6. Commit with a plain human message. Example: "Weekly curation Oct 31: swapped X for Y".

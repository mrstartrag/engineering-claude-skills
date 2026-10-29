# Curation rules

## Goal

A Top 20 list of Claude skills a software engineer must have, kept current every week. Not a dump of everything on GitHub.

## Scope — in

- Software engineering only: planning, coding, testing, debugging, refactoring, code review, architecture, docs for code, deployment, MCP, API/SDK work, frontend engineering, developer tooling.
- Skills that work in Claude Code, and ideally also in Codex / Cursor / compatible agents.
- Skills with a clear install path: plugin marketplace, `npx skills add`, or copy a `SKILL.md` folder.

## Scope — out

- Creative / design-for-its-own-sake: generative art, canvas posters, GIFs.
- Brand, internal comms, marketing, SEO, general writing.
- Document production (docx / pdf / pptx / xlsx) unless it is directly a dev workflow. Those live in `archive/`.
- Skills with no maintained source, no README, or a broken install.

## How a skill gets in

All four must hold:

1. **Useful on a real task.** It solves a concrete SWE pain: losing track on long tasks, generic UI, outdated docs, no tests, flaky debugging, token waste, forgetting context.
2. **Maintained.** A commit, release, or maintainer activity in the last 90 days, or an official Anthropic source that is still current.
3. **Verifiable.** Source repo, license, and install command can be checked. Star count is noted, but is not proof.
4. **Distinct.** It does not duplicate a Top 20 skill already in the list. If two skills do the same job, keep the better-maintained one and archive the other.

## How a skill gets dropped

- Unmaintained for 90+ days, broken install, or superseded by a better skill.
- A new skill beats it on the same job in a head-to-head test.
- It drifts out of SWE scope.

When dropped: move it to `archive/ARCHIVED.md` with date, reason, and what replaced it. Never delete the record.

## Weekly process — every Saturday, ~9:00 AM PT

1. Check the Top 20: stars, last commit, open issues, breaking changes.
2. Check the watchlist and new contenders from the past week: GitHub trending, Reddit r/ClaudeAI / r/programming, Dev.to, Hacker News.
3. Test install for any candidate that would enter. Do not add untested skills.
4. Swap at most 3 per week, usually 0–1. Stability matters.
5. Update README.md (date, table, watchlist), CHANGELOG.md (what changed and why), and archive/ARCHIVED.md (dropped skills).
6. Commit as `chore(curation): weekly update YYYY-MM-DD`.

## Versioning

- v1: 2026-10-27, initial Top 20.
- Each Saturday is a dated update, not a new v-number, unless the scope changes.

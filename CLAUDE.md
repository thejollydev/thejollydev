# CLAUDE.md — thejollydev

**`AGENTS.md` is authoritative.** Read it first; everything harness-neutral
lives there on purpose, so Claude Code, Codex and Antigravity all get the same
contract. Nothing in this file repeats a rule from it.

Claude-Code-specific notes only:

- Run `git pull` before starting anything, not just before pushing. The snake
  workflow commits to `main` on a 12-hour schedule, so a branch cut from a stale
  local `main` will conflict on a file you never touched.
- Preview README changes on GitHub itself rather than trusting a local Markdown
  render. Badge rows and tables lay out differently there, and layout is the
  point on a profile page.

# thejollydev — Agent Contract

Read by every agent: Claude Code, Codex and Antigravity all read this file.
Machine-wide conventions live in `~/.claude/CLAUDE.md`.

This repository owns the **GitHub profile surface** for the `thejollydev`
account: the `README.md` that renders at github.com/thejollydev, and the
scheduled workflow that keeps its contribution graphic current. There is no
application code — a README, one GitHub Actions workflow, and one generated
SVG. For most people arriving from a job posting, a referral or a repo link,
this page is the first and often the only thing they read.

## Startup

Before substantive work, resolve this repository to its workspace and read the
context:

```bash
never4ga --actor <client>/<model> context startup --client <client> --cwd "$PWD"
never4ga workspace resolve
```

`--actor` is a global flag and goes *before* the subcommand. It records who
wrote what, and `core/02` §5.2 requires the `<producer>/<version>` form —
`claude-code/claude-opus-5`, never bare `claude-code`.

The vault is `~/Vaults/never-knowledge`; this project's workspace is
`10_Workspaces/TheJollyDev/`. If Never4gA is unavailable, read the same files by
path and say that shared context was unavailable rather than guessing.

## Where authority lives

| Question | Source |
|---|---|
| What is open right now? | The tracker — the startup pack ends with it |
| What does the profile currently say? | `README.md` here; read it directly |
| What is this project for? | `workspace.md` in the workspace |
| Orientation and traps | `Context/agent-context.md` |
| What happened last? | `Logs/<year>/` in the workspace |

The vault holds the work; this repository holds the product. No repo-side
documentation mirrors.

## Hard rules

- **`dist/github-contribution-grid-snake.svg` is generated. Never edit it.**
- **Repo visibility, the repo name, and account settings are human-only.**
  Renaming this repository silently unpublishes the profile page.
- **The README asserts facts owned by other projects** — service counts, stack
  claims, "10+ services deployed". Verify against `bezaforge-infrastructure`
  before repeating them. Do not edit them here on the strength of what this
  README already says.
- **Badges are content, not decoration.** They carry the claims a visitor reads
  first, and shields.io colour choices are an accessibility concern.

## Traps

- **`main` moves without you.** The snake workflow auto-commits every 12 hours.
  **Pull before branching, and pull before pushing** — and do not read an
  unexpected commit as someone else's work in progress.
- **`git remote get-url --all origin` returns fetch URLs — GitHub only.** Use
  `--push --all`, or you will inspect one remote and report three.

## Checks

There is no test suite. The only workflow present drives the contribution
graphic; it is not a gate. What actually matters:

- **The rendered result.** A README that parses is not a README that reads well,
  and GitHub's rendering differs from a local previewer — badge rows wrap and
  tables behave differently.

## Conventions

The README is written in Joseph's voice: first person, plain claims backed by
links to real repositories. No emoji headers, no "passionate about" filler, no
metric that cannot be pointed at.

## Branching

All work happens on a branch and lands through a pull request. Never commit
directly to `main`, and never push to `main`.

One `origin` carries one fetch URL (GitHub) and three push URLs (GitHub, GitLab,
Gitea), so a plain `git push origin` reaches all three.

## Attribution

Never write an AI attribution anywhere: no `Co-Authored-By` naming a model or
assistant, no "Generated with", no session trailer, in a commit message, pull
request, issue or document. Commits are authored by Joseph.

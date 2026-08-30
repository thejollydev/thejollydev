# thejollydev — Agent Instructions

This repository owns the **GitHub profile surface** for the `thejollydev`
account: the `README.md` that renders at github.com/thejollydev, and the
scheduled workflow that keeps its contribution graphic current. There is no
application code — a README, one GitHub Actions workflow, and one generated
SVG. For most people arriving from a job posting, a referral or a repo link,
this page is the first and often the only thing they read.

## Hard rules

- **`dist/github-contribution-grid-snake.svg` is generated. Never edit it.**
- **Repo visibility, the repo name, and account settings are human-only.**
  Renaming this repository silently unpublishes the profile page.
- **The README asserts facts owned by other projects** — service counts, stack
  claims, "10+ services deployed". Verify them against their source before
  repeating them. Do not edit them here on the strength of what this README
  already says.
- **Badges are content, not decoration.** They carry the claims a visitor reads
  first, and shields.io colour choices are an accessibility concern.

## Traps

- **`main` moves without you.** The snake workflow auto-commits every 12 hours.
  **Pull before branching, and pull before pushing** — and do not read an
  unexpected commit as someone else's work in progress.
- **`git remote get-url --all origin` returns fetch URLs only.** Use
  `--push --all` if you need to inspect where pushes go.

## Checks

There is no test suite. The only workflow present drives the contribution
graphic; it is not a gate. What actually matters is **the rendered result** — a
README that parses is not a README that reads well, and GitHub's rendering
differs from a local previewer: badge rows wrap and tables behave differently.

## Conventions

The README is written in the first person, with plain claims backed by links to
real repositories. No emoji headers, no "passionate about" filler, no metric
that cannot be pointed at.

## Contributing

All work happens on a branch and lands through a pull request. Nothing is
committed or pushed directly to `main`.

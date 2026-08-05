# AGENTS.md

## Scope

This repository contains capture profiles and server configuration consumed by [prunus](https://github.com/meop/prunus).

## Working conventions

- Keep reusable capture profiles under `cfg/profiles/`.
- Each profile must retain distinct `## Capture` and `## Skip` sections because prunus parses those headings.
- Write profile guidance as concise instructions for the extraction model and preserve the intent of neighboring rules.
- Do not create or alter live per-tree profile symlinks merely to validate repository content.

## Validation

- Confirm edited profiles contain exactly the expected `## Capture` and `## Skip` headings.
- Preview Markdown changes for broken structure or malformed examples.
- Run `git diff --check` before committing.

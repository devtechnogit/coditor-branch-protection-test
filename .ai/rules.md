# Project rules

## Context files
- `rules.md` is the always-on source of truth. Keep it small. Add a convention when the user states one.
- `active-context.md` is current work only (aim for under 80 lines). Do not append session novels.
- `.ai/story/` holds rare decisions, one file each. Search it; do not preload it.
- Do not touch every context file on each change.

## Purpose
This is a throwaway repository (`coditor-branch-protection-test`). Its README says it exists to test whether a Coditor bot review counts toward GitHub branch protection required approvals, and that it is safe to delete.

## Stack
None. The repository has no source code, package manifests or build tooling. It contains only `README.md`.

## Commands
No test, lint or build commands are defined.

## Conventions
- Commit messages seen in history use a conventional prefix, e.g. `test: ...`.
- Changes land on `main` through pull requests (e.g. `#1`).

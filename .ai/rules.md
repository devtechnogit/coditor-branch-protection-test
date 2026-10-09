# Project rules

## Context files
- `rules.md` is the always-on source of truth. Keep it small. Add a convention when the user states one.
- `active-context.md` is current work only (aim for under 80 lines). Do not append session novels.
- `.ai/story/` holds rare decisions, one file each. Search it; do not preload it.
- Do not touch every context file on each change.

## Purpose
This is a throwaway repository (`coditor-branch-protection-test`). It exists to test whether a Coditor bot review counts toward GitHub branch protection required approvals, and that it is safe to delete.

## Stack
None. The repository has no source code, package manifests or build tooling. It contains only Markdown docs (`README.md`, `CONTRIBUTING.md`), `.markdownlint-cli2.yaml` and `.gitattributes` (`* text=auto eol=lf`: text files are normalized to LF).

## Commands
No test or build commands are defined. Markdown is linted with markdownlint-cli2 using the root `.markdownlint-cli2.yaml` (e.g. `npx markdownlint-cli2`); no package.json or CI step runs it yet.

## Conventions
- Commit messages follow Conventional Commits (e.g. `feat:`, `fix:`, `docs:`, `test:`, `chore(scope):`). This is a project rule.
- Changes land on `main` only through draft pull requests (e.g. `#1`); no direct pushes to `main`. This is a project rule.

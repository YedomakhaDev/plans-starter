# Block for CLAUDE.md / AGENTS.md

Copy the block below into `CLAUDE.md` and/or `AGENTS.md` in the project root.

```markdown
## Plans

All project information lives in `_plans/` (a separate git repository, ignored in the main repo).
Start with `_plans/README.md` — it maps every file.

- Project context: `_plans/project/context.md`
- Features: `_plans/features/<YYYY-MM-DD-slug>/` — before working on a feature, read its README.md, brief.md, and open-questions.md
- How to maintain the folder: `_plans/general-rules/plans-workflow.md`

Rules to follow:
- Commits: `_plans/general-rules/commits.md`
- Branches: `_plans/general-rules/branches.md`
- Language (code and everything for the client — in English): `_plans/general-rules/language.md`

While working:
- Record new decisions in decisions.md and new questions in open-questions.md (feature or project).
- Created or deleted a file in `_plans/` — update `_plans/README.md`.
- Track feature progress in its tasks.md.
```

# Agent instructions: AGENTS.md + CLAUDE.md

Keep agent rules in **one** file — `AGENTS.md` in the project root. Codex, Cursor, and other agents read it.
Claude Code reads `CLAUDE.md`, so it contains a single import line:

```markdown
@AGENTS.md
```

This way the rules live in one place and don't drift between files.

Copy the block below into `AGENTS.md` and add a heading and 1–2 sentences about the project on top.

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
- Design: `_plans/project/design/` — `tokens.md` is the source of truth for colors, fonts, and sizes; approved copy only in designs

While working:
- Record new decisions in decisions.md and new questions in open-questions.md (feature or project).
- Created or deleted a file in `_plans/` — update `_plans/README.md`.
- Track feature progress in its tasks.md.
```

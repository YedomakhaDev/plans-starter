# Connecting to a project

Repositories:

- **plans-starter** (this one) — the template. Only `general-rules/`, `features/_template/`, and the empty stubs change here.
- **plans-<project>** — a separate private repository for each project. Created from the template; it holds the briefs, correspondence, and features.

This keeps client data out of the template, while rule updates can be pulled into any project.

## New project

```bash
cd /path/to/project
git clone https://github.com/YedomakhaDev/plans-starter.git _plans
cd _plans
git remote rename origin template      # the template stays as upstream
git remote add origin <url-plans-project>
git push -u origin main
```

In the project's main repository, add to `.gitignore`:

```
_plans/
```

Then fill in `project/context.md` and paste the block from [general-rules/ai-agents.md](general-rules/ai-agents.md) into the project's `CLAUDE.md` / `AGENTS.md`.

## Pull updated rules from the template

```bash
cd _plans
git pull template main
```

Conflicts are only possible in files that exist in both repositories. So don't edit filled-in `project/` files in the template — only rules and stubs.

## Improve a rule from a project

Found a good rule in a project — move it to `plans-starter` and commit it there. Then pull it into the other projects with the command above.

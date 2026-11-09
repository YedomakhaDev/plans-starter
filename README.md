# Plans

A project workspace: briefs, estimates, correspondence, decisions, features, and general rules.
Cloned into the project root as `_plans/`. How to connect it to a new project: [SETUP.md](SETUP.md).

> Rule: added a file or folder — add a line here.

## General rules — `general-rules/`

The same for every project. Referenced from the project's `AGENTS.md` (`CLAUDE.md` imports it).

| File | Purpose |
|---|---|
| [plans-workflow.md](general-rules/plans-workflow.md) | How to maintain this folder: what goes where, how to name files |
| [commits.md](general-rules/commits.md) | Commit workflow (plan → approval → commits) and message format |
| [branches.md](general-rules/branches.md) | Branch naming and workflow |
| [language.md](general-rules/language.md) | What must be in English and what can be in your working language |
| [ai-agents.md](general-rules/ai-agents.md) | Agent instructions: block for `AGENTS.md`, plus `CLAUDE.md` with an import |

## Project — `project/`

Everything about the project as a whole.

| File / folder | Purpose |
|---|---|
| [context.md](project/context.md) | What the project is: client, contacts, stack, access, links |
| [brief/](project/brief/) | Original briefs, specs, designs, files from the client |
| [estimates/](project/estimates/) | Project estimates and their versions |
| [correspondence/](project/correspondence/) | Important client correspondence and calls |
| [decisions.md](project/decisions.md) | Log of decisions made and why |
| [open-questions.md](project/open-questions.md) | Open questions for the client and for myself |
| [backlog.md](project/backlog.md) | Ideas and tasks that haven't become features yet |
| [design/](project/design/) | Design: direction, tokens, components, concept log, references |

## Features — `features/`

One feature — one folder `YYYY-MM-DD-feature-slug/`, a copy of [features/_template/](features/_template/).

| Feature | Status | Summary |
|---|---|---|
| _none yet_ | | |

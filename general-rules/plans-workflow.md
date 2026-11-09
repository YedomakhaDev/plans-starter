# How to maintain the Plans folder

## What goes where

| What came in | Where |
|---|---|
| New project, overall brief, specs, designs | `project/brief/` |
| Estimate for the whole project | `project/estimates/` |
| Email, chat, call about the project as a whole | `project/correspondence/` |
| Decision that affects the project | `project/decisions.md` |
| Question without an answer | `open-questions.md` (project or feature) |
| "Someday" idea | `project/backlog.md` |
| New feature or large task | new folder in `features/` |
| Rule for all projects | `general-rules/`, then into the `plans-starter` template |

If the information belongs to a specific feature, put it in the feature folder, not in `project/`.

## Naming

- Files and folders: `kebab-case`, Latin characters.
- Dated files: `YYYY-MM-DD-topic.md`, e.g. `2026-11-09-kickoff-call.md`.
- Feature folders: `YYYY-MM-DD-feature-slug`, the feature start date. E.g. `2026-11-09-distributors-map`.
- Estimate versions: `YYYY-MM-DD-estimate-v1.md`, `...-v2.md`. Don't delete old ones.

## New feature

1. Copy `features/_template/` to `features/YYYY-MM-DD-feature-slug/`.
2. Fill in the feature's `README.md`: summary, status, links.
3. Add a row to the features table in the root `README.md`.

## Correspondence

- Save it as text (markdown), not screenshots — so it's searchable and can be passed to AI.
- At the top of the file: date, participants, channel (email / Slack / call).
- At the bottom: a short summary — what was decided and what to do next.
- Copy decisions from correspondence into `decisions.md`, questions into `open-questions.md`.

## Feature statuses

`idea` → `estimating` → `approved` → `in-progress` → `review` → `done` / `cancelled`

## Keeping it tidy

- Added or removed a file — update the root `README.md`.
- Question closed — move it to "Closed" with the answer instead of deleting it.
- Raw attachments (PDFs, images, archives) — next to the markdown file that describes them.
- Secrets (passwords, keys, tokens) do **not** go here. Only a link to where they're stored.

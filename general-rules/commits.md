# Commits

## Git: Logical Commits

Analyze all uncommitted changes in the current Git branch.

Group the changes into logical, atomic commits based on their purpose (feature, fix, refactor, styling, docs, tests, etc.).

For each proposed commit:
- Create a clear Conventional Commit message.
- List the files that will be included.
- Briefly explain why these files belong together.

Before staging or committing anything, present the complete commit plan and wait for my approval.

Do not stage any files, create any commits, or modify the Git index until I explicitly approve the plan.

After approval, stage only the relevant files for each commit and create the commits in the proposed order.

Never add co-authorship trailers (e.g. "Co-Authored-By") or any AI attribution to commit messages unless I explicitly ask for it.

Do not push.

If any file belongs to multiple logical changes, or if there is any ambiguity about how changes should be grouped, stop and ask for clarification before proceeding.

---

## Message format reference

[Conventional Commits](https://www.conventionalcommits.org/), in English.

```
<type>(<scope>): <subject>

<optional body: what and why>

<optional footer: Refs #123, BREAKING CHANGE: ...>
```

### Types

| Type | When |
|---|---|
| `feat` | New functionality |
| `fix` | Bug fix |
| `refactor` | Code change without behavior change |
| `style` | Formatting, CSS without logic changes |
| `perf` | Performance |
| `docs` | Documentation, README, plans |
| `test` | Tests |
| `build` | Build, dependencies, composer / npm |
| `ci` | CI/CD, deploy scripts |
| `chore` | Other maintenance |
| `revert` | Revert a commit |

### Rules

- **subject:** imperative mood (`add`, not `added`), lowercase, no trailing period, up to ~72 characters.
- **scope:** part of the project — `theme`, `blocks`, `woo`, `acf`, `header`, `checkout`, etc. Optional.
- Never commit secrets, `.env`, `node_modules`, `vendor`, build output (unless needed in production), or DB dumps.
- Make sure the build and linters pass before committing.

### Examples

```
feat(blocks): add testimonials slider block
fix(woo): correct tax calculation for EU customers
refactor(theme): move enqueue logic to separate class
build: bump @wordpress/scripts to 30.x
docs(plans): add estimate v2 for distributors map
```

### In the Plans repository

Type `docs`, scope is the feature or section:

```
docs(distributors-map): add client brief and open questions
docs(project): log decision on hosting
```

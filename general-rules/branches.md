# Branches

## Main branches

- `main` — what's in production. No direct commits (except small projects without a process).
- `develop` / `staging` — if the project has a staging environment.

If the agency has its own rules — follow them and record them in `project/context.md`.

## Working branches

```
<type>/<short-description>
```

| Prefix | When |
|---|---|
| `feature/` | New feature |
| `fix/` | Bug |
| `hotfix/` | Urgent production fix |
| `refactor/` | Refactoring |
| `chore/` | Maintenance, dependencies |

- `kebab-case`, Latin characters, short: `feature/distributors-map`, `fix/checkout-tax`.
- If there's a tracker task — its ID first: `feature/PROJ-123-distributors-map`.
- A feature branch name matches the slug of its folder in `features/` (without the date).

## Workflow

1. Branch off the latest `main` (or `develop`).
2. Commit following [commits.md](commits.md).
3. Before the PR: rebase onto the fresh base, build and linters pass.
4. PR with a description: what was done, how to test, link to the feature in Plans.
5. Delete the branch after merging.

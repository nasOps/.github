# Contributing to nasOps projects

## Branching strategy

We use trunk-based development. All feature branches merge directly to `main` — there is no long-lived `development` branch.

- Create a branch from a GitHub issue (auto-named `<issue-number>-<title>`, e.g. `42-add-ci-pipeline`)
- No prefixes like `feature/` or `bugfix/`
- Delete branches after merge

## Commit messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>: short description
```

Types in use: `feat`, `fix`, `chore`, `docs`, `devops`, `bug`

Danish and English are both acceptable.

## Pull requests

- PRs always target `main`
- Squash merge only — one commit per issue on `main`
- Requires 1 approval + all CI checks passing
- Use the PR template in `.github/PULL_REQUEST_TEMPLATE.md`

## CI

CI runs automatically on push and PR. Before opening a PR, run locally:

```bash
bundle exec rubocop
bundle exec rspec
```

# communicator: notes for agents

- What it is: Space Disco Communicator & Discotronic Flight Assistant, an Ember + Cordova app shell (2020). Part of the Space Disco org (Steven's party and music brand, being revived). Dormant code: keep changes small and say what you couldn't run.
- Stack: JavaScript, Ember CLI 3.x, Cordova via corber.
- Layout: Standard Ember layout: `app/` routes, templates and components; `tests/`; `corber/` the Cordova wrapper; `config/` environment.
- Commands:

  ```sh
  # Needs an old Node (the scaffold targets Node 6-12); nvm use 12
  npm ci
  npm test
  ```

- CI runs gitleaks on new commits and a PR title check. Nothing is built in CI yet (see docs/STATUS.md).
- Every change comes with a test when there is something testable; every bug fix with a test that failed before the fix.
- Commits and PR titles use Conventional Commits (`feat:`, `fix:`, `docs:`, `ci:`, `build:`, `chore:`, `test:`, `refactor:`).
- One PR per change, squash merged into the default branch. Agents merge their own PRs once CI is green. Say plainly in the PR what wasn't built or run.
- Never commit secrets or personal data. Config comes from environment variables; real values live in Steven's Bitwarden vault.
- Never without Steven's yes: deploying, publishing a package or app, making the repo public, changing repo settings, deleting data or rewriting history, spending money.
- Update docs/STATUS.md when a PR merges.
- The full repo standard and its model repo: spacedisco/playlog (docs/plan/repo-standard.md).

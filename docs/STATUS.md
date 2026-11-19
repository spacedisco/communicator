# Status

Updated 2026-11-19, when the repo standard baseline was applied.

**State:** dormant. Space Disco is being revived (spacedisco.com); this repo is kept as part of that.

## What works
- Docs, secrets scan and PR title checks run in CI.

## Known broken or missing
- The 2020 Ember toolchain doesn't install on Node 22, so nothing is built in CI.
- Seven open Dependabot security PRs against that toolchain; they can't be verified without a working build.
- `.travis.yml` is left over; Travis CI is not connected.

## Next
- If the revival wants a crew app, start fresh (a small web app or a ZYLR-style native app) rather than upgrading this scaffold.

## Not done yet from the repo standard
- Default branch `main`, branch protection with required checks and squash-only merges: repo settings, Steven's to-do.
- release-please, signed releases and a coverage floor: added when the repo is revived and has something to release.

## Log
- 2026-11-19: repo standard baseline (AGENTS.md, CLAUDE.md, CONTRIBUTING, SECURITY, STATUS, decision record, editorconfig, templates, CODEOWNERS, Dependabot, CI).


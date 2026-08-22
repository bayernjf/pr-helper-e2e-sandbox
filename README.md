# PR Helper E2E Sandbox

Public, disposable repository for validating PR Helper against real GitHub APIs.

## Branches

- `feature/test` and `fix/test`: independent source routes.
- `dev`: integration target.
- `main`: release target.

## Test controls

- Open a PR from either source branch to `dev`, then from `dev` to `main`.
- The `PR gate` workflow succeeds by default and is required by branch protection.
- Add a `.pr-helper-e2e/fail-ci` file to a source branch to make `PR gate` fail deliberately.
- Pushes merged into `dev` or `main` run `Post-merge verification`.

Do not store secrets, production configuration, or application code here.

Archive acceptance run at 2026-08-17T16:04:15Z

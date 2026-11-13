# git-api-sandbox

Verification repository for live-testing the `git-api` CLI (Forkline). Tiny on purpose.

- CI (`.github/workflows/ci.yml`): job `pass` always succeeds; job `gate` fails iff a file named `FAIL` exists at the repo root.
- `requirements.txt` pins an old, vulnerable `requests` on purpose so Dependabot raises alerts. Do not upgrade it.
- Base branch `main` is protected: checks `pass` and `gate` required, 0 approvals, conversations must be resolved.

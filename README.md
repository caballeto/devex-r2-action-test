# devex-r2-setup-devhelm

Round 2 sandbox for testing `devhelmhq/setup-devhelm@v1` in CI.

The workflow at `.github/workflows/test.yml`:
- pins `devhelmhq/setup-devhelm@v1`
- passes `api-token` via `secrets.DEVHELM_API_TOKEN`
- runs `devhelm monitors list --output json | head -5` to prove the CLI is on PATH and authenticated against the prod API.

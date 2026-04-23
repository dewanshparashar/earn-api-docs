# Arbitrum Earn API docs

OpenAPI reference for the Earn endpoints on Arbitrum Portal, rendered with [Scalar](https://github.com/scalar/scalar).

**Live docs:** https://dewanshparashar.github.io/earn-api-docs/

## Source of truth

This repo only contains the spec (`openapi.yaml`) and a static viewer. The actual route handlers live in the Arbitrum Portal monorepo:

- Repo: https://github.com/OffchainLabs/arbitrum-portal (private)
- Path: `packages/app/src/app/api/onchain-actions/v1/earn/`

When the API changes, update `openapi.yaml` here to match. Commit to `main` and GitHub Pages redeploys automatically.

## Local preview

`index.html` loads Scalar from a CDN, so any static server works:

```
python3 -m http.server 8000
```

Then open http://localhost:8000/.

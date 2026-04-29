# Secrets Policy

## What Counts As A Secret
Secrets include tokens, API keys, passwords, credentials, private keys, session values, database URLs with credentials, private deployment hooks, and any value that grants access.

## Related Terms
Config values may be harmless settings. Public IDs may identify a public project. Private URLs can expose non-public resources. Environment variables can hold either config or secrets.

## Rules
- No real secrets or fake-looking secrets should be stored in this repo.
- Use placeholders only.
- Do not paste secrets into prompts, examples, reports, or GitHub files.

## Safe Placeholders
- `YOUR_API_KEY_HERE`
- `NETLIFY_SITE_ID_PLACEHOLDER`
- `GITHUB_TOKEN_PLACEHOLDER`
- `DATABASE_URL_PLACEHOLDER`

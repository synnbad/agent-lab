# Environment Variable Rules

Local environment variables may be stored in `.env`, `.env.local`, or platform-specific secret stores. `.env` files are ignored. `.env.example` may be committed only with placeholders.

GitHub repository secrets and GitHub Actions secrets should hold workflow secrets. Netlify environment variables should hold deployment configuration and secrets.

Build-time variables are available during builds. Runtime variables are used by the running application. Public frontend variables may be exposed to browsers, so private server-side secrets must never be placed there.

Rules:
- Never expose private server-side secrets to frontend code.
- Never paste secrets into prompts.
- Never store secrets in agent examples.
- Use placeholders in documentation.

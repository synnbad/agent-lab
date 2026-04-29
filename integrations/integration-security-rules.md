# Integration Security Rules

## Rules
- Read-only by default.
- Explicit approval is required for writes.
- Explicit approval is required for deployments.
- Explicit approval is required for publishing.
- Explicit approval is required for environment variable changes.
- No secrets in GitHub.
- No raw client files in public repos.
- No sensitive student, staff, patron, client, HR, medical, immigration, or institutional data in examples.
- Prefer redacted, anonymized, or aggregated data.
- Clearly state when an adapter is unavailable.
- Provide manual fallback steps.
- Treat MCP servers as powerful but risky because they can expose tools and actions.
- Separate read tools from write tools.
- Label destructive actions clearly.
- Never assume a platform supports a connector just because another AI platform does.

## Approval Evidence
Approval should name the adapter, action, access level, target system, and allowed scope.

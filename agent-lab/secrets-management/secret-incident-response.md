# Secret Incident Response

## Response Checklist
1. Stop using the exposed secret.
2. Revoke or rotate the secret.
3. Remove the secret from current files.
4. Check commit history.
5. Check whether the secret reached a public remote.
6. Audit logs if available.
7. Replace the secret with a safe environment variable.
8. Review related integrations.
9. Document the incident.
10. Add prevention steps.

## Severity Levels
- Low: Placeholder or non-sensitive config was exposed.
- Medium: Internal-only config was exposed without access power.
- High: A real secret may have been exposed privately.
- Critical: A real secret reached a public remote or may have been used.

## Who To Notify
Notify the system owner, repository maintainer, security contact, and affected stakeholders based on severity.

## What To Document
Document the secret type, exposure path, timeline, rotation status, affected systems, corrective actions, and prevention steps.

## Prevention
Use `.gitignore`, secret scanning, minimal permissions, environment variables, and review before commits.

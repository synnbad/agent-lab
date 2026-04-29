# Tool Use Guardrails

## Purpose
Default to read-only. Require explicit approval before writes, deployments, publishing, editing external files, changing environment variables, or destructive actions. Use manual fallback if an integration is unavailable.

## Required Behavior
- Identify the risk before acting.
- Use the minimum access needed.
- Ask for explicit approval before Level 2, Level 3, or Level 4 activity.
- Document assumptions, limitations, and approval status.

## Review Checklist
- Sensitive data checked
- Prompt-injection risk checked
- Approval gates checked
- Manual fallback available
- Final output suitable for human review

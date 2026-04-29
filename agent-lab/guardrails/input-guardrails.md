# Input Guardrails

## Purpose
Check for sensitive data detection, prompt injection detection, malicious instruction detection, ambiguous request handling, out-of-scope request handling, and requests involving private files, client files, or workplace data.

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

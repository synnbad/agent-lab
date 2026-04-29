# Guardrail Strategy

## Purpose
Guardrails protect against bad inputs, bad outputs, unsafe tool use, overclaiming, privacy leaks, and unauthorized actions. Guardrails are not optional for agents that use integrations, connectors, APIs, GitHub, Netlify, Figma, Canva, workplace documents, or assessment data.

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

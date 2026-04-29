# Cross-Platform Agent Porting Workflow

## Purpose
Help convert one agent spec so it works across ChatGPT, Claude, Gemini, Microsoft Copilot Studio, Cursor, and API-based agents.

## Trigger
Use when adapting an agent to a new AI platform.

## Inputs
- Goal, audience, and desired artifact
- Source material, constraints, risks, and approval status

## Step-by-Step Process
1. Identify the target platform
2. Translate Integration Adapter terms into platform-specific terminology
3. Check whether the platform supports read-only, write, deploy, or sensitive-data access
4. Map required adapters to available tools, apps, connectors, MCP servers, actions, functions, or plugins
5. Remove unsupported capabilities
6. Add fallback instructions
7. Update security and approval rules
8. Test with a small read-only task first
9. Test draft/write behavior only after approval
10. Document platform limitations

## Output
A Markdown-ready deliverable with summary, decisions, assumptions, risks, quality checks, and next steps.

## Quality Control
Verify that the output is grounded in source context, privacy-safe, scoped to the goal, and clear enough for another person or agent to continue.

## Failure Modes
Missing source context, hidden assumptions, overbroad scope, unapproved external actions, weak privacy handling, and unclear ownership.

## Example
Use this workflow to move from a rough request to a reviewed, documented, and safe next-step artifact.

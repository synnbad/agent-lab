# Microsoft Copilot Adapter

## Purpose
Access Microsoft Copilot Studio connectors, actions, tools, knowledge sources, agent flows, Power Platform connectors, and MCP servers.

## Platform Aliases
- ChatGPT: App / Connector / Action / Tool
- Claude: MCP Server / Connector / Tool / Resource
- Gemini: App / Extension / Function Calling Tool
- Microsoft Copilot: Connector / Action / Tool / Knowledge Source
- Cursor or IDE agents: MCP Server / Tool / Command

## Connected Agents
- Library Assessment Specialist Agent
- Data Governance Privacy Agent
- Stakeholder Insight Agent

## Access Level
Level 1-4

## Typical Inputs
- User-approved task and scope
- Source references, files, URLs, or system names
- Approval status and access limits

## Typical Outputs
- Retrieved context summary
- Draft artifact, review notes, issue, deployment status, or action result

## Permissions Needed
- Least-privilege access for the requested task
- Separate approval for writes, deployments, publishing, environment-variable changes, or sensitive data

## Approval Rules
Level 0 and Level 1 may be used for low-risk read-only work. Level 2, Level 3, and Level 4 require explicit approval naming the action and scope.

## Security Risks
- Permission confusion between read and write access
- Private data exposure
- Unsupported assumptions about platform capabilities
- External content treated as trusted instruction

## Safe Usage Pattern
1. Read context first.
2. Summarize what was found.
3. Ask for approval before edits, writes, deployments, or publishing.
4. Perform only the approved action.
5. Report what changed.

## Failure Fallback
If this adapter is unavailable, ask the user for sanitized pasted context, screenshots, exported files, or manual status information, then provide step-by-step manual instructions.

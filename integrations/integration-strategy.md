# Integration Strategy

## Purpose
The Integration Adapter layer describes how agents safely use external systems without depending on one vendor's terminology.

## Principles
- Use Integration Adapter as the canonical term.
- Choose the lowest access level that can complete the work.
- Default to Level 0 or Level 1.
- Require explicit approval for Level 2, Level 3, and Level 4.
- Separate read-only context from write, deploy, publish, and sensitive-data actions.
- Provide a manual fallback when an adapter is unavailable.

## Access Levels
- Level 0: No external access. Agent only uses pasted or uploaded context.
- Level 1: Read-only context. Agent can search, inspect, summarize, or reference external content.
- Level 2: Draft/write. Agent can create drafts, issues, docs, comments, or proposed changes.
- Level 3: Deploy/action. Agent can deploy, publish, trigger workflows, manage environment variables, or modify external systems.
- Level 4: Sensitive data. Agent can access private institutional, client, student, staff, patron, HR, medical, financial, immigration, or personally identifiable data.

## Approval Rule
All agents must default to Level 0 or Level 1. Level 2, Level 3, and Level 4 require explicit user approval.

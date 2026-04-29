# Client Website Threat Model

## System Or Workflow Being Modeled
Client Website Threat Model

## Assets At Risk
- Private client content
- Accidental public commits
- Wrong deployment target
- Broken live site

## Trust Boundaries
External content, user-provided files, Integration Adapters, public repositories, deployment systems, and stakeholder-facing artifacts.

## Possible Attackers Or Failure Sources
Malicious external content, accidental user error, over-permissioned tools, stale assumptions, misconfigured deployments, and unclear ownership.

## Abuse Cases
- Private client content
- Accidental public commits
- Wrong deployment target
- Broken live site
- Unreviewed publishing
- Client brand misuse
- Form data exposure
- Accessibility failures
- Incorrect content
- Scope creep

## Likely Failure Modes
- Unapproved action or publication
- Sensitive data exposure
- Unsupported claims or incorrect assumptions
- Weak review before handoff

## Preventive Controls
- Keep raw client files out of public repos
- Use sanitized specs
- Require approval before deploy
- Test live URL before client handoff
- Document assumptions and limitations

## Detection Signals
- Unexpected tool request
- Missing approval record
- Sensitive content in output
- Broken build or incorrect published content
- Stakeholder confusion or metric dispute

## Required Approval Gates
Approval is required before writes, deployments, publishing, environment-variable changes, sensitive data use, or stakeholder-facing delivery.

## Manual Fallback
Pause automation, use sanitized summaries, perform manual review, and document the decision before continuing.

## Residual Risk
Some risk remains because external content, human interpretation, and platform behavior can change. Keep human review in the loop.

## Review Checklist
- Assets identified
- Approval gates checked
- Sensitive data minimized
- Fallback documented
- Limitations stated

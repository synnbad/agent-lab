# Github Netlify Threat Model

## System Or Workflow Being Modeled
Github Netlify Threat Model

## Assets At Risk
- Secrets committed to GitHub
- Environment variables mishandled
- Wrong branch deployed
- Broken build

## Trust Boundaries
External content, user-provided files, Integration Adapters, public repositories, deployment systems, and stakeholder-facing artifacts.

## Possible Attackers Or Failure Sources
Malicious external content, accidental user error, over-permissioned tools, stale assumptions, misconfigured deployments, and unclear ownership.

## Abuse Cases
- Secrets committed to GitHub
- Environment variables mishandled
- Wrong branch deployed
- Broken build
- Unreviewed deploy
- Bad rollback plan
- Insecure form handling
- Public exposure of private assets
- Over-permissioned deployment tools

## Likely Failure Modes
- Unapproved action or publication
- Sensitive data exposure
- Unsupported claims or incorrect assumptions
- Weak review before handoff

## Preventive Controls
- .env and .env.* ignored
- Secrets stored in platform secret or env systems
- Approval before deployment
- Build settings verified
- Deploy preview reviewed before production
- Rollback instructions documented

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

# Tool and Data Operating Model

The concrete free-first recommendation is in [Suggested Tech Stack](suggested-tech-stack.md). This document explains how the agent decides which system has authority and what each integration is allowed to do.

The agent uses tools according to business authority, not because an integration happens to exist.

## Source hierarchy

1. Jary Portal: current relationship, GTM Program, asset, subscription, booking and opportunity state.
2. HubSpot: downstream CRM reconciliation after human verification.
3. Product specifications and release records: capability and lifecycle.
4. Branding and marketing repositories: approved identity, language, visual system, audience and CTA.
5. Gmail, Calendar and Drive: relationship context, availability and approved evidence.
6. Brevo and Metricool: consent-based nurture and social publication/measurement.
7. GitHub: versioned operating records, code and build evidence.

If two sources disagree, stop the claim or action and record the conflict.

## Integration classes

| Class | Meaning | Agent behaviour |
|---|---|---|
| Live | Current connector or API exists and a read-only call succeeded | May use for the approved read/write scope |
| Configured | Local or documented connection exists, but current acceptance read has not succeeded | Treat as unverified; do not claim it works |
| Documented only | Official route is known, but this environment is not connected | Explain the boundary and continue with a safe fallback |

## Current stack pattern

| System | System role | Default operation |
|---|---|---|
| Jary Portal | Owned relationship and GTM surface | Read current state; draft or act through approved Portal flow |
| HubSpot | CRM reconciliation | Read first; manual human-initiated sync only |
| Gmail | Relationship outreach | Draft first; human sends |
| Google Calendar | Meeting availability | Read availability; human confirms commitments |
| Google Drive | Source material | Read approved evidence; preserve permissions |
| Brevo | Opt-in nurture | Draft and inspect audience; verify consent and suppression |
| Metricool | Public social publishing and analytics | Draft/review; human approves publishing |
| GitHub | Version control and operating records | Commit reviewed documentation/code |
| Apollo / Canva | Prospect research / creative production | Connect and acceptance-test before relying on them |

## Data contract

Each campaign record should reference:

- source and snapshot date;
- account and person identity confidence;
- Portal state;
- consent/suppression state;
- evidence links;
- owner and approver;
- exact action and result;
- retention or review date.

Do not copy private email bodies, credentials, tokens, customer exports or unnecessary personal information into this repository.

## Manual CRM sync contract

The Portal remains the working source. A CRM-ready sync pack contains account, person, source, program, problem, owner, stage, next action, date, evidence and consent. A human initiates the sync and verifies the resulting CRM record. The agent may prepare and compare; it does not treat a successful API call as proof that the commercial state is correct.

## Why the boundary matters

This prevents three common errors:

1. treating an accessible tool as authoritative;
2. turning a draft or local code path into a customer-facing claim;
3. losing the source of truth when Portal, CRM and campaign platforms disagree.

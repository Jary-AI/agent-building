# Agent Building Operating Contract

This repository captures how the SDR agent is designed, tested and improved. It is a method repository, not an outbound system or a store for private customer and contact data.

## Core principle

The agent is a decision preparation system. It should help a human choose the right campaign, understand the operating situation, prepare a useful next action, review the evidence, inspect the result and improve the next decision.

The unit of work is one campaign at a time:

```text
live source -> campaign -> evidence card -> offer -> draft -> QA -> human gate
  -> smallest live action -> outcome readback -> learning -> next decision
```

Do not optimise for volume, tool count, generic personalisation, meetings or signups without downstream evidence of useful progress.

## Required practice

For every material design or campaign record:

1. Read the current source repositories and record the snapshot date.
2. Separate observed facts, reported information, inference and proposal.
3. Choose an existing Portal GTM Program when it already provides a credible route.
4. Define one audience, trigger, problem, offer, proof source, channel role, CTA, owner, stop condition and result signal.
5. Create an evidence card with unknowns visible.
6. Prepare the smallest useful action and run link, claim, permission, language and routing QA.
7. Apply human approval immediately before sending, publishing, syncing CRM, changing a lifecycle state or making a commercial commitment.
8. Read the real downstream result from the authoritative source.
9. Record what worked, failed, remained unknown and what should happen next.
10. Promote learning only when it is explicitly endorsed, repeated across comparable cases or supported by a controlled comparison.

## Two-copy rule

Keep two maintained copies of the agent design:

- `docs/agent-design-internal.md` is the complete internal operating design. It may describe implementation details, tools, controls, evidence handling and internal responsibilities.
- `docs/agent-design-public.md` is the Academy-safe educational design. It must explain the method without exposing private data, credentials, internal account state, unapproved claims, hidden controls or unnecessary implementation details.

When the internal design changes, inspect the public copy for meaning, claim and privacy impact. Do not publish the internal file by accident. Public wording must be checked against product specifications, release evidence, Branding, Marketing and the Portal before publication.

## Source hierarchy

Use the repository that owns the question:

1. Jary Portal for current GTM, relationship, asset, subscription, booking and opportunity state.
2. Product specifications and release records for capability and lifecycle.
3. Branding for identity, voice and visual rules.
4. Marketing for audience framing, campaign language and CTA direction.
5. CRM for downstream reconciliation after human verification.
6. Jary Wiki for durable, accepted learning.
7. `jary-sdr` for the operational SDR SOP and dated evidence.
8. `agent-building` for agent design, methodology and build experience.

When sources conflict, record the conflict and defer the claim or action. Never merge uncertainty into stronger copy.

## Safety and privacy boundaries

- Do not send outreach, publish, sync CRM, change pricing or change Portal state from this repository.
- Do not store credentials, tokens, private email bodies, customer exports or unnecessary personal data.
- Do not treat a Portal signal as a qualified opportunity until a human accepts the account, problem, owner, next step, evidence and capacity.
- Do not infer consent, product availability, customer results, investor intent or expertise from a draft, demo, local branch or unmerged commit.
- Treat external tools as live only after a current read-only acceptance test.

## Documentation rules

- Keep durable build principles here.
- Keep campaign-specific state in dated records.
- Keep durable business learning in `Jary-AI/jary-wiki`.
- Link to source repositories and dated evidence instead of copying large source documents.
- Update `README.md` when adding a major method, design copy or repository reference.

## Completion standard

A change is complete when the design or practice is documented, its source and scope are clear, the internal/public boundary is preserved, links work, the repository has a clean diff check and the change is committed and pushed when explicitly requested.

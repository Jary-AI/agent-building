# Agent Building

An evidence-led build log for designing, operating and improving SDR agents.

## Purpose

Capture reusable experience from real campaign work: campaign contracts, human approval boundaries, research methods, tool limits, QA findings, outcome learning and changes to the agent operating model.

This repository is not a credential store, CRM export, private inbox archive or autonomous sending system.

## Current scope

- Campaign-by-campaign SDR execution.
- Investor, channel-partner and customer motions.
- Portal-led GTM Programs and owned content journeys.
- Human-in-the-loop approval before external communication, publication or CRM mutation.
- Evidence-led learning that can improve the SDR agent without silently widening permissions.

## Initial operating rule

Start with one measurable campaign, one audience cohort, one offer and one result signal. Record what was observed, what changed, what failed and what should be reused before adding volume or automation.

## How the agent works

The SDR agent is a decision preparation system. It reads the current commercial system, chooses one campaign, turns an account or Portal signal into an evidence card, prepares the smallest useful next action, waits for human approval at the external-action boundary, reads the result and promotes only supported learning.

```text
live source
  -> campaign selection
  -> evidence card
  -> method and offer
  -> channel assets
  -> QA and human approval
  -> smallest live action
  -> outcome readback
  -> learning and next decision
```

The agent works because it keeps state visible, uses a bounded campaign contract, separates observation from inference, and treats downstream progress as the success signal. It does not rely on volume, generic personalisation or a large tool count.

## Field manual

- [Agent operating manual](docs/agent-operating-manual.md): the complete model, roles, states, controls and rationale.
- [Internal agent design](docs/agent-design-internal.md): the full internal copy with implementation, tool and control details.
- [Public Academy agent design](docs/agent-design-public.md): the sanitised version prepared for Jary Portal Academy publication.
- [Methodology and reasoning](docs/methodology-and-reasoning.md): when and why to use ABM, Challenger, SPICED, MEDDPICC and the Portal GTM readiness gates.
- [Campaign runbook](docs/campaign-runbook.md): the repeatable step-by-step execution sequence and required artifacts.
- [Tool and data operating model](docs/tool-and-data-operating-model.md): source authority, integration classes, read/write boundaries and handoffs.
- [Suggested tech stack](docs/suggested-tech-stack.md): free-first architecture, current readiness, licensing boundaries and upgrade triggers.
- [Reference repositories](docs/reference-repositories.md): repositories used, authority by question and provenance for this build.
- [QA and learning loop](docs/qa-and-learning-loop.md): evidence quality, failure patterns, outcome metrics and self-improvement rules.
- [Initial build log](docs/2026-10-07-initial-sdr-agent-build.md): the first design decisions.
- [Live Portal readback](docs/2026-10-07-live-portal-readback.md): the observed program inventory and first campaign choice.

## Related system

The operational SDR repository is [`Jary-AI/jary-sdr`](https://github.com/Jary-AI/jary-sdr). This repository captures the agent-building experience and reusable patterns; it does not replace the SDR SOP or the Jary Wiki as the canonical home for durable business learning.

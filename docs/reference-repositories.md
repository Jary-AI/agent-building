# Reference Repositories

This map records the repositories used to ground the SDR agent build. Repository existence and default branches were checked on 2026-10-07 through GitHub. A repository is a source of evidence for a particular question; it is not automatically authoritative for every question.

## Direct references used for this build

| Repository | Role in the build | Authority used |
|---|---|---|
| [`Jary-AI/jary-sdr`](https://github.com/Jary-AI/jary-sdr) | SDR SOP, campaign portfolio, live stack readiness, methodology research, content rules and reusable SDR skill | SDR operating process and dated evidence |
| [`Jary-AI/partner-portal`](https://github.com/Jary-AI/partner-portal) | Portal GTM Program design, readiness gates, enrolment, assets, opportunity flow and campaign surface | Current relationship and GTM operating model |
| [`Jary-AI/product-specifications`](https://github.com/Jary-AI/product-specifications) | Product names, boundaries, feature status and xOS / AskJary+ definitions | What the product is and what it is allowed to claim |
| [`Jary-AI/branding`](https://github.com/Jary-AI/branding) | Brand identity, voice, visual language and claim guardrails | How Jary should present itself |
| [`Jary-AI/marketing`](https://github.com/Jary-AI/marketing) | Audience framing, campaign language, channels, content and CTA direction | Which proposition is adapted for which audience |
| [`Jary-AI/jary-wiki`](https://github.com/Jary-AI/jary-wiki) | Durable cross-workspace learning and accepted operating decisions | Long-lived learning authority |
| [`Jary-AI/agent-building`](https://github.com/Jary-AI/agent-building) | This repository: methodology, agent design rationale, build experience and reusable field notes | How the SDR agent is built and improved |

The repository keeps two copies of the design: [`agent-design-internal.md`](agent-design-internal.md) is the complete operating copy; [`agent-design-public.md`](agent-design-public.md) is the Academy-safe educational copy. The public copy must be reviewed for product claims, language and Portal publication before it is published.

## Supporting product and release references

These repositories were used as the surrounding reference set for product, release and system claims, and should be checked when a campaign depends on their subject matter:

| Repository | Use before making a claim |
|---|---|
| [`Jary-AI/growthos`](https://github.com/Jary-AI/growthos) | GrowthOS product or platform behaviour |
| [`Jary-AI/jary-releases`](https://github.com/Jary-AI/jary-releases) | Whether a feature, product or change is released and publishable |
| [`Jary-AI/jaryai-website`](https://github.com/Jary-AI/jaryai-website) | Public website wording and published surface |
| [`Jary-AI/jary-platform`](https://github.com/Jary-AI/jary-platform) | Shared platform behaviour and boundaries |
| [`Jary-AI/jary-runtime`](https://github.com/Jary-AI/jary-runtime) | Runtime and execution claims |
| [`Jary-AI/jary-ai-employee`](https://github.com/Jary-AI/jary-ai-employee) | AskJary+ / AI Employee implementation claims |
| [`Jary-AI/jary-codex`](https://github.com/Jary-AI/jary-codex) | Codex-specific implementation or integration claims |

## Reference order

Use the repository that owns the question:

```text
Portal / CRM state
  -> product specification
  -> release record
  -> branding
  -> marketing
  -> strategy and SDR interpretation
```

More specifically:

- **What is live?** Check the Portal and release records.
- **What does the product do?** Check product specifications and the owning product repository.
- **What should we say?** Check Branding, then Marketing, then the campaign adaptation in `jary-sdr`.
- **Who is engaged and what happens next?** Check the Portal first, then reconcile HubSpot.
- **What did the agent learn?** Check `jary-wiki`, then the dated SDR and Agent Building notes.

## Conflict rule

When repositories disagree, record the conflict with date and source. Do not merge the wording into a stronger claim. Product specifications cannot be overridden by marketing copy; marketing cannot turn a draft into a release; an SDR hypothesis cannot become a company promise without approval and evidence.

## Local checkout note

Some local folders are working copies, prototypes or historical snapshots. The GitHub repository and the relevant current branch are the reference identity. A local file, branch, demo or unmerged commit can support research, but it cannot independently prove a customer-facing capability.

## Provenance for this build

The immediate source files that shaped the Agent Building manual were:

- `jary-sdr/docs/SDR-SOP.md`;
- `jary-sdr/docs/sdr-agent-design-2026-10-06.md`;
- `jary-sdr/docs/sdr-methodology-research-2026-10-06.md`;
- `jary-sdr/docs/campaign-portfolio-and-execution-plan-2026-10-07.md`;
- `jary-sdr/docs/live-sdr-stack-readiness-2026-10-07.md`;
- `partner-portal/portal/GTM-PROGRAM-DESIGN.md`;
- `partner-portal/portal/KM-STARTER-PACK-GTM-RELEASE-2026-09-29.md`.

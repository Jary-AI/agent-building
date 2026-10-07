# Suggested SDR Tech Stack

**Principle:** use the smallest free or already-owned stack that can prove a campaign result. Add a paid tool only when a measured bottleneck is blocking a valuable, consented motion.

## Recommended architecture

```text
Jary Portal
  source of truth for programs, content, intent and opportunities
        |
        +--> Codex / SDR agent
        |      research, evidence cards, drafts, QA, approval packets, learning
        |
        +--> Gmail + Calendar + Drive
        |      human relationship work, scheduling and approved evidence
        |
        +--> Brevo
        |      opted-in news and nurture
        |
        +--> Metricool / native social
        |      public proof, approved publishing and measurement
        |
        +--> HubSpot
               manual downstream reconciliation after human acceptance

GitHub + Jary Wiki
  versioned SOP, product/brand sources, agent build records and durable learning
```

## Stack recommendation by stage

| Stage | Use | Recommended tool | Current status | Upgrade trigger |
|---|---|---|---|---|
| 1. Source of truth | GTM Programs, assets, subscriptions, bookings, opportunities and support | Jary Portal | Live working source | Improve the Portal when relationship state or program readiness is unclear |
| 2. Agent workspace | Research, evidence cards, drafts, QA, campaign records and reasoning | Codex + `Jary-AI/jary-sdr` | Live | Add a UI only when campaign state cannot be reviewed in files and Portal |
| 3. Account research | Named-account and role research | Apollo Free or approved public/company sources | Apollo available, not connected | Connect only when manual research is the demonstrated bottleneck |
| 4. Relationship email | One-to-one, approved follow-up and replies | Gmail on the authorised Jary domains | Connected; draft-first | Add sequencing only after a consented cohort and a repeatable offer exist |
| 5. Meetings | Availability, booking and follow-up | Google Calendar + Portal booking | Connected/readable | Improve when booking friction is evidenced in the funnel |
| 6. Evidence store | Approved decks, product specs, marketing and account materials | Google Drive + GitHub | Connected/readable | Add retrieval/indexing only when source discovery is the bottleneck |
| 7. Opt-in nurture | News, Academy and content subscriptions | Brevo Free | Connected; sender active; list needs audience growth | Pay when a valuable consented list or automation limit is reached |
| 8. Social publishing | Public proof, channel tests and analytics | Metricool, with native publishing fallback | Connected to Facebook, Instagram and LinkedIn; current account readback required per campaign | Upgrade when collaboration, reporting or channel limits block a measured campaign |
| 9. CRM reconciliation | Accepted opportunity, owner, stage, task and history | HubSpot Free | Connected/readable; onboarding/tasks remain | Extend only after Portal-to-CRM manual sync is verified and volume justifies it |
| 10. Version and learning | SOP, prompts, skills, evaluation fixtures, build experience | GitHub + Jary Wiki | GitHub live; Wiki is durable learning authority | Automate maintenance only after review and validation are stable |
| 11. Creative production | Campaign visuals and layouts | Existing Jary deck/HTML workflow; Canva after connection if needed | Canva not connected | Connect Canva when repeatable creative production is a measured constraint |

## Free-first pilot

The first market test can run with:

- Jary Portal;
- Codex;
- GitHub;
- Gmail;
- Google Calendar and Drive;
- HubSpot Free for manual reconciliation;
- Brevo Free for opted-in nurture;
- Metricool or native social publishing;
- public company research and a small manually approved account cohort.

Apollo and Canva remain optional additions. Their availability does not make them necessary for the first campaign.

## Licensing and data boundaries

- Jary Portal, GitHub repositories and Jary-authored content remain subject to their owners' access and licence rules.
- SaaS tools provide a service under their terms; they do not grant the right to copy third-party data, scrape social profiles, resell enrichment or ignore consent.
- Apollo data is a research input, not proof of consent, authority or buying intent.
- Brevo is for consent-based communication; an imported list must have a documented lawful basis and suppression path.
- LinkedIn, Instagram and Threads require official or native routes; browser scraping and unofficial engagement automation are excluded.
- Customer data, private email bodies, credentials, tokens and contact exports stay outside this repository.

## Acceptance test before a tool is called ready

1. Confirm the account and permission scope.
2. Run one read-only call or UI readback.
3. Confirm the tool's state against the source of truth.
4. Create a draft or sandbox artifact where possible.
5. Verify the artifact independently.
6. Record the result, limitation and date.
7. Apply human approval before sending, publishing, syncing or changing lifecycle state.

## Tool selection rule

Choose a tool only when it improves one named campaign decision:

```text
observed bottleneck
  -> smallest tool capability that addresses it
  -> read-only acceptance test
  -> draft-only trial
  -> measured live use
  -> retain, replace or remove
```

This keeps the stack subordinate to campaign learning. A larger stack is not evidence of a better SDR agent.

## References

The detailed licensing and plan research is maintained in [`Jary-AI/jary-sdr/docs/sdr-tech-stack-research-2026-10-06.md`](https://github.com/Jary-AI/jary-sdr/blob/main/docs/sdr-tech-stack-research-2026-10-06.md). Current connection state is maintained in the dated readiness note in the SDR repository.

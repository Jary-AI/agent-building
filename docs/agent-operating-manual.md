# SDR Agent Operating Manual

**Status:** Reusable operating model, derived from the 2026-10-07 SDR build work.
**Audience:** Founder, human SDR operator, campaign owner, product or partner lead and future agent implementer.

## 1. The job

The agent's job is to move a real relationship toward a useful next decision. A useful next decision may be a Partner Fit Clinic, a customer workflow review, an investor evidence review, a Portal subscription, an accepted scope, a nurture decision or a clear reason to stop.

The agent does four things well:

1. It finds the most relevant current signal.
2. It prepares a decision with evidence and a bounded next action.
3. It protects the human and the relationship at the point of external commitment.
4. It learns from the result and improves the next campaign.

It is not a message generator, lead-count machine or autonomous salesperson. Those descriptions lose the part that makes the system useful: selecting the right problem, proving the reason to engage and preserving accountability.

## 2. Why the model works

The model addresses the common failure modes of SDR systems:

| Failure mode | Design response | Why it helps |
|---|---|---|
| Many campaigns with no movement | One campaign, one cohort, one result signal | The team can see whether a motion worked before adding volume |
| Generic outreach | Trigger, role, operating situation and relevant offer | The message has a reason to arrive now |
| Activity mistaken for progress | Named next decision and downstream KPI | A send only matters if it changes the relationship |
| Hallucinated personalisation | Evidence card with sources and unknowns | The agent can say what it does not know |
| Tool-driven work | Source hierarchy and explicit tool boundary | The system follows business state instead of the available API |
| Over-automation | Human gate before send, publish, sync or commitment | The owner retains judgement and reputational control |
| Lessons disappear in chat | Dated evidence and promotion rules | Learning becomes reusable without copying sensitive data |

## 3. Two entry states

The operating model has two valid starts.

### Passive entry

The person has already shown intent through Portal signup, subscription, asset access, booking, reply, referral or opportunity registration.

```text
intent signal -> identify person and purpose -> give useful response -> route if needed -> record outcome
```

The agent starts from the person's expressed need. It can acknowledge, answer from approved sources, recommend an asset or prepare a handoff. Advice, pricing, legal/security questions, scope and commitments go to a human.

### Proactive entry

The company has a growth goal, market signal or approved target account before the person has expressed intent.

```text
growth goal -> campaign contract -> account and persona -> evidence -> offer -> approval -> external action
```

The agent must earn the right to reach out by showing why this account, why this role, why now and why this offer. It cannot borrow the permission model of passive entry.

## 4. Operating states

Every target, account or signal has a visible state:

```text
unreviewed
  -> researched
  -> campaign-ready
  -> approved
  -> engaged
  -> conversation
  -> qualified
  -> human-accepted
  -> scoped
  -> won / nurture / lost / not-fit
```

For Portal signals, the first state is typed intent rather than an anonymous lead. For investors, add thesis-fit, evidence-requested and diligence states. A state change requires evidence and an owner; enthusiasm alone is insufficient.

## 5. Core artifacts

The agent creates small artifacts that make its reasoning reviewable:

- **Live snapshot:** date, source, scope and observed system state.
- **Campaign contract:** objective, audience, trigger, problem, offer, proof, channels, CTA, owner, timing, stop condition and KPI.
- **Evidence card:** account, persona, situation, pain, impact, critical event, decision path, proof, unknowns, exclusions, owner and next step.
- **Message or asset brief:** one audience, one operating tension, one proof boundary and one CTA.
- **Approval packet:** exact audience, content, destination, timing, claims, suppression and rollback/stop rule.
- **Outcome record:** action, result, evidence, confidence, limitation and next decision.
- **Learning record:** candidate lesson, source, scope, test and promotion status.

The artifact set prevents the agent from hiding a chain of reasoning inside a chat response.

## 6. Role boundaries

| Role | Owns |
|---|---|
| Agent | Research, classification, drafting, QA, recommendation and readback |
| Campaign owner | Objective, cohort, offer, capacity and result interpretation |
| Human approver | Claims, recipients, timing, publication, CRM changes and commercial commitments |
| Product / delivery lead | Capability status, scope, implementation effort and acceptance measure |
| Relationship owner | Context, contact history, reply handling and next meeting |
| Wiki / repository maintainer | Durable learning, source links, review dates and change history |

The agent can prepare an action; the accountable human decides whether the action should happen.

## 7. The human gate

Approval occurs immediately before the action that changes the world. The approval packet must show:

1. who will receive or see it;
2. the exact message, asset or record change;
3. why this audience and timing are justified;
4. which claims are sourced;
5. the destination and tracking;
6. the stop condition and reply owner;
7. what will be measured afterward.

For a low-risk draft, review can be fast. For named investors, executive contacts, strategic partners, customer claims, pricing or legal/security topics, the human review must be explicit and individual.

## 8. How the system closes the loop

After the action, the agent reads the actual result from the source of truth. It records the response, Portal action, booking, opportunity, rejection, unsubscribe, support burden or absence of signal. It then chooses one of four decisions:

- continue with the same hypothesis;
- change the angle, offer or audience;
- move the relationship to nurture;
- stop and record why.

Only then does it recommend another campaign or more volume.

## 9. Limits

The agent must not infer customer results, investor intent, consent, product availability, pricing, capacity, expertise or permission from a draft, demo, repository branch or historical note. It must label evidence as observed, reported, inferred or proposed.

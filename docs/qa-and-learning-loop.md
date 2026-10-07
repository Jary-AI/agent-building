# QA and Learning Loop

## 1. Quality model

The agent is judged on four layers:

| Layer | Question | Evidence |
|---|---|---|
| Truth | Is the claim supported and current? | Source, date and evidence label |
| Fit | Is this the right account, role, trigger and offer? | Evidence card and campaign contract |
| Experience | Can the person understand and act on it? | Readability, permissions, links and response path |
| Outcome | Did the action create the intended next decision? | Portal, channel, CRM and human readback |

Passing one layer does not compensate for failing another. A beautiful post with no fit is weak; a qualified account with a broken Portal path is also weak.

## 2. Failure patterns and corrections

| Observed failure | Root cause | Correction |
|---|---|---|
| Same template repeated across channels | Channel was treated as the strategy | Keep the claim and offer stable, then redesign the channel role and creative form |
| Campaigns started from a tool | Tool availability replaced commercial selection | Read Portal programs and pipeline first |
| Large product catalogue in the first message | Product description replaced buyer problem | Lead with one operating situation and one useful next action |
| Unfinished job used as a universal pain | A real concept was over-generalised | Test sharper alternatives: decision latency, evidence gaps, exception ownership, adoption or cost substitution |
| Portal signup treated as qualified opportunity | Passive intent and commercial acceptance were collapsed | Route, give value and ask for human qualification |
| Social reach used as success | Intermediate activity was mistaken for business movement | Track useful Portal action, conversation, scope and proof |
| Live capability inferred from repo or demo | Source hierarchy was ignored | Require current release or Portal evidence |
| HubSpot treated as primary truth | CRM was updated without relationship verification | Keep Portal authoritative and sync manually |
| Too many tools before one validated offer | Stack breadth hid a weak hypothesis | Run a smallest useful campaign with the available stack |
| Agent asked for permission too early | Planning and external action were mixed | Prepare a complete, reviewable packet first; ask only at the action boundary |

## 3. Learning record

After each meaningful campaign or user correction, write:

```text
Date and campaign:
Expected result:
Action taken:
Observed result:
Evidence links:
What changed:
Confidence:
Limitation:
Next experiment:
Promotion scope: turn / task / workspace / skill
Review date:
```

## 4. Promotion rules

- **Turn:** useful only for the current response.
- **Task:** applies to the current campaign or review.
- **Workspace:** reusable across Jary work after review; publish to the Jary Wiki.
- **Skill:** changes the agent instructions or supporting resources; requires an explicit, reviewable approval before changing the skill file.

A lesson can be promoted when the user explicitly corrects or endorses it, the same pattern appears in at least two comparable cases with evidence, or a controlled comparison shows meaningful improvement. A plausible tactic remains a hypothesis.

## 5. Metrics that matter

Track the full path:

```text
approved cohort
  -> meaningful reach
  -> useful engagement
  -> Portal action
  -> human conversation
  -> qualified opportunity
  -> accepted scope or evidence step
  -> value / repeatability / support burden
```

Also track side effects: unsubscribes, negative replies, claim corrections, privacy issues, founder time, delivery effort and opportunities that should have been stopped earlier.

## 6. Why self-improvement remains controlled

The agent may update task notes and propose a better next test. Durable learning belongs in the Jary Wiki; this repository keeps the agent-building method and evidence references. Learning cannot grant access, approve claims, send messages, publish, change pricing, sync CRM or silently edit the skill.

The improvement loop is:

```text
observe -> record -> compare -> propose -> approve -> change one thing -> verify -> retain or roll back
```

That loop makes the agent more capable without allowing an accidental success, a persuasive story or a single noisy metric to rewrite the operating rules.

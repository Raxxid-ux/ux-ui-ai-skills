---
name: ux-research-insights-intermediate
description: Synthesizes UX research into insights with rigor — weighting evidence strength, spotting contradictions, and stress-testing conclusions before they drive design decisions. Use when you already know the basic affinity-mapping method and need to go deeper — validating insights, resolving conflicting data, or defending research findings to stakeholders.
level: intermediate
---

# UX Research Insights (Intermediate)

This assumes you already know basic synthesis: collect raw data, group it, name the pain, suggest a direction. That method gets you a first-pass insight. This version adds what most beginner processes skip — checking whether that insight is actually trustworthy before you build a whole design decision on it.

## Why this level exists
The beginner method treats every insight as equally solid. In real projects, that's dangerous — a strong opinion from one loud user can get treated the same as a pattern seen across twenty people. This method adds rigor at each step so weak patterns don't get promoted to "the truth" by accident.

## Step 1 — Collect and tag evidence strength
As you collect data points, tag each one by how reliable it is:
- **Direct observation** (you watched it happen) — strongest. People's actions are more honest than their words.
- **Self-reported** (someone told you in an interview or survey) — moderate. People misremember, want to sound good, or answer what they think you want to hear.
- **Inferred** (you're guessing based on indirect signals, like a support ticket or a one-line review) — weakest. Treat this as a hypothesis to test, not a confirmed fact.

Don't build a major design decision on inferred-only evidence. It's fine as a starting hunch, but go find stronger evidence before committing.

## Step 2 — Group, then actively look for contradictions
Group your data as usual. But this time, don't just look for agreement — actively hunt for data points that contradict each other, either inside one group or between two groups.

Contradictions are not noise to throw away. They usually mean you're looking at two different types of users who need different things, not one confused pattern. If you find a real contradiction, split that group into two and treat them separately.

*Example:* Some users say they want more notifications to stay on track, others say notifications feel like nagging. That's not one group with mixed feelings — it's likely two different user types with different self-control styles, and they may need different settings, not one universal decision.

## Step 3 — Insight statement with a confidence level
Write the insight the same way as before, but now add a confidence rating and your reasoning for it:

`People feel [emotion] when [situation] because [reason]. — Confidence: [low/medium/high], based on [how many sources / what kind of evidence].`

A single self-reported quote from one person is low confidence. The same pattern showing up across five or more direct observations, or repeated consistently across many interviews, is high confidence. Being honest about this saves you from overbuilding around a shaky finding.

## Step 4 — Stress-test before you commit
Before you treat a high-confidence insight as settled, ask yourself three questions:
- **What would disprove this?** Have I actually looked for evidence against it, or only gathered evidence that supports what I already believed?
- **Is this about the product, or about one person's specific life situation?** Some pain points are real but rare — a one-off circumstance, not a pattern worth designing around.
- **If I showed this insight to the actual users, would they nod and agree, or would they say "that's not quite it"?** If you're not sure, that's a sign to go check with a real person before moving forward.

## Step 5 — Direction with tradeoffs named
Don't just suggest a direction — name what it costs, so whoever reads this (including future you) can make an informed call, not just follow blindly.

*Example:* "Direction: make the first step of the app anonymous, so people don't feel judged early on. Tradeoff: this reduces the personal data you collect early, so personalization may need a second opt-in step later, and you lose some early context about who the user is."

## Common mistakes at this level
- **Treating a loud minority as a majority pattern.** Always check how many actual sources support a finding before acting like it's the dominant user need.
- **Confirmation bias.** It's easy to keep collecting more evidence for a pattern you already like the sound of, instead of actively checking for the data that contradicts it.
- **Skipping confidence levels when presenting findings.** Without them, a weak, one-person hunch looks exactly as solid as a well-supported pattern to whoever you're presenting to — and that leads to bad decisions downstream.

## Checklist
```
[ ] Evidence tagged by strength (direct / self-reported / inferred)
[ ] Contradictions actively checked, segments split where needed
[ ] Each insight has a confidence level and stated reasoning
[ ] Each high-confidence insight stress-tested against disproof
[ ] Direction includes named tradeoffs, not just the upside
```

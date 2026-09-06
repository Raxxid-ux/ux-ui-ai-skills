---
name: critique-design-intermediate
description: Gives rigorous, systems-level design critique that evaluates decisions against user goals, business constraints, and design-system consistency — not just surface polish. Use when you need to critique a design that's already functionally fine, and want to catch deeper issues like flawed assumptions, edge cases, or scalability problems before it ships.
level: intermediate
---

# Critique a Design (Intermediate)

This assumes the design already passes basic checks — clear hierarchy, decent spacing, readable contrast. At this level, critique moves from "is this screen well-made" to "is this the right screen, built in a way that holds up." Surface-level polish stops being the interesting question; the assumptions underneath the design become the interesting question.

## Critique across four layers, not just one screen

**1. Assumption layer**
What is this design assuming about the user that hasn't actually been confirmed? Every screen makes silent assumptions ("users will read this label," "users know what this icon means," "users will have the app open when this matters"). Name the assumptions and ask which ones are genuinely risky if wrong.

**2. Goal-fit layer**
Does this design actually solve the user goal it claims to solve, or does it solve an adjacent, easier problem instead? It's common for a design to look complete while quietly avoiding the hardest part of the actual problem.

**3. Edge case layer**
What happens when things aren't ideal — empty states, error states, very long or very short content, slow network, a user who's new vs. a returning user? A design that only works in the "happy path" screenshot isn't finished. Ask specifically: what does this look like on someone's worst day using it, not their best?

**4. System layer**
Does this design fit consistently with the rest of the product, or does it quietly introduce a new pattern that conflicts with existing ones (a new button style, a new spacing rule, a new interaction model)? One-off exceptions accumulate into an inconsistent product over time.

## How to structure the critique
Same discipline as beginner level — one main issue at a time, always paired with a fix — but the *source* of the issue is now allowed to be structural, not just visual. Example: "The main issue isn't the button placement, it's that this flow assumes users already understand what the feature does — which hasn't been validated. Fix: add a one-line explainer before this step, or test this assumption with 3-5 users before investing further in this flow."

## Common mistakes at this level
- Critiquing only what's visible on screen and ignoring what happens in edge cases or failure states.
- Accepting a design's stated goal at face value instead of checking if it actually addresses the real user problem.
- Giving feedback that conflicts with the existing design system without acknowledging the tradeoff of introducing a new pattern.
- Being so focused on structural critique that basic usability issues get missed — check both levels, not just the advanced one.

## Checklist
```
[ ] Assumptions the design relies on are named and evaluated
[ ] Design checked against the actual user goal, not just the stated one
[ ] Edge cases and non-ideal states considered, not just the happy path
[ ] Consistency with the existing design system checked
[ ] Feedback still ends in one clear, prioritized fix
```

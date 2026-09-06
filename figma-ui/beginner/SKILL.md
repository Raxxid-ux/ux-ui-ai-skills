---
name: build-ui-in-figma-beginner
description: Step-by-step guidance for building a UI screen or component in Figma, covering layout order, spacing, and basic color/typography rules. Use when you're new to Figma and need a clear build order instead of guessing where to start, or when a screen feels messy and you're not sure why.
level: beginner
---

# Build UI in Figma (Beginner)

Figma has no fixed order to build in, which is exactly why beginners often end up with messy files — colors added before layout is settled, text sized randomly, spacing that "looks fine" but isn't consistent. This skill gives you one fixed order to follow every time, so structure always comes before decoration.

## Why order matters
If you pick colors and fonts before the layout is solid, you'll keep re-doing work every time the layout changes. Structure first, style second — always in that order.

## Default rules to start with
- Favor generous white space over cramming things in. A clean screen with fewer elements usually looks more professional than a busy one.
- Use a consistent spacing scale — pick multiples of 4px or 8px (8, 16, 24, 32...) for gaps and padding. Don't use random numbers like 13px or 22px.
- Stick to one primary color for buttons/actions, one neutral gray scale for text/backgrounds, and use extra colors sparingly.

## Step-by-step build order
```
[ ] Step 1: Set the frame size (decide mobile ~375x812 or desktop ~1440 width)
[ ] Step 2: Block out the layout with plain rectangles/frames — no real content yet, just structure
[ ] Step 3: Add real content (text, icons, images) into the blocked structure
[ ] Step 4: Apply your spacing scale (4px or 8px multiples) and align everything
[ ] Step 5: Apply color and typography
[ ] Step 6: Turn any repeating structure (like a card or list item) into a reusable component
```
Don't jump to Step 5 or 6 before Step 1-4 are done. It's tempting to make things pretty early, but it causes rework later.

## What is Auto Layout, and why use it
Auto Layout is a Figma feature that automatically manages spacing and alignment for you, instead of you manually dragging each element into place. Use it for anything that repeats (like a list of cards, or a row of buttons) — manually placing repeating elements is the most common cause of messy, hard-to-edit files.

## Common mistakes
- Designing colors and fonts before the layout structure is settled.
- Using random spacing values instead of a consistent scale.
- Manually positioning repeating elements instead of using Auto Layout.
- Adding too many colors or fonts, which makes the design feel busy instead of clean.

## Checklist
```
[ ] Frame size decided
[ ] Layout structure blocked out first
[ ] Real content added into the structure
[ ] Spacing scale applied consistently
[ ] Color and type applied last
[ ] Repeating elements turned into components
```

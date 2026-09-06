---
name: design-fundamentals-intermediate
description: Advanced typography and color decisions covering type systems, accessible contrast ratios, semantic color roles, and how to make these choices systematically rather than one screen at a time. Use when building or auditing a design system's type and color foundation, or when basic type/color choices already work and you need them to scale consistently across a whole product.
level: intermediate
---

# Design Fundamentals: Typography and Color (Intermediate)

This assumes you already know basic type scales and simple palettes. At this level, the goal shifts from "does this screen look good" to "does this system hold up consistently across dozens of screens, states, and future additions."

## Typography as a system, not a scale

### Modular scale, not arbitrary sizes
Instead of picking sizes that "feel right" one at a time, use a consistent ratio between steps (e.g. each size is roughly 1.25x the previous one). This keeps the whole scale feeling mathematically related instead of arbitrary, and makes it predictable to add new sizes later without breaking the rhythm.

### Semantic naming, not just sizes
Don't name your text styles "24px" or "18px" — name them by role: `heading-page`, `heading-section`, `body-primary`, `body-secondary`, `label`. This means when the underlying size needs to change (a common redesign step), you update the definition once instead of hunting down every "24px" text layer across the product.

### Optical adjustments
Font size alone isn't the full story — different fonts at the "same" size can look different in actual visual weight. When pairing fonts, check them side by side at real sizes, not just by their numbers, and adjust weight or size slightly if one font is visually louder than the other at a supposedly equal size.

## Color as a system

### Semantic color roles, not just brand colors
Beyond primary/neutral/accent, a scalable system needs functional roles: `success`, `warning`, `error`, `info`, `disabled`. Define these separately from your brand palette, and make sure they don't visually clash or get confused with brand colors that happen to be similar (e.g. don't let your brand's orange be mistaken for a warning state).

### Accessible contrast, checked with numbers
"Looks readable" isn't reliable enough at this level — check actual contrast ratios. Body text against its background should meet at least a 4.5:1 contrast ratio; larger text (headings) can go as low as 3:1. Use a contrast-checking tool rather than judging by eye, since screens and lighting vary a lot between people.

### Color in dark mode / multiple themes
If the product might need a dark mode or multiple themes, define colors as roles (`background`, `surface`, `text-primary`) that map to different actual values per theme, rather than hardcoding one fixed hex value everywhere. This is far easier to set up early than to retrofit later.

## Common mistakes at this level
- Defining type/color by literal value (a size, a hex code) instead of by semantic role, which makes systemwide changes painful.
- Skipping numeric contrast checks and relying only on visual judgment, which misses real accessibility issues.
- Letting brand colors and functional colors (like error/warning) overlap or get confused.
- Building a highly systematic type/color architecture for a project too small to need it — match the system's complexity to the project's actual scale and lifespan.

## Checklist
```
[ ] Type scale follows a consistent ratio, not arbitrary sizes
[ ] Text styles named by role, not by raw size
[ ] Font pairing checked visually at real size, not just by number
[ ] Semantic color roles (success/warning/error/etc.) defined separately from brand colors
[ ] Contrast ratios checked numerically, not just by eye
[ ] Color roles set up to support theming if that's a future possibility
```

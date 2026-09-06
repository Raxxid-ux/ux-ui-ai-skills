---
name: build-ui-in-figma-intermediate
description: Advanced Figma workflow guidance covering component architecture, variants, design tokens, and file organization for scalable design systems. Use when you already know basic layout/spacing and need to structure a file that other people (or future you) can maintain, extend, or hand off to developers.
level: intermediate
---

# Build UI in Figma (Intermediate)

This assumes you already know the basics: frame setup, spacing, Auto Layout, and simple components. This version is about building files that scale — that stay organized as a project grows past a handful of screens, and that don't collapse into chaos when someone else (or future you) has to work in them.

## Component architecture, not just components
A single component is easy. The hard part is structuring a *system* of components that don't fight each other.

- **Base components** should hold only the smallest reusable unit (a single button, a single input field) — not entire sections.
- **Composed components** combine base components (a form = multiple input fields + a button). Don't duplicate a base component's styling inside a composed one — reference the base component instead.
- Before building a new component, check if an existing one can be extended with a variant instead of creating a near-duplicate. Duplicate components with tiny differences are the #1 cause of design-system drift.

## Variants over duplicates
Use Figma variants (button: primary/secondary/disabled, size: small/large) instead of making separate components for each state. This keeps the file smaller and keeps every state properly linked — so a change to the base design updates everywhere at once.

## Design tokens (colors, spacing, type as variables)
Instead of hardcoding hex values or font sizes directly onto elements, define them once as styles or variables (color styles, text styles, spacing variables) and apply those everywhere. This means a brand color change is one edit, not a hundred manual fixes across every screen.

## File organization for handoff
```
[ ] Pages separated by purpose (e.g. "Cover," "Components," "Screens," "Archive")
[ ] Components page kept clean — one clear source of truth, not scattered duplicates
[ ] Layers named clearly (not "Frame 47" — name it what it actually is)
[ ] Consistent naming convention across components (e.g. Button/Primary/Large)
[ ] Redundant or abandoned exploration moved to an Archive page, not left cluttering the main file
```

## Common mistakes at this level
- Building near-duplicate components instead of using variants — this creates drift where fixing one doesn't fix the others.
- Hardcoding colors/spacing instead of using shared styles or variables, making global changes painful.
- Messy layer names and unclear file structure, which makes handoff to developers slow and error-prone.
- Over-engineering a design system for a small project — not every project needs full token architecture. Match the system's complexity to the project's actual size and lifespan.

## Checklist
```
[ ] Component library uses variants, not duplicate components
[ ] Colors, spacing, and type use shared styles/variables
[ ] File pages organized clearly by purpose
[ ] Layers and components named descriptively
[ ] System complexity matches project size — not over-built
```

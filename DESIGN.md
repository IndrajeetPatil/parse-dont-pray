---
version: alpha
name: Parse, Don't Pray
description: >-
  Type-safe data validation presentation design: clean white canvas, dual
  Pydantic pink and Zod blue branding, semantic pastel cards, and
  colorblind-friendly callouts.
colors:
  primary: "#e92063"
  secondary: "#3e67b1"
  bg-canvas: "#ffffff"
  text: "#222222"
  muted: "#666666"
  pydantic: "#e92063"
  zod: "#3e67b1"
  callout-tip: "#7570b3"
  callout-caution: "#e6ab02"
  card-blue: "#e3f2fd"
  card-green: "#e8f5e9"
  card-orange: "#fff3e0"
  card-red: "#ffebee"
  card-yellow: "#fffbc1"
  table-code-bg: "#f8f9fa"
  code-highlight: "#fff8e1"
typography:
  display:
    fontFamily: News Cycle, Impact, sans-serif
    fontSize: 1.3em
    fontWeight: 700
  heading:
    fontFamily: News Cycle, Impact, sans-serif
    fontSize: 1.1em
    fontWeight: 700
  body:
    fontFamily: News Cycle, sans-serif
    fontSize: 32px
    fontWeight: 400
  mono:
    fontFamily: monospace
rounded:
  sm: 4px
  md: 10px
  lg: 15px
  pill: 25px
components:
  page:
    backgroundColor: "{colors.bg-canvas}"
    textColor: "{colors.text}"
  card-pydantic:
    backgroundColor: "{colors.bg-canvas}"
    borderColor: "{colors.pydantic}"
    rounded: "{rounded.lg}"
  card-zod:
    backgroundColor: "{colors.bg-canvas}"
    borderColor: "{colors.zod}"
    rounded: "{rounded.lg}"
  card-goal:
    backgroundColor: "{colors.card-yellow}"
    rounded: "{rounded.pill}"
  card-info:
    backgroundColor: "{colors.card-blue}"
    rounded: "{rounded.md}"
  card-success:
    backgroundColor: "{colors.card-green}"
    rounded: "{rounded.md}"
  card-warning:
    backgroundColor: "{colors.card-orange}"
    rounded: "{rounded.md}"
  card-error:
    backgroundColor: "{colors.card-red}"
    rounded: "{rounded.md}"
---

# DESIGN.md

The visual design specification of the Parse, Don't Pray presentation deck.

## Overview

The visual design is built around the dual themes of Python's Pydantic and TypeScript's Zod data validation ecosystems on a crisp, light presentation canvas. It pairs the high-contrast RevealJS `simple` theme with distinctive brand accents (Pydantic pink `#e92063` and Zod blue `#3e67b1`), semantic pastel card containers, and ColorBrewer-inspired colorblind-friendly callouts.

The presentation format is Quarto RevealJS (`theme: simple`). Custom styles are defined in `style.css` and mirrored in the front matter above.

## Colours

- **Canvas & Typography:**
  - `bg-canvas` (`#ffffff`): Clean white canvas background across all slides.
  - `text` (`#222222`): High-contrast dark charcoal text.
  - `muted` (`#666666`): Secondary metadata, slide footers, and diagram connector links.
- **Library Accents:**
  - `pydantic` (`#e92063`): Signature pink accent used for Pydantic headers, comparison cards, and Python validation highlights.
  - `zod` (`#3e67b1`): Signature blue accent used for Zod headers, comparison cards, and TypeScript validation highlights.
- **Semantic Pastel Cards:**
  - `card-yellow` (`#fffbc1`): High-priority goal statements and core thesis highlights.
  - `card-blue` (`#e3f2fd`): Informational context, stack assumptions, and type-system takeaways.
  - `card-green` (`#e8f5e9`): Parsing wins, validation benefits, and robust runtime patterns.
  - `card-orange` (`#fff3e0`): Runtime friction, caveats, and boundary migration hazards.
  - `card-red` (`#ffebee`): Unvalidated risks, silent type coercion bugs, and security pitfalls.
- **Callout Palette:**
  - `callout-tip` (`#7570b3`): Purple left border and 15% opacity tinted background for tips and recommended patterns.
  - `callout-caution` (`#e6ab02`): Gold left border and 15% opacity tinted background for caveats and warnings.

## Typography

- **Headings & Body:** Default RevealJS `simple` theme sans-serif typography (`News Cycle`, `Impact`, sans-serif).
- **Code:** Monospace stack for Python and TypeScript schemas, validation rules, and JSON payloads.
- **Comparison Tables:** Nested code blocks in `.smaller` slides render with a light background (`#f8f9fa`), 4px rounded corners, and word wrapping.
- **Line Highlights:** Selected code lines highlight with `#fff8e1` while maintaining full opacity on surrounding code.

## Layout & Components

- **Library Comparison Cards:** Fenced divs styled with a white background, 2px solid border (`#e92063` for Pydantic or `#3e67b1` for Zod), 15px border radius, and a subtle card shadow (`0 4px 6px rgba(0,0,0,0.1)`).
- **Goal Cards:** Centred pill-shaped containers with `#fffbc1` background and 25px border radius.
- **Callouts:** Full-width Quarto callout blocks customized with ColorBrewer-derived purple and gold tints.
- **Icons:** Inline SVG mask spans (`.deck-icon`) powered by Font Awesome Free path data in `currentColor`.

## Do's and Don'ts

- **Do** retain `theme: simple` in `index.qmd` front matter.
- **Do** use `#e92063` for Pydantic elements and `#3e67b1` for Zod elements to preserve brand recognition.
- **Do** reuse the established semantic pastel colours for card containers.
- **Don't** introduce dark canvas backgrounds or high-saturation backgrounds that reduce text readability.

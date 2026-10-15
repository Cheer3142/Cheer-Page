---
name: Obsidian Observatory
description: The shared visual system of cerosoft.net and Cheer's portfolio — CeroSoft's obsidian, ivory, champagne and cyan, carrying the portfolio's night sky.
colors:
  obsidian-950: "#080d10"
  obsidian-900: "#0c1216"
  obsidian-850: "#121a20"
  obsidian-800: "#19232a"
  slate-700: "#263139"
  mist-400: "#9ca7a9"
  silver-200: "#d9dcda"
  ivory-50: "#f8f7f3"
  ivory-100: "#f0eee8"
  ivory-200: "#e3e1da"
  stone-300: "#d3d0c6"
  ink-900: "#182127"
  ink-600: "#56626a"
  cyan-400: "#18bcc4"
  cyan-500: "#08a5ad"
  cyan-700: "#066f74"
  champagne-300: "#c9bc9e"
  bronze-700: "#6e5f3d"
  night-ink: "#e9eae7"
  night-ink-soft: "#c5cbca"
  night-muted: "#b5bdbe"
  plate: "#ffffff"
typography:
  display:
    fontFamily: "DM Sans, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "clamp(42px, 6.6vw, 68px)"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "DM Sans, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "clamp(34px, 4.4vw, 48px)"
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: "-0.035em"
  title:
    fontFamily: "DM Sans, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 500
    lineHeight: "30px"
    letterSpacing: "-0.025em"
  body:
    fontFamily: "DM Sans, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: "26px"
  label:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "11px"
    fontWeight: 600
    lineHeight: "18px"
    letterSpacing: "0.22em"
  numeral:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "30px"
    fontWeight: 400
    lineHeight: "28px"
  data:
    fontFamily: "IBM Plex Mono, ui-monospace, monospace"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: "18px"
    letterSpacing: "0.04em"
rounded:
  sm: "2px"
  md: "3px"
  lg: "4px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "48px"
  section: "88px"
components:
  button-primary:
    backgroundColor: "{colors.cyan-500}"
    textColor: "{colors.obsidian-900}"
    rounded: "{rounded.sm}"
    height: "48px"
    padding: "0 22px"
  button-primary-hover:
    backgroundColor: "{colors.cyan-400}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.sm}"
    height: "48px"
    padding: "0 22px"
  tag:
    backgroundColor: "{colors.obsidian-850}"
    textColor: "{colors.mist-400}"
    rounded: "{rounded.sm}"
    padding: "3px 10px"
  card:
    backgroundColor: "{colors.obsidian-850}"
    rounded: "{rounded.lg}"
  product-stage:
    backgroundColor: "{colors.ivory-200}"
    textColor: "{colors.ink-900}"
    rounded: "{rounded.lg}"
    padding: "44px"
  deep-band:
    backgroundColor: "{colors.obsidian-950}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.lg}"
    padding: "44px"
---

# Design System: Obsidian Observatory

Source of truth for values: [`tokens.css`](tokens.css). Live specimen: [`design-system.html`](design-system.html).

## Overview

Two sites, one world. **cerosoft.net** is a studio at night: obsidian rooms, ivory daylight sections, champagne hairlines that read like engraved metal, and a single cyan signal for "act here". **The portfolio** is an observatory: a drifting star field, instruments, telescopes. The fusion keeps CeroSoft's materials and discipline and lets the portfolio keep its sky — the stars are now silver with a few champagne ones, and the portrait sits inside CeroSoft's orbit ring with its slowly turning cyan arc.

Tone: precise, quiet, expensive. Nothing glows that isn't an action. Edges are almost square. Lines do the work that shadows do elsewhere.

Night (obsidian) is the primary theme. Day is not an inversion; it is CeroSoft's ivory, with bronze replacing champagne and deep cyan replacing bright cyan so text keeps AA contrast.

## Colors

Three families and one rule for each.

### Primary — Signal Cyan
`cyan-500 #08a5ad` fills primary buttons, focus rings and the active nav underline. `cyan-400 #18bcc4` is cyan as **text** on obsidian (links, organisation names, accent words in headings); `cyan-700 #066f74` is the same role on ivory (5.1:1 on `ivory-100`).

### Secondary — Champagne
`champagne-300 #c9bc9e` is metal, not paint: hairlines (`--line-lux`, 22% alpha), the rule in front of every label, dates, stat numerals, publication years. On ivory, champagne text becomes `bronze-700 #6e5f3d` (5.3:1).

### Neutral — Obsidian and Ivory
Night surfaces step `obsidian-900 → 850 → 800`; `obsidian-950` is the sunk layer (contact, footer, deep bands). Day surfaces step `ivory-100 → 50 → white`, with `ivory-200` sunk. Ink is `#e9eae7` by night and `ink-900 #182127` by day; secondary text is `mist-400` / `ink-600`, both ≥5:1.

### Named Rules
- **One signal.** Cyan is spent on action and on one accent word per heading. Never on decoration, never as a background wash larger than a glow.
- **Metal for time.** Anything that is a date, a year, a count or a measurement is champagne/bronze. Anything you can click is cyan.
- **Stages keep their own light.** The CeroSoft product stage is an ivory plate in both themes (`.on-stage` remaps ink locally). The thesis band is obsidian in both themes. These are the two fixed-light regions; everything else follows the theme.

## Typography

- **DM Sans** (CeroSoft's face) for everything you read, from 68px display to 13px captions. Thai falls back to **Noto Sans Thai**.
- **Cormorant Garamond** appears only as numerals in the publication list — the same role it plays for CeroSoft's giant "0".
- **IBM Plex Mono** only for data: dates, coordinates, the email address. Never as a "technical" costume.

### Hierarchy
| Role | Size / line | Weight | Tracking |
|---|---|---|---|
| Display (hero name) | clamp(42–68px) / 1.0 | 600 | -0.04em |
| Headline (section) | clamp(34–48px) / 1.08 | 500 | -0.035em |
| Title (card, role) | 22 / 30 | 500 | -0.025em |
| Body | 16 / 26 | 400 | 0 |
| Lede | 19 / 31 | 400 | 0 |
| Label | 11 / 18 caps | 600 | 0.22em |
| Data | 12–13 mono | 500 | 0.04em |

### Named Rules
- **Medium headlines.** Section headings are weight 500, not bold; size and tight tracking carry them. Only the hero name goes to 600.
- **Tracking floor −0.04em.**

## Layout

Single 1120px column with a 16px safe-area gutter. Sections breathe at 88px. Section heads stack label → headline → 60ch paragraph. Lists of record (timeline, publications) are full-width rows opened by a 1px ink rule and separated by `--border` hairlines — CeroSoft's service-list pattern. Breakpoints: 860px (hero and bands go single column), 760px (nav links hide, grids go single), 520px (publication rows stack).

## Elevation & Depth

Depth comes from layer colour and hairlines first. Shadows are reserved for objects that sit *on* the page:
- `--shadow-lift` — portrait, hovered primary button (cyan-tinted, offset downward, soft).
- `--shadow-stage` — the two fixed-light stages.
Glows are radial gradients on surfaces (hero, thesis band), never halos around elements.

## Shapes

Near-square: `2px` controls and tags, `3px` images, `4px` cards and stages. Circles exist only as instrument geometry — the orbit ring, pipeline step markers. List bullets are 5px outlined diamonds, borrowed from CeroSoft's system-line markers.

## Components

### Buttons
Primary: cyan fill, obsidian text, 48px, 2px radius; hover brightens to `cyan-400` in both themes (obsidian text keeps ≥6:1), lifts 2px with a soft cyan shadow. Line: transparent with a champagne hairline; hover fills with `surface-raised` and the hairline goes solid champagne. Focus: 2px cyan ring, 4px offset.

### Labels (eyebrows)
11px tracked caps with a 32px champagne rule in front — the CeroSoft `.tag` signature. Used once per section head; never stacked.

### Tags
2px radius chips on `surface-raised` with a `--border` outline, muted ink.

### Cards
`surface-raised`, 1px `--border`, 4px radius, no shadow. Hover swaps the border to the champagne hairline. Media sits on a white `--plate` so diagrams and screenshots read in both themes.

### Navigation
Sticky, 84% surface with an 18px blur, champagne hairline below. Links are 13px muted; hover draws a cyan underline out from the centre.

### Product stage (signature)
The CeroSoft block is lifted straight from cerosoft.net: an ivory gradient plate (`#e8e6df → #d8d8d3`) with `--shadow-stage`, dark ink, deep-cyan links, champagne-rimmed phone screenshots.

### Orbit (signature)
A 1px champagne ring at 136% of the portrait with an inner cyan arc that turns once every 26 s. Stops under reduced motion.

## Do's and Don'ts

### Do:
- Pull every colour from `tokens.css` semantics (`--accent`, `--lux-text`, `--line-lux`), never from raw hex in components.
- Keep one cyan word per heading at most (`Building <em>CeroSoft</em>`).
- Test both themes; the stages must look identical in each.

### Don't:
- Bring back gold or indigo from the old cosmic palette.
- Round anything past 4px, or use pill shapes.
- Use gradient text, glass cards, or hard offset block shadows.
- Use champagne on ivory as text — that is what bronze is for.

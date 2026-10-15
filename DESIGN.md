---
name: The Live Twin — Portfolio Edition
description: The portfolio of Patcharadanai Sombatsatien in the visual world of cerosoft.net: charcoal and fog grounds joined by trapezoid notches, one cyan voice, a wireframe dome standing in for the digital twin.
colors:
  cero-cyan: "#00adb5"
  cero-cyan-hover: "#22c4cc"
  charcoal: "#222831"
  charcoal-raised: "#2a3039"
  charcoal-deep: "#1d2229"
  hero-glow: "#2e3641"
  device-black: "#10141a"
  graphite: "#393e46"
  fog: "#f4f5f5"
  paper: "#ffffff"
  well: "#eef0f1"
  muted: "#5b616b"
  line: "#e1e4e6"
  line-strong: "#c9cdd1"
  on-dark: "#eceef0"
  on-dark-heading: "#f3f4f5"
  on-dark-muted: "#a9afb6"
typography:
  display:
    fontFamily: "Inter, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "clamp(2.8rem, 6.4vw, 5.6rem)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Inter, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "clamp(2.1rem, 4.2vw, 3.75rem)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.035em"
  title:
    fontFamily: "Inter, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "1.3rem"
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: "-0.015em"
  body:
    fontFamily: "Inter, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  control:
    fontFamily: "Inter, Noto Sans Thai, system-ui, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 600
    lineHeight: 1.2
  label:
    fontFamily: "Geist Mono, ui-monospace, monospace"
    fontSize: "0.72rem"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "0.06em"
rounded:
  hairline: "2px"
  chip: "6px"
  button: "8px"
  well: "10px"
  capsule: "12px"
  card: "14px"
spacing:
  gutter: "clamp(16px, 4vw, 48px)"
  section: "clamp(96px, 11vw, 168px)"
components:
  button-primary:
    backgroundColor: "{colors.cero-cyan}"
    textColor: "{colors.charcoal}"
    typography: "{typography.control}"
    rounded: "{rounded.button}"
    padding: "0 20px"
    height: "48px"
  button-primary-hover:
    backgroundColor: "{colors.cero-cyan-hover}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "#ffffff"
    rounded: "{rounded.button}"
    height: "48px"
  nav-capsule:
    backgroundColor: "rgba(58, 64, 72, 0.5)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.capsule}"
    height: "52px"
  chip-cta:
    backgroundColor: "{colors.cero-cyan}"
    textColor: "{colors.charcoal}"
    typography: "{typography.label}"
    rounded: "{rounded.chip}"
    height: "32px"
  tag:
    backgroundColor: "{colors.well}"
    textColor: "{colors.graphite}"
    typography: "{typography.label}"
    rounded: "{rounded.chip}"
    padding: "5px 9px"
  card-light:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.charcoal}"
    rounded: "{rounded.card}"
  card-dark-notched:
    backgroundColor: "{colors.charcoal}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.card}"
---

# Design System: The Live Twin, Portfolio Edition

Source of truth for values: [`tokens.css`](tokens.css). Live specimen: [`design-system.html`](design-system.html). The parent system is CeroSoft's own `DESIGN.md` in the CeroSoft-Webpage repo; this file records how the portfolio uses it. When the two differ, cerosoft.net wins.

## Overview

**Creative North Star: "The Live Twin"**

cerosoft.net presents a real operation as a live digital twin: a charcoal cinematic stage where a wireframe draws itself and cyan markers light up where things are happening. The portfolio borrows that grammar for a person. The hero is the same charcoal stage; the wireframe is a slowly turning dome (a nod to the telescope instruments in the work); the portrait sits in a dark notched card; and three live markers say what is true right now: firmware at AirGradient, founder of CeroSoft, M.Sc. from Xi'an Jiaotong.

The page breathes in alternating takes, exactly as the CeroSoft site does: charcoal for the hero, Experience and Contact; fog (#F4F5F5) for CeroSoft, Work, Research and Education. The grounds meet at trapezoid notches. Statements are large, light and tight in Inter 400. Geist Mono appears only as small uppercase data labels.

One accent does all the signalling. Cero Cyan marks the primary action, live events, and the last letter of the two headlines that are allowed one (the name, and "Let's talk").

**Key Characteristics:**
- Charcoal and fog grounds joined by trapezoid notches.
- A single accent, Cero Cyan, for action, live events and the last letter of a headline.
- Inter 400 statements with negative tracking; Geist Mono uppercase for Latin data.
- Floating capsule nav with a cyan call-to-action cell.
- 14px light cards; dark cards cut with one 26px clipped corner.
- A canvas wireframe dome that draws upward with a cyan leading edge, then turns with one live marker in orbit; reduced motion shows the finished frame.

## Colors

A near-monochrome charcoal-and-fog system with one cool cyan voice. Values are CeroSoft's.

### Primary
- **Cero Cyan** `#00adb5`: primary buttons, the nav CTA cell, live dots, the dome's leading edge and orbiting marker, focus on dark, text selection, and the last letter of the hero name. Text on cyan is always Charcoal. **Cyan Lift** `#22c4cc` is its hover.

### Neutral
- **Charcoal** `#222831`: dark ground and the ink on light grounds (one value, two roles). **Charcoal Raised** `#2a3039` and **Charcoal Deep** `#1d2229` shade dark panels and the footer; **Hero Glow** `#2e3641` lifts the hero behind the dome.
- **Fog** `#f4f5f5` is the light ground; **Paper** `#ffffff` the light card; **Well** `#eef0f1` the inset behind images and the tag fill; **Muted** `#5b616b` body copy on light; **Graphite** `#393e46` tag ink.
- **Line** `#e1e4e6` and **Line Strong** `#c9cdd1`: card borders; list rules (publications).
- **On-Dark** `#eceef0`, **On-Dark Heading** `#f3f4f5`, **On-Dark Muted** `#a9afb6`, and the hairline `rgba(236,238,240,.14)` on charcoal.
- **Device Black** `#10141a` frames phone screenshots.

### Named Rules
**One Voice.** Cyan means "act here" or "this is live". It never fills a section or a card, and never colours text except one headline letter.

**Charcoal Is Ink.** The dark ground and the light-ground text are the same charcoal. Do not introduce a second near-black.

**Local remap, not a theme.** There is no day/night toggle. `.dark` and `.card-dark` remap the semantic tokens (`--ink`, `--ink-muted`, `--rule`, `--chip-bg`, `--focus`) for everything inside them.

## Typography

**Inter** for everything read (Noto Sans Thai as the Thai fallback); **Geist Mono** for data labels only.

| Role | Size / line | Weight | Tracking |
|---|---|---|---|
| Display (hero name) | clamp(2.8–5.6rem) / 1.02 | 400 | -0.04em |
| Headline (section) | clamp(2.1–3.75rem) / 1.08 | 400 | -0.035em |
| Figure (stats) | clamp(1.9–2.6rem) / 1.1, tabular | 400 | -0.035em |
| Title (card, role) | 1.3rem / 1.3 | 500 | -0.015em |
| Body | 1rem / 1.6 | 400 | 0 |
| Label (Geist Mono, uppercase) | 0.72rem / 1.4 | 400 | 0.06em |

### Named Rules
**Light Statements.** Latin display and headline text is weight 400, never bold.
**Mono Is Data.** Geist Mono carries dates, counts, tags and marker labels. It is never a label above a heading.
**Typed Last Letter.** The hero name types in grapheme by grapheme and its last letter is cyan. The contact headline repeats the move once. No other headline is coloured.

## Layout

A single column of full-bleed sections inside a centred wrap of `min(1200px, 100% − 2 × gutter)`. Section rhythm is `clamp(96px, 11vw, 168px)`; consecutive light sections drop their top padding so the fog runs on. Section heads are centred, a headline and a 60ch lead. Splits go single-column at 1000px; the nav collapses to a menu toggle at 860px; the notch shortens to 18px at 640px.

Order: hero (charcoal, stats strip inside) → CeroSoft (fog, dark notched card) → Work (fog, thesis dark card, light project cards) → Experience (charcoal, timeline with logo tiles) → Research and Education (fog) → Contact and footer (charcoal).

## Elevation & Depth

Depth comes from ground changes and cinematic light, not shadow stacks. Light cards are flat with a 1px Line border. Only product imagery floats: the portrait and the CeroSoft screenshots use **Device drop** (`0 40px 80px -30px rgba(0,0,0,.7)`). The hero's depth is a radial glow behind the dome and fog in the wireframe's alpha.

## Shapes

Cards 14px; buttons 8px; chips, tabs and marker labels 6px; the nav capsule 12px; image wells 10px. Dark cards keep 14px on three corners and cut the top-right with a 26px diagonal clip. Section joins use a trapezoid notch: a centred tab `min(520px, 64%)` wide and 26px tall, in Fog, on the dark section's top or bottom edge.

## Components

### Buttons
48px, 8px radius, 600 weight at 0.95rem, with a trailing arrow (inline SVG) that nudges 3px on hover. **Primary:** cyan fill, charcoal text, lifts to Cyan Lift. **Ghost (on dark):** transparent, white 32% border, white text. **Outline (on light):** charcoal border, inverts on hover.

### Navigation
A capsule fixed 14px from the top, max 1080px, 52px tall, translucent graphite with a 16px blur; solid once the hero has scrolled away. Brand with a pulsing live dot on the left, links centred-right, a cyan "Get in touch" chip at the end. Below 860px a menu toggle opens a solid dark sheet; the last row is cyan.

### Markers (signature)
A 6px mono-uppercase chip on a near-black fill with a cyan hairline and a dot. The first marker is live (pulsing cyan); the rest are static grey dots. They sit under the portrait and state current roles.

### Dome (signature)
A canvas wireframe sphere behind the hero portrait. Latitude and longitude lines in cool grey with depth-based alpha; it draws upward over 2.8s with a cyan leading ring, then turns slowly while a tilted cyan orbit carries one live marker. It pauses off-screen and shows one finished frame under reduced motion.

### Timeline logo tiles
Company logos sit on a 96×56 white tile (6px radius) above each date, so JPG and SVG logos with white backgrounds read on charcoal.

### Motion
Expo-out (`cubic-bezier(.16, 1, .3, 1)`) for everything. The hero name types in at 45ms per grapheme, then copy rises 24px in sequence. Cards settle 28px upward on entry and are never hidden. Reduced motion shows every finished state.

## Do's and Don'ts

### Do:
- Pull colours only from `tokens.css`; use the semantic roles inside `.dark` and `.card-dark`.
- Alternate charcoal and fog and join them with the notch.
- Keep cyan to actions, live events and one headline letter, with charcoal text on it.
- Set Latin headlines at weight 400 with negative tracking.

### Don't:
- Reintroduce a day/night toggle, champagne, ivory, gold or indigo.
- Put a label above a heading, or use mono for anything but Latin data.
- Add shadows to text cards, gradient text, or glass cards.
- Round past 14px or use pill shapes outside small controls.

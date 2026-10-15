# Patcharadanai Sombatsatien — Portfolio

Static one-page portfolio (HTML + CSS + a little vanilla JS). No build step.

## Structure

```text
Cheer-Portfolio/
├── index.html     # the whole page: content, styles (Cosmic Portfolio tokens) and scripts
├── img/           # WebP images (projects, CondoMate screens, portrait)
└── video/         # MP4 demos (vehicle counting, LINE Notify)
```

## Preview locally

Open `index.html` in a browser, or run a static server:

```bash
npx serve .
```

## Design

Colours, fonts, spacing and radii follow the **Cosmic Portfolio** design system
(night-sky `surface`, gold accent, indigo secondary; Space Grotesk + IBM Plex Sans Thai).
Dark is the default theme; the "Day" button switches to the light theme.

## Deploy (suggested)

- **GitHub Pages:** push this folder to a repo (e.g. `Cheer3142.github.io`) and enable Pages on `main` / root.
- **Vercel:** import the repo as a static site (no build command, output = root), or add it as a subdomain of cerosoft.net.

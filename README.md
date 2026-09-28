# The 404 on 369

The inside breakdown of the glitches, anomalies, and hidden mechanics of the universal frequency blueprint... and some of the other stupid stuff I think about.

A personal digital garden of thought experiments — not answers. Live at <https://404369.xyz>.

## Files

| Path | What it is |
| --- | --- |
| `index.html` | The threshold: masthead, manifesto, hedge, and three doors onto the shelves. |
| `reality-mechanics.html` | Shelf 01 — Reality Mechanics. |
| `two-beings.html` | Shelf 02 — The Thoughts of Two Beings. |
| `field-notes.html` | Shelf 03 — Field Notes. |
| `404.html` | The not-found page. Because it sits at the deploy root, Cloudflare Pages serves it with a real 404 status for unknown URLs instead of the homepage. |
| `favicon.svg` | The site mark, drawn flat in the design system palette. |
| `_redirects` | One rule, so the browser's automatic `/favicon.ico` request gets the SVG rather than the catch-all page. |
| `styles.css` | The entire design system: warm bone paper on a graph-paper ground, a margin-annotation column, ink and one correction-pen red. |
| `.github/workflows/deploy.yml` | The deploy workflow. |
| `README.md` | This file. |

## Design

Every page shares one stylesheet and the same masthead, `sheet`/`row` structure, and colophon. There is no JavaScript anywhere and no external requests at all: system font stacks, inline SVG, no webfonts, no CDN, no analytics. The door interactions are CSS-only, driven by `:hover` and `:focus-visible`.

## Deploy

Pushing to `main` runs `.github/workflows/deploy.yml`, which deploys the repository root to Cloudflare Pages with `wrangler pages deploy . --project-name=404369`.

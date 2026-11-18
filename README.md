# Spazio Zeno — Website

Homepage of Spazio Zeno, the design studio from San Zeno, Brescia.

- Static site: one `index.html` (HTML, CSS, JavaScript). No build step.
- Default view: static grid (Figma «Homepage / Desktop / 1440w / Grid Large»).
- Immersive view: Osmo Supply «Infinite Draggable Grid» (GSAP 3.15 + Observer), images rise in a wave.
- About panel under the header, smooth scroll with Lenis, easing `cubic-bezier(0.625, 0.05, 0, 1)`.
- Contact: hello@spaziozeno.com

## Images
For now every image is a grey placeholder (`#D9D9D9`). Real project images will be added later.

## Font
The page uses **Neue Montreal Regular** from `fonts/NeueMontreal-Regular.woff2`.
The font file is **not** in this repository because the repository is public and the font is a commercial typeface.
Add the licensed file to `fonts/` before deploying; without it the page falls back to Helvetica Neue / Arial.

## Deploy (Vercel)
Framework preset: **Other** · Build command: none · Output directory: `.` (root).

# Spazio Zeno — Website

Homepage of Spazio Zeno, the design studio from San Zeno, Brescia.

- Static site: one `index.html` (HTML, CSS, JavaScript). No build step.
- Default view: static grid (Figma «Homepage / Desktop / 1440w / Grid Large»).
- Immersive view: Osmo Supply «Infinite Draggable Grid» (GSAP 3.15 + Observer), images rise in a wave.
- About panel under the header, smooth scroll with Lenis, easing `cubic-bezier(0.625, 0.05, 0, 1)`.
- Contact: hello@spaziozeno.com

## Images
For now every image is a grey placeholder (`#D9D9D9`). Real project images will be added later.

## About photos (slider)
The photos of the About panel are the `<img>` tags written inside `<div class="about__media" id="aboutMedia">` in `index.html`.
To add a photo, put the file in `img/` (e.g. `img/about/studio-01.webp`) and add one line inside that div, in the order the photos should appear:

```html
<img src="img/about/studio-01.webp" alt="Short description of the photo">
```

The panel adapts by itself:
- **no photos** → the photo box and the arrows are hidden;
- **1 photo** → the photo is shown, without arrows;
- **2 or more** → slider with the arrows (the new photo is revealed from the side of the arrow, 0.9 s).

To remove a photo, delete its `<img>` line. Nothing else to change in CSS or JavaScript.

## Font
The page uses **Neue Montreal Regular** from `fonts/NeueMontreal-Regular.woff2`.
The font file is **not** in this repository because the repository is public and the font is a commercial typeface.
Add the licensed file to `fonts/` before deploying; without it the page falls back to Helvetica Neue / Arial.

## Deploy (Vercel)
Framework preset: **Other** · Build command: none · Output directory: `.` (root).

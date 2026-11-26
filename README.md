# MAAG — collection page with footer overscroll

Static prototype of the MAAG collection page. The footer fills one screen;
scrolling past it fills a progress line and opens the new-arrivals block
(ZARA-style overscroll).

Open `index.html` in a browser, no build step.

- `assets/` — images and SVG icons exported from Figma
- Overscroll threshold, decay and View Transition are in the script at the bottom of `index.html`
- With `prefers-reduced-motion` the overscroll is off and «Новинки» works as a plain link

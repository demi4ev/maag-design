# MAAG — collection page with footer overscroll

Static prototype of the MAAG collection page. The footer fills one screen;
scrolling past it fills a progress line and opens the new-arrivals block
(ZARA-style overscroll).

Open `maag/index.html` in a browser, no build step.

- `assets/` — images and SVG icons exported from Figma
- Overscroll threshold, decay and View Transition are in the script at the bottom of `index.html`
- With `prefers-reduced-motion` the overscroll is off and «Новинки» works as a plain link

## Structure

- `index.html` — project selector (tabs MAAG / VILET, task list in each)
- `maag/` — MAAG collection page with footer overscroll
- `vilet/` — VILET home page with expanding menu (1440 / 768 / 360 from Figma «main-menu 18-11-2026»)
  - Menu opens from the burger, «Одежда» expands the submenu (side panel on desktop/tablet, replaces the list on mobile), Esc / overlay / ✕ close it
  - Placeholders (grey blocks) mark photos not yet exported from Figma: menu banner, «Pants» heroes, «Tops»/«Looks» tiles, #VILETLOOKS grid

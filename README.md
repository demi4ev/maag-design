# MAAG — collection page with footer overscroll

Static prototype of the MAAG collection page. The footer fills one screen;
scrolling past it fills a progress line and opens the new-arrivals block
(ZARA-style overscroll).

Open `maag-1115/index.html` in a browser, no build step.

- `assets/` — images and SVG icons exported from Figma
- Overscroll threshold, decay and View Transition are in the script at the bottom of `index.html`
- With `prefers-reduced-motion` the overscroll is off and «Новинки» works as a plain link

## Structure

- `index.html` — project selector (tabs MAAG / VILET, task list in each)
- `maag-1110/` — MAAG catalog with quick add to cart (1440 / 360 from Figma «MAAG» frames «1440 - catalog» / «360 - catalog»)
  - «+» on a card opens colour + size: a panel over the lower edge of the photo on desktop, a dimmed bottom sheet on ≤760px; tapping a size adds the item at once, «Отменить» undoes it, the header cart badge counts
  - Esc / outside click / ✕ close the picker; the second icon in the 360 header switches to one column
  - Per-colour stock is stubbed in the script (`COLORS`): XS sold out for the first colour, a crossed swatch marks a colour with no sizes left
- `maag-1115/` — MAAG collection page with footer overscroll
- `vilet-132/` — VILET home page with expanding menu (1440 / 768 / 360 from Figma «main-menu 18-11-2026»)
  - Menu opens from the burger, «Одежда» expands the submenu (side panel on desktop/tablet, replaces the list on mobile), Esc / overlay / ✕ close it
  - Placeholders (grey blocks) mark photos not yet exported from Figma: «Pants» heroes, «Tops»/«Looks» tiles, #VILETLOOKS grid

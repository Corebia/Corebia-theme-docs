---
title: Collection list
layout: default
parent: Sections
nav_order: 7
permalink: /sections/collection-list/
---

# Collection list

The **Collection list** section displays a row of collection cards. Each card shows the collection's image (or first product image as a fallback) and name, and links to the collection page.

## Settings

- **Heading** — The section heading. Default: `Collections`.
- **Collections** — Reference text only; collections are configured per block.
- **Number of columns on desktop** — Range: 2 to 5.
- **Color scheme** — The color scheme applied to the section. Default: scheme-1.
- **Image ratio** — The aspect ratio of each collection card image. Options:
  - **Adapt to image** — Each card uses the natural ratio of its collection image.
  - **Portrait** — 3:4.
  - **Square** — 1:1.
  - **Landscape** — 4:3.

## Blocks

Each block represents one collection card.

### Collection

- **Collection** — The collection to display in this slot.

## Tips

- **Cap at three or four collections** for the home page. Long lists better belong on the Collection list page (`/collections`).
- **Collection images** — Make sure each collection has an image set in `Shopify admin > Products > Collections > [collection]`. Without an image, Shopify falls back to the first product's image, which can be inconsistent.
- **Image ratio** — Match this to your photography style. Portrait works for category-style collections (Outerwear, Knitwear); landscape works for editorial collections (Spring 2026 Lookbook).
- **Heading customization** — Replace `Collections` with something more brand-aligned (`Shop by category`, `Our world`).

## Related

- For the dedicated full-page collection list, see [Collections list page](../../templates/collection-list/).

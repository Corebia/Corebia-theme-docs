---
title: Home page
layout: default
parent: Templates
nav_order: 1
permalink: /templates/home-page/
---

# Home page

The **Home page** is the storefront entry point at `/`. It uses the `index.json` template, which is JSON-based, so you can fully customize the section list from the theme editor.

## URL

`https://yourstore.com/`

## Sections included by default

When Pave is installed, the home page comes with these sections in this order:

1. **Hero banner** — Full-bleed editorial photograph with brand name overlay.
2. **New arrivals** — Row of three featured product cards.
3. **Brand message** — Image + heading + body + button.
4. **Collection list** — Two collection cards.
5. **Brand image** — Full-bleed editorial image.
6. **Newsletter** — Email signup form.

To customize, open the theme editor and select any section to edit its settings. Use the **Add section** button to insert new sections at any position.

## Sections that can be added

The home page accepts any section in the **Body** group:

- [Hero banner](../../sections/hero/)
- [New arrivals](../../sections/new-arrivals/)
- [Brand message](../../sections/brand-message/)
- [Brand image](../../sections/brand-image/)
- [Collection list](../../sections/collection-list/)
- [Newsletter](../../sections/newsletter/)
- [Rich text with image](../../sections/rich-text-image/)
- [Customer reviews](../../sections/customer-reviews/)
- [FAQ](../../sections/faq/)
- [Recently viewed](../../sections/recently-viewed/)
- [Featured product](../../sections/featured-product/)
- [Custom Liquid](../../sections/custom-liquid/)

## Special behaviors

- **Header on home page** — The fixed branding in the top left is hidden on the home page so the hero banner can use the full screen. The hover trigger zone for the navigation panel is only active on the home page.
- **Recently viewed on home page** — Hidden for first-time visitors who have no view history. To avoid an empty section on a fresh visit, consider not adding **Recently viewed** to the home page.

## Tips

- **Lead with brand, then product.** Pave's design favors a hero-first home page over a catalog-first one. Move products higher up only if your traffic is buyers, not browsers.
- **Aim for 4–7 sections.** Too few feels sparse; too many turns the home page into a long scroll.
- **Replace default copy.** The default headings ("Crafted with intention", "ATELIER") are placeholders. Update them before publishing.

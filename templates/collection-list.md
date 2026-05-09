---
title: Collections list page
layout: default
parent: Templates
nav_order: 5
permalink: /templates/collection-list/
---

# Collections list page

The **Collections list page** is the index of every collection in your store. It uses the `list-collections.json` template.

## URL

`https://yourstore.com/collections`

## Sections included by default

1. **Main list collections** — The grid of all collections in the store.

## Main list collections section

- **Show back link and breadcrumb** — Toggle.
- **Heading** — The page heading. Default: `Collections`.
- **Subheading** — Optional supporting text.
- **Heading alignment** — Options: **Left**, **Center**, **Right**.
- **Image ratio** — Aspect ratio of each collection card image. Options: **Adapt to image**, **Square (1:1)**, **Portrait (3:4)**, **Landscape (4:3)**.
- **Desktop columns** — Range slider.
- **Mobile columns** — Options: **1 column**, **2 columns**.
- **Sort collections by** — Options: **Admin order**, **A–Z**, **Most products first**.
- **Show product count** — Display the number of products in each collection on the card.
- **Show empty collections** — Toggle whether collections with zero products are listed.
- **Color scheme** — Default: scheme-1.
- **Top padding** and **Bottom padding**.

## Sections that can be added

In addition to **Main list collections**, you can add any of these sections:

- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [Newsletter](../../sections/newsletter/)
- [FAQ](../../sections/faq/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Sort collections by Admin order** if you've manually arranged collections in `Shopify admin > Products > Collections`. The default sort is alphabetical, which may not match your intended hierarchy.
- **Hide empty collections** by setting **Show empty collections** to off — empty collections look like errors to customers.
- **Mobile columns** — On mobile, **1 column** gives each collection a hero-like presence; **2 columns** keeps the page short. Pick based on the number of collections.

## Related

- For a curated list of collections on the home page, use the [Collection list section](../../sections/collection-list/) instead.

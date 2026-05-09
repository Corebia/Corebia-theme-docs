---
title: Collection page
layout: default
parent: Templates
nav_order: 3
permalink: /templates/collection-page/
---

# Collection page

The **Collection page** displays the products inside a single collection, with filters, sort options, and a product grid. It uses the `collection.json` template.

## URL

`https://yourstore.com/collections/<collection-handle>`

## Sections included by default

1. **Main collection** — The collection grid with filters and sort.

## Main collection section

### Hero banner area

- **Show hero banner** — Uses the collection image as a full-width banner. Default: on.
- **Hero height** — Options: **Small (21:9)**, **Medium (16:9)**, **Large (16:9 tall)**.
- **Mobile image (optional)** — Recommended ratio: 4:5 or 3:4. Falls back to collection image if empty.
- **Image focal point** — Options: **Top**, **Center**, **Bottom**, **Left**, **Right**.
- **Text position** — Options: **Bottom center**, **Center**, **Bottom left**.
- **Hero overlay darkness** — Range slider.
- **Show collection description** — Toggle the collection description text.

### Filters and toolbar

- **Show filters** — Toggle the filter panel. Filters come from your Shopify admin filtering configuration. See [Search and filtering](../../features/search/).
- **Show sort options** — Toggle the sort dropdown.

### Product grid

- **Products per page** — How many products to load per page. Pagination loads more.
- **Desktop columns** — Options: **2 columns**, **3 columns**, **4 columns**.
- **Show vendor** — Display vendor on each card.
- **Show second image on hover** — Displays alternate product image on hover.
- **Show quick view button** — Adds a quick-view button on hover.

### Other

- **Show back link and breadcrumb** — Toggle.
- **Color scheme** — Default: scheme-1.

## Special behaviors

- **Filter persistence** — Selected filters appear in the URL as query params, so customers can bookmark filtered views.
- **Sort persistence** — Same as filters; sort option is reflected in the URL.
- **Filter drawer on mobile** — Filters open in a slide-in drawer on small screens.
- **Pagination** — Customers click through pages; the URL updates with the `page=` parameter.
- **Empty state** — If a collection has no products that match the current filters, a clear empty state is shown with a way to clear filters.

## Sections that can be added

You can add any of these sections below the **Main collection** section:

- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [Newsletter](../../sections/newsletter/)
- [FAQ](../../sections/faq/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Configure filters in your admin.** `Shopify admin > Online Store > Navigation > Search and discovery` (or via the Search & Discovery app) is where you control which filters appear.
- **Hero banner per collection** — Each collection can have its own hero image. Set it in `Shopify admin > Products > Collections > [collection] > Image`.
- **Products per page** — 24 to 36 is typical. Lower numbers force more pagination clicks; higher numbers slow down initial load on slow connections.

## Catalog template

The catalog page (`/collections/all`) uses a separate template — see [Catalog page](../catalog-page/).

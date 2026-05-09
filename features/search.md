---
title: Search
layout: default
parent: Features
nav_order: 2
permalink: /features/search/
---

# Search

Pave provides two search experiences: **predictive search** in the header (suggestions as the customer types) and **faceted filtering** on the search results, collection, and catalog pages.

## Predictive search

When the customer opens the header search bar and starts typing, Pave fetches suggestions in real time without a page reload.

### Where it appears

- In the inline search field that expands inside the header navigation panel.

### What is shown

By default, predictive search returns matching products, with optional inclusion of collections, pages, and articles. Configuration is in the predictive search section settings (controlled internally by the theme).

### Settings (predictive search)

Predictive search reads its settings from the **Predictive search** section. The settings are:

- **Show vendor** — Toggle vendor display in suggestions.
- **Show price** — Toggle price display.
- **Show collections** — Include collections as suggestion type.
- **Show pages** — Include pages.
- **Show articles** — Include articles.
- **Product results limit** — Cap the number of product suggestions returned.

### How to configure

These settings are exposed in the theme editor when you select a predictive search section in the editor (typically internal — Pave wires them up automatically).

## Faceted filtering

Faceted filtering lets customers narrow the product grid by attributes: collection, vendor, price range, color, size, availability.

### Where it appears

- The [Collection page](../../templates/collection-page/).
- The [Catalog page](../../templates/catalog-page/).
- The [Search page](../../templates/search-page/).

### Filter source

Filter options come from the **Search and discovery** configuration in your Shopify admin:

1. In `Shopify admin > Online Store > Navigation`, scroll to **Search and discovery**, or install the **Search & Discovery** app from the Shopify App Store.
2. Configure filters per collection or globally. You can include filters based on product type, vendor, price, color, size, availability, and any product metafield you've defined.
3. Save.

The **Show filters** setting on the relevant section must be enabled for filters to appear. See the section settings on each page.

### Filter behavior

- Selected filters are reflected in the URL, so a filtered view can be bookmarked and shared.
- Multiple filters compose with AND logic.
- Within a single filter (for example, color), multiple values compose with OR logic.

### Sort options

Sort options are also controlled by Shopify and rendered when **Show sort options** is enabled on the section. Default sorts include: Featured, Best selling, Alphabetical (A–Z, Z–A), Price (low → high, high → low), Date (new → old, old → new).

## Search results page

When the customer presses Enter in the search field, they land on the [Search page](../../templates/search-page/). It shows the matching products in a grid with the same filtering and sort tools as the collection page.

If a search returns no products, the **Featured collection (shown when no results)** setting on the section can fall back to a curated collection.

## Troubleshooting

- **My filters don't appear** — Confirm **Show filters** is enabled on the relevant section, and that filters are configured in `Shopify admin > Online Store > Navigation > Search and discovery`.
- **Predictive search shows nothing** — The customer may have typed fewer than two characters; predictive search waits for at least two. Also confirm the storefront is not in a frozen-cache state from a recent theme deploy.
- **A product is not searchable** — Check that the product status is **Active**, and that it is published to the **Online Store** sales channel.
- **Custom synonyms** — Configure synonyms in the Search & Discovery app so common alternate terms map to the right products.

## Related

- [Search page template reference](../../templates/search-page/)
- [Collection page template reference](../../templates/collection-page/)

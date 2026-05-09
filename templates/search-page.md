---
title: Search page
layout: default
parent: Templates
nav_order: 7
permalink: /templates/search-page/
---

# Search page

The **Search page** displays the results of a customer's search query. It uses the `search.json` template.

## URL

`https://yourstore.com/search?q=<query>`

## Sections included by default

1. **Main search** — The results grid with filters, sort, and an empty-state featured collection.

## Main search section

### Filters and toolbar

- **Show filters** — Toggle the filter panel. Filters are inferred from search results.
- **Show sort options** — Toggle the sort dropdown.

### Product grid

- **Products per page** — How many products to load per page.
- **Desktop columns** — Options: **2 columns**, **3 columns**, **4 columns**.
- **Show vendor** — Display vendor on each card.
- **Show second image on hover** — Displays alternate product image on hover.

### Empty state

- **Featured collection (shown when no results)** — When a search returns no products, this collection is shown as a fallback. Default: leave blank to show no fallback.

### Other

- **Show back link and breadcrumb** — Toggle.
- **Color scheme** — Default: scheme-1.

## Special behaviors

- **What gets searched** — Products, blog articles, and pages, as configured in `Shopify admin > Online Store > Navigation > Search and discovery`.
- **Predictive search** — As the customer types in the header search box, predictive suggestions appear inline. The full Search page is the destination after pressing Enter or clicking through. See [Search](../../features/search/).
- **Filter persistence** — Selected filters appear in the URL.
- **Empty state** — When a search returns no results, an empty state encourages further exploration. The optional **Featured collection** appears below.

## Sections that can be added

You can add any of these sections below the **Main search** section:

- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Newsletter](../../sections/newsletter/)
- [FAQ](../../sections/faq/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Set a featured collection** — A blank empty state sends customers away. Featuring your top sellers or new arrivals on no-results is a quick win.
- **Synonyms in admin** — Configure synonyms in the Search & Discovery app so common typos and alternate names map to the right products.
- **Test searches** — Search for products by alternate names ("jumper" vs "sweater"). Surprises here mean missed sales.

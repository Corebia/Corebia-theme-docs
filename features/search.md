---
title: Search
layout: default
parent: Features
nav_order: 2
permalink: /features/search/
---

# Search

Pave provides two search experiences: **predictive search** in the header, with suggestions as the customer types, and **faceted filtering** on the search results, collection and catalog pages.

## Predictive search

When the customer opens search in the header and types, Pave fetches suggestions in real time without a page reload.

### Where it appears

- In the search popover of the desktop header bar.
- In the search field inside the header's navigation panel.
- At the top of the [Search page](../../templates/search-page/).

### What is shown

Suggested search terms, matching products with their price, and matching collections, pages and articles. Suggestions start after two characters.

### Before the customer types

The search drawer doesn't have to open empty. Under [Theme settings > Search](../../theme-settings/search/) you can fill it with:

- **Featured collection.** Products from one collection, shown before a query. **Products to show** sets how many, from 2 to 10.
- **Popular searches menu.** A menu whose items become links in the drawer. Build it under `Online Store > Navigation` like any other menu.
- **Show recent searches.** The shopper's last five searches, kept in their own browser only. They can remove any of them. Off by default.

With none of these set, the drawer shows nothing until the customer types.

## Faceted filtering

Faceted filtering lets customers narrow the product grid by attributes: collection, vendor, price range, color, size, availability.

### Where it appears

- The [Collection page](../../templates/collection-page/).
- The [Catalog page](../../templates/catalog-page/).
- The [Search page](../../templates/search-page/).

On the collection page, the **Filter layout** setting places the filters in a sidebar or in a horizontal bar above the grid. On mobile, both open the same slide-in drawer.

### Filter source

Filter options come from Shopify's **Search & Discovery** app:

1. Install the free **Search & Discovery** app from the Shopify App Store.
2. In the app, open **Filters** and add the filters you want: product type, vendor, price, color, size, availability, or any product metafield you've defined.
3. Save.

The **Show filters** setting on the relevant section must be on for filters to appear. See the section settings on each page.

### Filter behavior

- Selected filters are reflected in the URL, so a filtered view can be bookmarked and shared.
- Multiple filters combine with AND logic.
- Within a single filter (for example, color), multiple values combine with OR logic.

### Sort options

Sort options are controlled by Shopify and shown when **Show sort options** is on in the section. The usual sorts are Featured, Best selling, Alphabetical (A to Z, Z to A), Price (low to high, high to low) and Date (new to old, old to new).

## Search results page

When the customer presses Enter in the search field, they land on the [Search page](../../templates/search-page/). It shows the matching products in a grid with the same filtering and sort tools as the collection page.

Above the results, a row of links switches between **All** results, **Products**, **Articles** and **Pages**. Filters and sorting apply to products, so they are hidden while the customer looks at articles or pages.

If a search returns nothing, the page can offer a way forward: **Featured collection (shown when no results)** shows a curated collection, and **Contact link (shown when no results)** adds a link to a page you choose, usually your contact page.

## Troubleshooting

- **My filters don't appear.** Confirm **Show filters** is on in the relevant section, and that filters are set up in the Search & Discovery app.
- **Predictive search shows nothing.** The customer may have typed fewer than two characters; predictive search waits for at least two.
- **The drawer is empty before typing.** Set a featured collection or a popular searches menu under [Theme settings > Search](../../theme-settings/search/).
- **A product is not searchable.** Check that the product status is **Active**, and that it is published to the **Online Store** sales channel.
- **Custom synonyms.** Configure synonyms in the Search & Discovery app so common alternate terms map to the right products.

## Related

- [Search page template reference](../../templates/search-page/)
- [Collection page template reference](../../templates/collection-page/)
- [Search settings](../../theme-settings/search/)

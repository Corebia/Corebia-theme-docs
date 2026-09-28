---
title: Search page
layout: default
parent: Templates
nav_order: 8
permalink: /templates/search-page/
---

# Search page

Where a shopper lands after pressing Enter in the header's search field. It uses the **Main search** section: the same filterable, sortable grid as a collection page, plus an empty state for searches that return nothing.

The dropdown that appears while typing is configured separately, in [Predictive search](../../sections/predictive-search/).

## Section settings

- **Show back link and breadcrumb.** The back link returns to the previous page in your store, and the breadcrumb traces the path from the home page. Default: on.

### Filters and toolbar

- **Show filters.** Default: on.
- **Show sort options.** Default: on.

### Product grid

- **Products per page.** Range: 8 to 48 in steps of 4. Default: 24.
- **Desktop columns.** **2 columns**, **3 columns** or **4 columns** (default).
- **Show vendor.** Default: off.
- **Show second image on hover.** Default: on.

### Empty state

- **Featured collection (shown when no results).** The collection whose products are offered when a search returns nothing.
- **Contact link (shown when no results).** A link to your contact page, offered alongside the no-results message. Leave blank to show no link at all.

### Colors

- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 95 px and 65 px. The largest padding, used on screens 1920 px and wider; it scales down on smaller screens.

## Products, articles and pages

Shopify searches products, blog articles and pages together. Above the results, a switcher lets the shopper narrow them to **All**, **Products**, **Articles** or **Pages**. It stays in place even when one type has no matches, so the shopper can always switch back.

## Filtering search results

Search results carry the same filters as a collection page, configured in Shopify's free [Search & Discovery](https://apps.shopify.com/search-and-discovery) app. This is a Theme Store requirement and it is on by default: a shopper who searches "shirt" and gets ninety results needs to narrow them the same way they would in a collection. The filters are product filters, so they and the sort control are hidden while the shopper is looking at articles or pages only.

## The empty state

A search with no matches is a moment where shoppers leave. Setting **Featured collection** turns a dead end into a route back: the page explains that nothing matched and offers that collection's products instead.

Pick something broad: best sellers, new arrivals, or the catalog's most popular category. A narrow collection here is unlikely to match what the shopper was after.

## Improving what search finds

What matches, and in what order, is Shopify's, not the theme's. To improve it:

- Write product titles the way shoppers describe things, not the way your supplier does.
- Add synonyms in Search & Discovery, so "trainers" finds "sneakers".
- Use product types and tags consistently; both are searched.

## Tips

- **24 results per page suits search.** A shopper who searched has a specific intent and scans quickly; more per page means less pagination in the way.
- **Four columns is right here** even if your collections use three. Search results are scanned rather than browsed.
- **Set the empty state before launch.** It is invisible until it matters, and by then the shopper is already leaving.
- **Point the contact link at a real person.** A shopper who searched and found nothing is often one question away from buying. Your [contact page](../contact-page/) is the natural target.

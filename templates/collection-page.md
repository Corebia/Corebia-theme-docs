---
title: Collection page
layout: default
parent: Templates
nav_order: 3
permalink: /templates/collection-page/
---

# Collection page

The collection page is built from the **Main collection** section: an optional hero banner using the collection's own image, then a filterable, sortable product grid with a sidebar.

## Section settings

- **Show back link and breadcrumb** — Default: on.

### Hero banner

- **Show hero banner** — Uses the collection image as a full-width banner. Default: on.
- **Hero height** — **Small (35% of screen height)**, **Medium (50%)** (default) or **Large (65%)**.
- **Mobile image (optional)** — 3:4 aspect ratio recommended. Falls back to the collection image.
- **Image focal point** — **Use the image's focal point** (default), **Top**, **Center**, **Bottom**, **Left** or **Right**. The default follows the crop set on the image in your Files area.
- **Text position** — **Bottom center** (default), **Center** or **Bottom left**.
- **Hero overlay darkness** — Range: 0% to 80% in 5% steps. Default: 35%.
- **Show collection description** — Default: on.

### Filters and toolbar

- **Show filters** — Default: on.
- **Sidebar navigation** — A menu shown at the top of the sidebar, above the filters.
- **Show sort options** — Default: on.

### Product grid

- **Products per page** — Range: 4 to 24 in steps of 2. Default: 12.
- **Desktop columns** — **2**, **3** (default) or **4 columns**.
- **Show vendor** — Default: off.
- **Show second image on hover** — Displays the alternate product image on hover. Default: on.
- **Show quick view button** — Shows the quick add `+` button on the cards in this grid. Default: on. It also needs **Show quick add button** to be on under [Product cards](../../theme-settings/product-cards/); this setting can only turn it off for this grid, not on.

### Colors

- **Color scheme** — Default: scheme-1.

## Blocks

- **App block** — Any block offered by an installed app.
- **Custom Liquid** — See [Custom Liquid](../../sections/custom-liquid/).

## Filters come from Shopify

The filters in the sidebar are configured in Shopify's free [Search & Discovery](https://apps.shopify.com/search-and-discovery) app, not in the theme. Install it and open **Filters** to choose which of availability, price, product type, vendor and variant options appear, and in what order.

**Show filters** here only controls whether the theme renders them. With no filters configured in the app, the sidebar shows nothing to filter by.

## The collection image

The hero uses the image set on the collection under `Shopify admin > Products > Collections`. A collection with no image renders no hero, whatever this setting says.

## Tips

- **Set the focal point on the image, not here.** The default option follows the image's own focal point, which then applies everywhere that image is used — hero, tiles, cards.
- **12 products per page suits most catalogs.** Fewer means more pagination; more delays the first paint on mobile without much gain.
- **Use the sidebar navigation for sibling collections.** A shopper in "Coats" is often looking for "Jackets", and a menu at the top of the sidebar is the shortest path.
- **Turn the hero off for utility collections.** A collection that exists to group products for a filter or a link doesn't need a banner.

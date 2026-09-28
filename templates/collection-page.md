---
title: Collection page
layout: default
parent: Templates
nav_order: 4
permalink: /templates/collection-page/
---

# Collection page

The collection page is built from the **Main collection** section: an optional hero banner using the collection's own image, then a filterable, sortable product grid, with up to three promotional tiles placed among the products.

The same section, set up differently, drives the [Lookbook collection page](../lookbook-collection/).

## Section settings

- **Show back link and breadcrumb.** Default: on.

### Hero banner

- **Show hero banner.** Uses the collection image as a full-width banner. Default: on.
- **Hero height.** **Small (35% of screen height)**, **Medium (50% of screen height)** (default) or **Large (65% of screen height)**.
- **Mobile image (optional).** 3:4 aspect ratio recommended. Falls back to the collection image.
- **Image focal point.** **Use the image's focal point** (default), **Top**, **Center**, **Bottom**, **Left** or **Right**. The default follows the crop set on the image in your Files area. The collection template Pave installs comes with **Center** selected, so switch it to the first option if you set focal points on your collection images.
- **Text position.** **Bottom center** (default), **Center** or **Bottom left**.
- **Hero overlay darkness.** Range: 0% to 80% in 5% steps. Default: 35%.

The hero settings are shown while **Show hero banner** is on.

- **Show collection description.** Default: on.
- **Description position.** **Above the grid** (default), **Below the grid** or **Both**. Below the grid the whole description is shown. Above it, the whole description is shown too, except that it is shortened to the first 120 characters when the hero banner is on. Shown when the description is on.

### Filters and toolbar

- **Show filters.** Default: on.
- **Filter layout.** **Sidebar** (default) or **Horizontal bar above the grid**. Where the filters sit on desktop. On mobile both layouts open the same slide-in drawer. Shown when filters are on.
- **Sidebar navigation.** A menu shown at the top of the sidebar.
- **Show sort options.** Default: on.

### Product grid

- **Products per page.** Range: 4 to 24 in steps of 2. Default: 12.
- **Pagination.** **Numbered pages**, **Load more button** (default) or **Infinite scroll**. How shoppers reach the rest of the products. Numbered pages are always crawlable, and the other two keep the next page's link in the page, so search engines can still follow it.
- **Grid style.** How the products are laid out.
  - **Uniform grid** (default) is the standard product grid.
  - **Editorial index** lists the products as large names and reveals each photograph as a shopper points at or focuses a name. On touch screens, and for shoppers who reduce motion, every name keeps its photograph beside it. The grid view control is hidden in this style.
  - **Lookbook spread** keeps the product cards but varies their proportions and widths on a repeating six-cell pattern. It is the grid the [Lookbook collection page](../lookbook-collection/) ships with.
- **Let customers change the grid view.** Adds a control above the grid for 2, 3 or 4 columns, or a list. Your desktop column choice is where it starts. Default: on.
- **Desktop columns.** **2 columns**, **3 columns** (default) or **4 columns**.
- **Show vendor.** Default: off.
- **Show second image on hover.** Displays the alternate product image on hover. Default: on.
- **Show quick add button.** Shows the quick add `+` button on the cards in this grid. Default: on. It also needs **Show quick add button** to be on under [Product cards](../../theme-settings/product-cards/); this setting can only turn it off for this grid, not on.

### Colors

- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 95 px and 65 px. The largest padding, used on screens 1920 px and wider; it scales down on smaller screens.

## Blocks

### Promotional tile

Three fixed tile slots that sit inside the product grid, for a campaign image, a message or a link between the products. They can't be added or removed, only filled: an empty slot shows nothing at all, so a collection with no tiles set looks exactly like a plain grid.

- **Position in the grid.** Which cell the tile takes, counted across the whole collection rather than within one page. Range: 1 to 24. Default: 3. A position past the last product shows nothing. At 12 products per page, the maximum of 24 keeps every tile on page 1 or page 2.
- **Image.** Optional.
- **Heading.**
- **Body text.**
- **Link label** / **Link.** Both a label and a link are needed for the link to show.
- **Columns wide.** Range: 1 to 3. Default: 1. Kept to one column in the list view.
- **Rows tall.** Range: 1 to 3. Default: 1.

All three slots start at position 3. Give each tile you use its own position, or two tiles will sit side by side.

### Other blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/custom-liquid/).

## Filters come from Shopify

The filters are configured in Shopify's free [Search & Discovery](https://apps.shopify.com/search-and-discovery) app, not in the theme. Install it and open **Filters** to choose which of availability, price, product type, vendor and variant options appear, and in what order.

**Show filters** here only controls whether the theme renders them. With no filters configured in the app, there is nothing to filter by.

## The collection image

The hero uses the image set on the collection under `Shopify admin > Products > Collections`. A collection with no image renders no hero, whatever this setting says. The hero is also never shown on `/collections/all`, which has its own [Catalog page](../catalog-page/) template.

## Tips

- **Set the focal point on the image, not here.** The default option follows the image's own focal point, which then applies everywhere that image is used: hero, tiles and cards.
- **12 products per page suits most catalogs.** Fewer means more pagination; more delays the first paint on mobile without much gain.
- **Use the sidebar navigation for sibling collections.** A shopper in "Coats" is often looking for "Jackets", and a menu at the top of the sidebar is the shortest path.
- **Pick the horizontal filter bar for small catalogs.** With three or four filters, a bar above the grid gives the products the full width. A long list of filters reads better in the sidebar.
- **One promotional tile per page is usually enough.** A tile interrupts the grid on purpose. Two on the same screen start competing with the products.
- **Turn the hero off for utility collections.** A collection that exists to group products for a filter or a link doesn't need a banner.

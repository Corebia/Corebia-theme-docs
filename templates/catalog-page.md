---
title: Catalog page
layout: default
parent: Templates
nav_order: 4
permalink: /templates/catalog-page/
---

# Catalog page

The catalog is the page at `/collections/all`: everything you sell, in one filterable grid. It uses the **Main catalog** section, which is close to the [Collection page](../collection-page/) but replaces the hero banner with a text heading and a sidebar menu.

It is an alternate template, `collection.all.json`, so editing it doesn't affect your individual collection pages.

## Section settings

- **Show back link and breadcrumb.** Default: on.

### Catalog heading

- **Show catalog heading.** Displays a heading above the sidebar and on mobile. Default: on.
- **Catalog heading.** Leave empty to use the collection name.
- **Heading link.** Optional URL the heading links to.
- **Sidebar navigation.** A menu shown at the top of the sidebar.

### Filters and toolbar

- **Show filters.** Default: on.
- **Show sort options.** Default: on.

### Product grid

- **Products per page.** Range: 4 to 24 in steps of 2. Default: 12.
- **Desktop columns.** **2**, **3** (default) or **4 columns**.
- **Show vendor.** Default: off.
- **Show second image on hover.** Displays the alternate product image on hover. Default: on.
- **Show quick add button.** Shows the quick add `+` button on the cards in this grid. Default: on. It also needs **Show quick add button** to be on under [Product cards](../../theme-settings/product-cards/).

### Colors

- **Color scheme.** Default: scheme-1.

## Blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/custom-liquid/).

## Catalog or collection?

Both show a filterable grid. The difference is what a shopper arrives expecting.

|  | Catalog | Collection |
|---|---|---|
| URL | `/collections/all` | `/collections/<name>` |
| Opens with | A heading and the sidebar | A hero banner using the collection image |
| Suits | Browsing everything | A curated, themed group |

Link the catalog from your navigation as "Shop all" or similar, and use collections for the routes into it.

## Tips

- **Use the sidebar navigation as the main way in.** On the catalog page it is the shopper's map of your collections, and it is the one thing this template has that the collection page's hero replaces.
- **Filters matter more here than anywhere.** This is the page with the most products on it, so it is where a shopper most needs to narrow down. Configure them in [Search & Discovery](https://apps.shopify.com/search-and-discovery).
- **Leave the heading empty** to let it follow the collection name, unless "All products" isn't the word you'd use.

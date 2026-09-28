---
title: Shop by color
layout: default
parent: Sections
nav_order: 24
permalink: /sections/shop-by-color/
---

# Shop by color

**Shop by color** is a row of color swatches, one for each color in the collection's color filter. A shopper taps a color and the collection reloads filtered to it; tapping the active color again removes the filter.

It reads the filters of the collection it sits on, so it belongs on a [collection template](../../templates/collection-page/). Placed anywhere else, it has no collection to read and shows nothing. It can't be placed in the header or footer groups.

## Settings

- **Heading.** Optional. Leave it blank for swatches with no heading.
- **Section width.** **Page width** (default) or **Full width**.
- **Color scheme.** Default: scheme-1.
- **Top padding** / **Bottom padding.** Range: 0 to 100 px in 1 px steps. Default: 40 px each.

## Where the colors come from

The swatches are the values of the collection's color filter, so the section needs one:

1. In the [Search & Discovery](https://apps.shopify.com/search-and-discovery) app, add a filter for your color option (for example **Color** or **Colour**) or for the Shopify taxonomy color attribute.
2. Make sure the collection has products in more than one color.

Each swatch takes its fill from what Shopify knows about that color: the swatch color or image saved on the option value or taxonomy value first, then Pave's own list of common color names. A color the theme can't resolve shows a neutral chip, and its name still says which color it is.

The section shows nothing when the collection has no color filter, when the filter has no values, or when the collection holds more than 5,000 products, where Shopify stops returning filters.

Swatch size and shape follow the card swatch settings in [Product cards](../../theme-settings/product-cards/), so these swatches match the ones on your product cards.

## Tips

- **Place it above the product grid.** On the collection template, drag it above the main collection section so it reads as a shortcut into the grid.
- **For a store-wide strip, use your all-products collection.** The section can only see one collection's colors, so a row covering the whole catalog goes on the collection that holds everything.
- **Name colors consistently.** "Navy", "navy" and "Navy blue" become three swatches. Tidy option values before you add the filter.
- **Many colors scroll sideways on a phone.** That is intended, but twenty near-identical shades make a long strip. Grouping shades is a job for your option values, not the section.

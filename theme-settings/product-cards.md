---
title: Product cards
layout: default
parent: Theme settings
nav_order: 7
permalink: /theme-settings/product-cards/
---

# Product cards

These settings apply to the product card wherever it appears — collection pages, the catalog, search results, New arrivals, recommendations and recently viewed. Setting them once here keeps every grid in the store consistent.

## Settings

- **Image ratio** — **Adapt to image**, **Portrait (3:4)**, **Square (1:1)** (default) or **Landscape (4:3)**.
- **Show quick add button** — Adds a `+` button to product cards. Products with one variant are added straight to the cart; products with several add the first available variant. Default: on.
- **Show color swatches on cards** — Shows up to 5 colors as selectable swatches. Choosing one updates the card's image, price and link. Any colors beyond the fifth are counted in a `+N` indicator. Default: on.
- **Days to show the new badge** — Products created within this many days show a **new** badge on cards. Range: 0 to 90 days. Default: 30. Set to 0 to hide the badge. The sale badge takes priority over the new badge.

## A note on Image ratio

**Adapt to image** keeps every product's own proportions, which is honest but gives an uneven grid unless your photography is already consistent. The three fixed ratios crop to a common shape, which is what makes a grid look deliberate.

If your catalog is shot to one standard, choose the ratio that matches it and nothing gets cropped. If it isn't, choose the ratio that suits most of it and set focal points on the images that suffer — see [Product media](../../features/product-media/).

## A note on swatches

Card swatches read a product's color option and show it as a real color or image. They rely on Shopify's swatch data, which is set per option value under `Shopify admin > Settings > Metafields and metaobjects`, or automatically from color names. See [Swatches](../../features/swatches/) for the full setup.

Products without a color option simply show no swatches; nothing needs turning off per product.

## Tips

- **Quick add earns its place on repeat-purchase catalogs** — consumables, refills, basics. On a considered-purchase catalog it can short-circuit a decision the product page was going to help with.
- **Quick add on a multi-variant product picks the first available variant.** That is right for a product where the variants are sizes of the same thing, and wrong for one where they are meaningfully different. Consider turning it off if your catalog is mostly the latter.
- **30 days is a sensible new badge.** Long enough that a shopper sees it, short enough that it still means something. Stores that add stock rarely may want 60; stores adding daily may want 7.
- **The two badges never stack.** A product that is both new and on sale shows the sale badge, because that is the one that moves a decision.

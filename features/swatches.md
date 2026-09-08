---
title: Swatches
layout: default
parent: Features
nav_order: 5
permalink: /features/swatches/
---

# Swatches

A swatch shows a variant's colour or material as a chip rather than as a word, so a shopper picks "the sand one" by looking at it.

## Where swatches appear

- **In the variant picker**, on the [Product page](../../templates/product-page/) and in [Featured product](../../sections/featured-product/). Their size and shape are set store-wide under [Variant picker](../../theme-settings/variant-picker/).
- **On product cards**, in every grid in the store, when **Show color swatches on cards** is on under [Product cards](../../theme-settings/product-cards/). Up to five colours show; the rest are counted in a `+N` indicator. Choosing one swaps the card's image, price and link to that variant.

## How a swatch gets its colour

The theme tries four things in order, and the first that gives an answer wins.

### 1. Shopify's own swatch data, the one to use

Set under `Shopify admin > Settings > Metafields and metaobjects > Product options`, where each option value can carry a colour or an image. This is Shopify's native mechanism, it works across apps and themes, and it handles both colours and pattern or material images.

An option value with an **image** here shows that image as the chip. That is the right choice for wood grains, marbles, tweeds and prints, which no single colour can represent.

### 2. A per-product override

For a product whose colour names are its own, add the JSON metafield `pave.color_overrides` to it: an object mapping option value names to hex colours.

```json
{
  "Sand": "#D8C9AE",
  "Ink": "#1B1D26"
}
```

Keys are matched case-insensitively against the option value name. Define the metafield once under `Shopify admin > Settings > Metafields and metaobjects > Products`, then fill it in only on the products that need it.

### 3. The theme's built-in colour names

If neither of the above is set, the theme recognises around thirty common colour names, in English and Spanish, and draws the chip from those.

This is a convenience, not a strategy: it covers the likes of `black`, `navy`, `beige`, `negro` and `crudo`, and it will not know your house names.

### 4. Nothing

An option value the chain can't resolve falls back to a neutral chip with the value's name beside it. The picker still works; it just isn't visual for that value.

## Tips

- **Set Shopify's swatch data and stop there.** It is the only step of the four that is portable, that works for images as well as colours, and that doesn't need per-product work.
- **Use images for anything that isn't flat colour.** A single hex for a leopard print or an oak veneer is worse than no swatch.
- **Be consistent within an option.** Half the colours as real swatches and half as neutral fallbacks looks broken, more than either would alone.
- **Treat the built-in dictionary as a safety net.** It stops a store looking unfinished before you have set anything up; it isn't meant to be the final state.

## Troubleshooting

- **A swatch shows as a plain chip with the name beside it.** Nothing in the chain resolved that value. Set it in Shopify's product options metafield, or add it to `pave.color_overrides` on that product.
- **The colour is close but not right.** You are getting step 3, the built-in dictionary. Set the real value in Shopify's swatch data.
- **No swatches at all on cards.** Check **Show color swatches on cards** under [Product cards](../../theme-settings/product-cards/), and check the product actually has a colour option.

## Related

- [Variant picker](../../theme-settings/variant-picker/): swatch size and out-of-stock behaviour.
- [Product cards](../../theme-settings/product-cards/): swatches in grids.
- [Product media](../product-media/): variant images and how they're chosen.

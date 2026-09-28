---
title: Swatches
layout: default
parent: Features
nav_order: 5
permalink: /features/swatches/
---

# Swatches

A swatch shows a variant's color or material as a chip rather than as a word, so a shopper picks "the sand one" by looking at it.

## Where swatches appear

- **In the variant picker**, on the [Product page](../../templates/product-page/) and in [Featured product](../../sections/featured-product/). Their size and shape are set store-wide under [Variant picker](../../theme-settings/variant-picker/).
- **On product cards**, in every grid in the store, when **Show color swatches on cards** is on under [Product cards](../../theme-settings/product-cards/). Up to five colors show; the rest are counted in a `+N` indicator. Choosing one swaps the card's image, price and link to that variant. The same page sets the card swatches' width, height, corner radius and border.

## Which options get swatches

Swatches are for color options, so the theme looks at the option's name. It recognizes the usual names for color in 16 languages, such as `Color`, `Colour`, `Couleur`, `Farbe`, `Colore`, `Cor`, `Kleur`, `Färg` and `Kolor`. An option named something else, such as `Shade` or `Finish`, gets no swatches on cards.

On the product page, the **Controls** setting under [Variant picker](../../theme-settings/variant-picker/) decides the rest. **By option type**, the default, gives color options swatches, size options buttons and every other option a menu. **Same for every option** applies the chosen style to all options, so any option can be shown as swatches.

## How a swatch gets its color

The theme tries four things in order, and the first that gives an answer wins.

### 1. Shopify's own swatch data, the one to use

Set under `Shopify admin > Settings > Metafields and metaobjects > Product options`, where each option value can carry a color or an image. This is Shopify's native mechanism, it works across apps and themes, and it handles both colors and pattern or material images.

An option value with an **image** here shows that image as the chip. That is the right choice for wood grains, marbles, tweeds and prints, which no single color can represent.

### 2. A per-product override

For a product whose color names are its own, add the JSON metafield `pave.color_overrides` to it: an object mapping option value names to hex colors.

```json
{
  "Sand": "#D8C9AE",
  "Ink": "#1B1D26"
}
```

Keys are matched case-insensitively against the option value name. Define the metafield once under `Shopify admin > Settings > Metafields and metaobjects > Products`, then fill it in only on the products that need it.

### 3. The theme's built-in color names

If neither of the above is set, the theme recognizes around thirty common color names, in English and Spanish, and draws the chip from those.

This is a convenience, not a strategy: it covers the likes of `black`, `navy`, `beige`, `negro` and `crema`, and it will not know your house names.

### 4. Nothing

An option value the chain can't resolve falls back to a neutral chip with the value's name beside it. The picker still works; it just isn't visual for that value.

## Tips

- **Set Shopify's swatch data and stop there.** It is the only step of the four that is portable, that works for images as well as colors, and that doesn't need per-product work.
- **Use images for anything that isn't flat color.** A single hex for a leopard print or an oak veneer is worse than no swatch.
- **Be consistent within an option.** Half the colors as real swatches and half as neutral fallbacks looks broken, more than either would alone.
- **Treat the built-in dictionary as a safety net.** It stops a store looking unfinished before you have set anything up; it isn't meant to be the final state.

## Troubleshooting

- **A swatch shows as a plain chip with the name beside it.** Nothing in the chain resolved that value. Set it in Shopify's product options metafield, or add it to `pave.color_overrides` on that product.
- **The color is close but not right.** You are getting step 3, the built-in dictionary. Set the real value in Shopify's swatch data.
- **No swatches at all on cards.** Check **Show color swatches on cards** under [Product cards](../../theme-settings/product-cards/), and check the product's color option has one of the recognized names.

## Related

- [Variant picker](../../theme-settings/variant-picker/): swatch size, controls and out-of-stock behavior.
- [Product cards](../../theme-settings/product-cards/): swatches in grids.
- [Product media](../product-media/): variant images and how they're chosen.

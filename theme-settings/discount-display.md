---
title: Discount display
layout: default
parent: Theme settings
nav_order: 8
permalink: /theme-settings/discount-display/
---

# Discount display

These settings control how a reduced price is presented, everywhere one appears: product cards, product pages, featured products and the cart.

They govern **presentation only**. The discounts themselves are created under `Shopify admin > Discounts`, or by setting a compare-at price on a variant.

## Settings

- **Show discount badge.** Shows the discount badge wherever a reduced price appears. Default: on. Strikethrough prices still show when the badge is hidden.
- **Badge label format.** How badges are written. Default: **Minus percentage**.

  | Option | Reads as |
  |---|---|
  | Minus percentage | `-20%` |
  | Percentage off | `20% OFF` |
  | Save percentage | `SAVE 20%` |
  | Save amount | `SAVE $12.00` |

  When a product's variants are discounted by different amounts, the badge on its card reads `Up to` followed by the largest of them, in whichever format you chose.

- **Minimum discount to show badge.** Discounts below this percentage don't show a badge; the strikethrough price still appears. Range: 0% to 50%. Default: 0%, meaning every discount gets a badge.
- **Badge background color.** Defaults to the text color of the active color scheme. Set a color here to override it wherever the badge appears.
- **Badge text color.** Defaults to the surface color of the active color scheme. Keep a contrast ratio of at least 4.5:1 against the badge background.
- **Use a promotion label from product metafields.** Default: off. A product's promotion label replaces its sale badge, for offers set up outside Shopify discounts.

## Promotion labels from metafields

With **Use a promotion label from product metafields** on, the theme reads two metafields per product:

| Metafield | Type | Purpose |
|---|---|---|
| `pave.promo_label` | Single line text | The label to show instead of the sale badge |
| `pave.promo_percent` | Number | An optional percentage to include in the label |

Define them once under `Shopify admin > Settings > Metafields and metaobjects > Products`, then fill them in per product.

This is for offers Shopify's discount engine doesn't model: a bundle handled by an app, a members' price, a seasonal promotion run outside Shopify. A product with a promotion label set shows that label in place of its calculated sale badge.

## Tips

- **Set a minimum threshold.** A `−3%` badge draws attention to how small the saving is. Somewhere between 10% and 15% is where a badge starts to earn its space.
- **Leave the badge colors empty unless you have to change them.** Empty means the badge follows each section's color scheme, so it stays legible when a section is dark and when it is light. A fixed color is fixed everywhere, including on the scheme where it clashes.
- **If you do set them, check the contrast.** 4.5:1 between badge text and badge background. A red badge with white text often lands just under.
- **Hiding the badge doesn't hide the discount.** The compare-at price still shows struck through. Turning the badge off makes a store read quieter, not cheaper.

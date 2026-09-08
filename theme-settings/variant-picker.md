---
title: Variant picker
layout: default
parent: Theme settings
nav_order: 9
permalink: /theme-settings/variant-picker/
---

# Variant picker

How shoppers choose between variants — sizes, colors, materials — on every product page and featured product in the store. It is set once here rather than per product.

## Settings

- **Style** — Applies to every product page. The first three show color swatches at different sizes; the last replaces them with a menu, which suits catalogs with many variants. Default: **Pills with 32 x 32px swatches**.

  | Option | What it looks like | Suits |
  |---|---|---|
  | Pills with 32 x 32px swatches | Rounded pills, medium swatch | Most catalogs |
  | 44 x 44px swatches with labels | Large swatch with the value written beside it | Color-led catalogs where the shade is the decision |
  | Compact 24 x 24px swatches | Small swatch, tight row | Products with many colors |
  | Dropdown menu | A select menu, no swatches | Long option lists, or products with several option sets |

- **Show selected value next to the option name** — The option name reads `Color — Red` instead of `Color`. Default: on.
- **Out-of-stock variant style** — How unavailable combinations are presented. Default: **Strikethrough**.

  | Option | Behaviour |
  |---|---|
  | Strikethrough | Shown, struck through, still selectable |
  | Faded and not selectable | Shown, dimmed, can't be chosen |
  | Hidden | Removed from the picker entirely |

## Choosing an out-of-stock style

This is a merchandising decision more than a visual one.

**Strikethrough** is the default because it tells the shopper the size exists and is temporarily gone, and lets them select it to see the sold-out state and any back-in-stock offer. It is the most informative option.

**Faded and not selectable** is quieter and prevents dead ends, at the cost of the shopper not being able to confirm what they wanted.

**Hidden** makes a permanently discontinued variant disappear. Use it if your catalog carries variants you never intend to restock; avoid it for temporary stockouts, because a shopper who can't find their size assumes you never carried it.

## Swatches

The three swatch styles draw their colors from Shopify's swatch data. Setting that up — real colors, or images for patterns and materials — is covered in [Swatches](../../features/swatches/).

An option with no swatch data falls back to its name written in the pill, so the picker still works before you have set anything up.

## Tips

- **Match the swatch size to how much the color matters.** If shade is the purchase decision, 44 px with labels. If color is incidental, 24 px keeps the buy box short.
- **Dropdown when the list is long.** Past roughly a dozen values, swatches wrap into a block that pushes the add-to-cart button below the fold on mobile.
- **Leave the selected value on.** `Color — Sand` removes any doubt about which swatch is active, which matters most for the small swatch styles.
- **This is a store-wide setting.** There is no per-product override, so choose for the catalog you have most of.

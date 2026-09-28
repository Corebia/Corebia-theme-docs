---
title: Variant picker
layout: default
parent: Theme settings
nav_order: 15
permalink: /theme-settings/variant-picker/
---

# Variant picker

How shoppers choose between sizes, colors and materials, on every product page and featured product in the store. It is set once here rather than per product.

## Settings

- **Style.** Applies to every product page. The first three show color swatches at different sizes; the last replaces them with a menu, which suits catalogs with many variants. Default: **Pills with 32 x 32px swatches**.

  | Option | What it looks like | Suits |
  |---|---|---|
  | Pills with 32 x 32px swatches | Rounded pills, medium swatch | Most catalogs |
  | 44 x 44px swatches with labels | Large swatch with the value written beside it | Color-led catalogs where the shade is the decision |
  | Compact 24 x 24px swatches | Small swatch, tight row | Products with many colors |
  | Dropdown menu | A select menu | Long option lists, or products with several option sets |

- **Controls.** Default: **By option type**.
  - **By option type** gives color options swatches, size options buttons (or a menu with the **Dropdown menu** style) and every other option a menu.
  - **Same for every option** follows the style above for all options.
- **Show selected value next to the option name.** The chosen value appears beside the option name, so it reads `Color Sand` rather than `Color` on its own. Default: on.
- **Out-of-stock variant style.** How unavailable combinations are presented. It applies to swatches and buttons whose value has no in-stock variant with the other options chosen. Default: **Strikethrough**.

  | Option | Behavior |
  |---|---|
  | Strikethrough | Shown, struck through, still selectable |
  | Faded and not selectable | Shown, dimmed, can't be chosen |
  | Hidden | Removed from the picker. The selected value always stays, and an option with no available value at all keeps its values, struck through, so it is never left empty |

- **Remember the shopper's size.** Preselects the size a shopper last picked when they open another product. Stored in their browser only, and only when they allow preferences under your store's privacy settings. Default: on.

## Choosing the controls

**By option type** is the default because each kind of option gets the control that suits it: a shopper compares colors by eye, sizes at a glance, and reads through anything else, such as a material or a length.

**Same for every option** is for catalogs where that distinction gets in the way, for example products whose options are all short codes that read well as pills.

Pave recognizes color and size options by their names, in many languages (Color, Colour, Farbe, Size, Talla, Taille and others). A color option must be called by one of those names exactly; one named `Shade` or `Finish`, for example, is treated as an other option and shown as a menu under **By option type**.

## Choosing an out-of-stock style

This is a merchandising decision more than a visual one.

**Strikethrough** is the default because it tells the shopper the size exists and is temporarily gone, and lets them select it to see the sold-out state and any back-in-stock offer. It is the most informative option.

**Faded and not selectable** is quieter and prevents dead ends, at the cost of the shopper not being able to confirm what they wanted.

**Hidden** makes a permanently discontinued variant disappear. Use it if your catalog carries variants you never intend to restock; avoid it for temporary stockouts, because a shopper who can't find their size assumes you never carried it.

## Size memory

With **Remember the shopper's size** on, a shopper who picks `M` on one product finds `M` already selected on the next one that has it. It saves a tap on every product, and it avoids the classic mistake of adding the default size by accident.

The size is kept in the shopper's own browser, never sent to you, and only when their privacy preferences allow it. A shopper who has declined preferences cookies simply gets the normal picker.

## Swatches

The three swatch styles draw their colors from Shopify's swatch data. Setting that up, with real colors or with images for patterns and materials, is covered in [Swatches](../../features/swatches/).

A value with no swatch data and a color name the theme doesn't recognize shows a neutral striped chip, so the picker still works before you have set anything up. The value's name still shows next to the option name.

## Tips

- **Match the swatch size to how much the color matters.** If shade is the purchase decision, 44 px with labels. If color is incidental, 24 px keeps the buy box short.
- **Dropdown when the list is long.** Past roughly a dozen values, swatches wrap into a block that pushes the add-to-cart button below the fold on mobile.
- **Leave the selected value on.** Showing `Color Sand` removes any doubt about which swatch is active, which matters most for the small swatch styles.
- **Name your options plainly.** `Color` and `Size` get the right controls automatically. Creative option names lose them.
- **This is a store-wide setting.** There is no per-product override, so choose for the catalog you have most of.

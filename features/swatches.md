---
title: Swatches
layout: default
parent: Features
nav_order: 5
permalink: /features/swatches/
---

# Swatches

Pave's variant picker supports color swatches that display a colored chip or a small variant image alongside the option name, giving customers a visual way to pick variants.

## Where swatches appear

- The **Variant picker** block on the [Product page](../../templates/product-page/) and [Featured product section](../../sections/featured-product/).

## Configuring swatches

Swatches are powered by Shopify's product taxonomy and option metafields. There are two ways to set up swatches:

### Color name → automatic chip

When the option name is **Color**, Pave attempts to interpret common color names (black, white, red, navy, etc.) and render a colored chip automatically.

### Variant image → image swatch

If a variant has an image assigned (in `Shopify admin > Products > [product] > Variants > [variant] > Image`), Pave can use that image as the swatch chip.

## Variant picker settings

In the **Variant picker** block on the product page:

- **Type** — **Dropdown** (compact picker for many variants) or **Buttons** (visual buttons, the default for small variant counts).
- **Color option display** — **Color chip (dot + name)** shows the swatch alongside the color name. **Text buttons only** disables swatches and shows just text.

## Tips

- **Use the option name "Color"** for color options. Pave's swatch detection keys on this name. Variations like "Colour" (British spelling) or "Shade" do not trigger swatch rendering — rename them in your product admin.
- **Set a variant image for every color**, even if the only difference is the color. Without a variant image, the swatch falls back to a CSS chip and may not exactly match your product photography.
- **Don't mix swatch types in one option.** If half your colors have a variant image and half don't, the picker looks inconsistent. Either set images for all colors, or rely entirely on automatic chips.
- **Keep variant counts manageable.** A 30-color variant picker is overwhelming. Consider grouping related variants into a parent product and using a separate dropdown for shade.

## Troubleshooting

- **My swatches show as plain buttons** — Check that the option name is exactly "Color" and that **Color option display** is set to **Color chip (dot + name)** in the Variant picker block.
- **The color chip doesn't match my product** — The chip is generated from the color name. For exact matching, upload a variant image for that variant.
- **Swatches disappeared after a theme update** — Open the theme editor and reselect the **Variant picker** block to confirm settings still match. Swatch behavior is controlled by block settings.

## Related

- [Product page template reference](../../templates/product-page/) — Variant picker block reference.
- [Product media](../product-media/) — How variant images are configured.

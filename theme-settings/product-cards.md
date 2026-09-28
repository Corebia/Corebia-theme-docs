---
title: Product cards
layout: default
parent: Theme settings
nav_order: 14
permalink: /theme-settings/product-cards/
---

# Product cards

These settings apply to the product card wherever it appears: collection pages, the catalog, search results, New arrivals, recommendations, recently viewed and the search drawer. Setting them once here keeps every grid in the store consistent.

## Settings

- **Image ratio.** **Adapt to image**, **Portrait (3:4)**, **Square (1:1)** (default) or **Landscape (4:3)**.
- **Show quick add button.** Adds a `+` button to product cards. Products with one variant are added straight to the cart; products with several add the first available variant. Default: on.
- **Show an image carousel on cards.** Lets shoppers page through up to 5 of a product's images on the card with arrow buttons, without opening the product page. Products with one image are unchanged. Default: off.
- **Play a product video on card hover.** On a mouse, resting on a card plays the product's first video, muted and looping. Nothing is downloaded until the pointer arrives, and touch devices and shoppers who have asked for reduced motion see only a still frame. Default: off.
- **Show a quick view button on cards.** Lets shoppers open a product's media, price, options and add-to-cart in a popup from the grid, without leaving the page. Default: off.
- **Show a size selector on cards.** Shows up to 10 size values on a card as selectable buttons. Choosing one updates the card's price, availability and link to that variant; it doesn't add anything to the cart. Default: off.
- **Show color swatches on cards.** Shows up to 5 colors as selectable swatches. Choosing one updates the card's image, price and link. Any colors beyond the fifth are counted in a `+N` indicator. Default: on.
- **Show product rating on cards.** Shows stars and the number of reviews under the price. Needs a product reviews app that fills the product rating metafields; products without a rating show nothing. Default: off.
- **Days to show the new badge.** Products created within this many days show a **New** badge on cards. Range: 0 to 90 days. Default: 30. Set to 0 to hide the badge. The sale badge takes priority over the new badge.
- **Card style.** **Flat** (default) puts the card straight on the page background. **Bordered** draws a hairline around it, and **Card** gives it its own raised surface; both add padding inside the card.
- **Corner radius.** Range: 0 to 40 px in 2 px steps. Default: 0 px.
- **Text alignment.** **Left** (default), **Center** or **Right**.
- **Title case.** **Default** follows the Heading 6 case set under [Typography](../typography/). **Uppercase** applies to product card titles only. Default: **Default**.
- **Swatch width.** The size of the color swatches on product cards. The tap target around each swatch doesn't shrink with it. Range: 16 to 100 px. Default: 16 px.
- **Swatch height.** Range: 16 to 100 px. Default: 16 px.
- **Swatch corner radius.** Range: 0 to 100 px. Default: 100 px. At the default the corners follow the swatch: a circle when the width and the height match, an ellipse when they don't. Any other value is a corner radius in pixels, so 0 gives a square swatch.
- **Swatch border.** **None** or **Solid** (default). The border is what separates a pale swatch from the card behind it.
- **Swatch border width.** Shown when **Swatch border** is **Solid**. Range: 0 to 10 px in 0.5 px steps. Default: 1 px.
- **Swatch border opacity.** Shown when **Swatch border** is **Solid**. Lower values fade the border toward the card behind it. Range: 0% to 100%. Default: 100%.

The position, font and shape of card badges are set under [Badges](../badges/), and how the card moves on hover under [Animations](../animations/).

## Quick add, quick view and the size selector

The three shortcuts do different jobs:

- **Quick add** puts a product in the cart from the grid, choosing the first available variant for the shopper.
- **Quick view** opens the product in a popup so the shopper can choose a variant properly before adding.
- **The size selector** lets the shopper pick a size on the card itself, which then points the card's link and price at that size.

On collection and catalog pages, quick add is also controlled by the page's own section, which has its own **Show quick add button** setting. The button only shows there when both are on.

A card showing a size selector doesn't also show the quick view button, to keep the card uncluttered. The size selector finds the size option by its name (Size, Talla, Taille, Größe and others), so an option named anything else shows no selector.

## A note on Image ratio

**Adapt to image** keeps every product's own proportions, which is honest but gives an uneven grid unless your photography is already consistent. The three fixed ratios crop to a common shape, which is what makes a grid look deliberate.

If your catalog is shot to one standard, choose the ratio that matches it and nothing gets cropped. If it isn't, choose the ratio that suits most of it and set focal points on the images that suffer. See [Product media](../../features/product-media/).

## A note on swatches

Card swatches read a product's color option and show it as a real color or image. They rely on Shopify's swatch data, which is set per option value under `Shopify admin > Settings > Metafields and metaobjects`, or automatically from color names. See [Swatches](../../features/swatches/) for the full setup.

Products without a color option simply show no swatches; nothing needs turning off per product.

## Tips

- **Quick add earns its place on repeat-purchase catalogs.** Consumables, refills, basics. On a considered-purchase catalog it can short-circuit a decision the product page was going to help with.
- **Quick add on a multi-variant product picks the first available variant.** That is right for a product where the variants are sizes of the same thing, and wrong for one where they are meaningfully different. Quick view or the size selector suit those catalogs better.
- **30 days is a sensible new badge.** Long enough that a shopper sees it, short enough that it still means something. Stores that add stock rarely may want 60; stores adding daily may want 7.
- **Badges never stack.** A product that is both new and on sale shows the sale badge, because that is the one that moves a decision. See [which badge wins](../discount-display/#which-badge-wins).
- **Pick one card extra, not all of them.** A carousel, swatches, a size selector, ratings and a quick view button on one small card compete for the same space. Choose the one or two your catalog actually needs.
- **Hover video is for a few hero products.** It plays only on a mouse and only once the pointer arrives, so it costs nothing until then, but a whole grid of moving cards is tiring to scan.

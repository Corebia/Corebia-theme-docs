---
title: Featured product
layout: default
parent: Sections
nav_order: 16
permalink: /sections/featured-product/
---

# Featured product

**Featured product** puts one complete, buyable product anywhere sections are allowed: a home page, a landing page, a blog article. It is the product page's buy box, moved.

It carries the same blocks as the [Product page](../../templates/product-page/), including the variant picker, the buy buttons and app blocks, so a shopper can choose a variant and add to cart without leaving the page they're on.

It can't be placed in the header or footer groups.

## Settings

- **Product.** The product to feature.
- **Show back link and breadcrumb.** Default: on. Usually worth turning **off** here: on a home page there is nothing to go back to.

### Media

- **Desktop media width.** **Small**, **Medium** (default) or **Large**.
- **Desktop media position.** **Left** (default) or **Right**.
- **Desktop gallery layout.** **Stacked**, **2 columns**, **Thumbnails** (default) or **Thumbnail slideshow**.
- **Mobile layout.** **Show thumbnails** (default), **Hide thumbnails** or **2 columns**.
- **Use sticky product information on desktop.** Keeps the buy box in view while the media column scrolls. Default: on.
- **Use video looping.** Default: off.

### General

- **Color scheme.** Default: scheme-1.
- **Top padding** / **Bottom padding.** Range: 0 to 100 px in 4 px steps. Default: 36 px each.

## Blocks

The block set is identical to the product page's, and each block is documented once, there:

| Block | Limit |
|---|---|
| [Vendor](../../templates/product-page/#vendor) | 1 |
| [Heading](../../templates/product-page/#heading) | 1 |
| [Price](../../templates/product-page/#price) | 1 |
| [Text](../../templates/product-page/#text) | n/a |
| [SKU](../../templates/product-page/#sku) | 1 |
| [Inventory status](../../templates/product-page/#inventory-status) | 1 |
| [Variant picker](../../templates/product-page/#variant-picker) | 1 |
| [Buy buttons](../../templates/product-page/#buy-buttons) | 1 |
| [Product description](../../templates/product-page/#product-description) | 1 |
| [Collapsible tab](../../templates/product-page/#collapsible-tab) | n/a |
| [Pop-up](../../templates/product-page/#pop-up) | n/a |
| [Share](../../templates/product-page/#share) | 1 |
| [Product rating](../../templates/product-page/#product-rating) | 1 |
| [Icon with text](../../templates/product-page/#icon-with-text) | n/a |
| [Custom Liquid](../../templates/product-page/#custom-liquid) | n/a |
| App block | n/a |

## Tips

- **Trim the blocks.** A featured product doesn't need everything the product page carries. Heading, price, variant picker and buy buttons is usually the whole job; collapsible tabs and icon rows belong on the product page itself.
- **Turn off the back link and breadcrumb.** They are on by default because the same defaults serve the product page, where they belong.
- **Use it for one hero product**, a launch or a bundle. For a row of several products use [New arrivals](../new-arrivals/).
- **It is not a replacement for the product page.** Search engines index the product page, not this section, and shoppers arriving from Google land there.

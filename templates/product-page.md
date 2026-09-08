---
title: Product page
layout: default
parent: Templates
nav_order: 2
permalink: /templates/product-page/
---

# Product page

The product page is built from the **Main product** section: a media column and a buy box, where almost everything in the buy box is a block you add, remove and reorder.

Below it you can add any section that isn't restricted to the header or footer — [Product recommendations](../../sections/product-recommendations/), [Recently viewed](../../sections/recently-viewed/), [FAQ](../../sections/faq/) and the rest.

The same block set is available in [Featured product](../../sections/featured-product/), which puts a complete buy box on any other page.

## Section settings

- **Show back link and breadcrumb** — Default: on.

### Media

- **Desktop media width** — **Small**, **Medium** (default) or **Large**.
- **Desktop media position** — **Left** (default) or **Right**.
- **Desktop gallery layout** — **Stacked**, **2 columns**, **Thumbnails** (default) or **Thumbnail slideshow**.
- **Mobile layout** — **Show thumbnails** (default), **Hide thumbnails** or **2 columns**.
- **Use sticky product information on desktop** — Keeps the buy box in view while the media column scrolls. Default: on.
- **Use video looping** — Loops product videos. Default: off.

### General

- **Color scheme** — Default: scheme-1.
- **Top padding** / **Bottom padding** — Range: 0 to 100 px in 4 px steps. Default: 36 px each.

## Blocks

Add, remove and reorder these in the theme editor. The order you set is the order they appear in the buy box.

### Vendor

Limit 1. The product's vendor. No settings.

### Heading

Limit 1. The product title. No settings.

### Price

Limit 1.

- **Show compare-at price** — The struck-through original. Default: on.
- **Show discount badge** — Default: on. How the badge is written is set store-wide under [Discount display](../../theme-settings/discount-display/).
- **Tax note text** — Shown below the price when taxes are included. Default: `Tax included`. Leave blank to use the default translation.

### Text

A free line of copy in the buy box.

- **Text** — Inline rich text. Default: `Text block`.
- **Text style** — **Body** (default), **Subheading** or **Uppercase**.

### SKU

Limit 1.

- **Text style** — **Body** (default), **Subheading** or **Uppercase**.

### Inventory status

Limit 1.

- **Text style** — **Body** (default), **Subheading** or **Uppercase**.
- **Low inventory threshold** — Below this quantity the status switches to low stock. Range: 0 to 100. Default: 10.
- **Show inventory count** — Shows the actual number remaining. Default: on.

### Variant picker

Limit 1. The picker's appearance is set store-wide under [Variant picker](../../theme-settings/variant-picker/); these settings are about the size guide.

- **Size guide page** — Appears as a link next to the size option and opens in a popup. To use a different guide on one product, add the page metafield `custom.size_guide` to that product; it takes priority over this setting.
- **Size guide link label** — Default: `Size guide`.
- **Show size guide for all options** — Shows the link on every option, not only on options named Size. Default: off.

### Buy buttons

Limit 1.

- **Show quantity selector** — Default: on.
- **Show dynamic checkout buttons** — Using the payment methods available on your store, customers see their preferred option, like PayPal or Apple Pay. Default: on. See [Accelerated checkout](../../features/accelerated-checkout/).
- **Show recipient information form for gift card products** — Gift card products can optionally be sent direct to a recipient along with a personal message. Default: on. See [Gift cards](../../features/gift-cards/).

### Product description

Limit 1. The description from the product itself. No settings.

### Collapsible tab

An accordion row in the buy box. Add as many as you need.

- **Heading** — Leave blank to use the default heading for the type below.
- **Content type** — **Description**, **Composition and care**, **Shipping and returns**, or **Custom** (default). Choose a type to use its translated default heading, or Custom to write your own.
- **Use product description** — The tab shows the product description instead of the content below. Default: off.
- **Tab content** — Rich text.
- **Tab content from page** — If assigned, replaces the content above.

### Pop-up

A link in the buy box that opens a page's content in a modal.

- **Link label** — Default: `Size guide`.
- **Page** — The content of this page appears in the pop-up.

### Share

Limit 1.

- **Show label text** — Default: off.
- **Label** — Default: `Share`. See [Social sharing](../../features/social-sharing/).

### Product rating

Limit 1. Shows a product's star rating once the standard `reviews.rating` metafield holds a value. Nothing appears until a product has reviews. No settings.

### Icon with text

A row of up to three reassurance points — shipping, payment, returns.

- **Layout** — **Horizontal** (default) or **Vertical**.
- **Icon / image size** — Range: 16 to 48 px in 2 px steps. Default: 24 px.

Then the same four settings for each of the three points:

- **First heading**, **Second heading**, **Third heading** — Inline rich text. Defaults: `Shipping`, `Payment`, `Returns`.
- **First icon source**, **Second icon source**, **Third icon source** — **Upload image** (default) or **Built-in icon**.
- **First image**, **Second image**, **Third image** — Used when that source is Upload image.
- **First icon**, **Second icon**, **Third icon** — Used when that source is Built-in icon. Choose from Truck (shipping), Shield (security), Lock (secure payment), Leaf (sustainability), Package, Refresh (returns), Heart, Star, Check (guarantee), Clock (fast) and Credit card. Defaults: Truck, Shield, Refresh.

### Custom Liquid

- **Liquid code** — See [Custom Liquid](../../sections/custom-liquid/).

### App block

Any block offered by an app installed on your store, rendered inside the buy box.

## Alternate templates

To give some products a different layout, duplicate the product template in `Shopify admin > Online Store > Themes > … > Edit code`, or from the theme editor's template picker, and assign it per product under the product's **Theme template** setting.

## Tips

- **Order the blocks the way the decision is made.** Heading, price, variant picker, buy buttons is the spine. Everything else supports it and belongs below.
- **Sticky product information pays off on long pages.** With a tall media column, it keeps the add-to-cart button reachable without scrolling back.
- **Use collapsible tabs for what most shoppers skip.** Care instructions and returns policy belong there; the thing that sells the product does not.
- **Set the size guide once.** The section setting covers the whole catalog; the `custom.size_guide` metafield handles the products that need their own.
- **Three icons, not six.** The row is reassurance, not a feature list, and past three it stops being read.

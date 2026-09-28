---
title: Featured product
layout: default
parent: Sections
nav_order: 25
permalink: /sections/featured-product/
---

# Featured product

**Featured product** puts one complete, buyable product anywhere sections are allowed: a home page, a landing page, a blog article. It is the product page's buy box, moved.

It carries most of the blocks of the [Product page](../../templates/product-page/), including the variant picker, the buy buttons and app blocks, so a shopper can choose a variant and add to cart without leaving the page they're on. Until you pick a product, it shows a placeholder image and a prompt.

It can't be placed in the header or footer groups.

## Settings

- **Product.** The product to feature.
- **Show back link and breadcrumb.** The back link returns to the previous page in your store, and the breadcrumb traces the path from the home page. Default: on. Usually worth turning **off** here: on a home page there is nothing to go back to.

### Media

- **Desktop media width.** **Small**, **Medium** (default) or **Large**.
- **Desktop media position.** **Left** (default) or **Right**.
- **Desktop gallery layout.** **Stacked**, **2 columns**, **Thumbnails** (default) or **Thumbnail slideshow**. The layouts work as on the [Product page](../../templates/product-page/#media): **2 columns** puts a large first item over a two-column grid and hands over to the **Mobile layout** on phones.
- **Mobile layout.** **Carousel with dots** (default), **Carousel** or **2 columns**. Applies below 990 px. Shown for every desktop layout except **Stacked**, which shows every item on phones too.
- **Use sticky product information on desktop.** On screens 990 px and wider, keeps the buy box in view while the gallery scrolls. Default: on.
- **Use video looping.** Product videos, including YouTube and Vimeo, start again when they end. Default: off.

### General

- **Color scheme.** Default: scheme-1.
- **Top padding** / **Bottom padding.** Range: 0 to 100 px in 4 px steps. Default: 36 px each.

## Blocks

The product's media gallery is fixed in place and has no settings. Everything in the information column is a block you can add, remove and reorder. None of them has a limit, but most only make sense once.

### Vendor, Heading, Product description

No settings. They show the product's vendor, its title and its description.

### Price

- **Show compare-at price.** Default: on.
- **Show discount badge.** Default: on.
- **Tax note text.** Shown below the price when taxes are included. Leave blank to use the default translation. Default: `Tax included`.

### Text

- **Text.** Default: `Text block`.
- **Text style.** **Body** (default), **Subheading** or **Uppercase**.

### SKU

- **Text style.** **Body** (default), **Subheading** or **Uppercase**.

### Inventory status

- **Text style.** **Body** (default), **Subheading** or **Uppercase**.
- **Low inventory threshold.** Range: 0 to 100. Default: 10.
- **Show inventory count.** Default: on.
- **Show stock bar when stock is low.** Default: on.
- **Pre-order message.** Shown when a tracked variant has no stock but keeps selling, because **Continue selling when out of stock** is on for it. Default: `Pre-order: ships as soon as it's back in stock`.

### Variant picker

The picker's style is set once for the whole store, in the [Variant picker](../../theme-settings/variant-picker/) theme settings.

- **Size guide page.** Appears as a link next to the size option and opens in a popup. To use a different guide on one product, add the page metafield `custom.size_guide` to that product; it takes priority over this setting.
- **Size guide link label.** Default: `Size guide`.
- **Show size guide for all options.** Shows the size guide link on every option, not only on options named Size. Default: off.

### Buy buttons

- **Show quantity selector.** Default: on.
- **Show dynamic checkout buttons.** Shows the shopper's preferred payment method, such as PayPal or Apple Pay, from those available on your store. Default: on.
- **Show recipient information form for gift card products.** Lets a gift card be sent straight to a recipient with a personal message. Default: on.

### Personalization

A text field the shopper fills in before adding to cart, such as a monogram. What they type is shown in the cart and saved on the order.

- **Label.** The label above the field. Default: `Personalization`.
- **Property name.** The name the value is saved under on the order, for example `Monogram`. Default: `Personalization`.
- **Field type.** **Single line** (default) or **Multiple lines**.
- **Maximum characters.** Range: 5 to 250 in steps of 5. Default: 20.
- **Placeholder.** Example text inside the empty field.
- **Required.** Default: off.

### Collapsible tab

- **Heading.** Leave blank to use the default heading for the content type below.
- **Content type.** **Description**, **Composition and care**, **Shipping and returns** or **Custom** (default). Every type except Custom brings its own translated heading.
- **Use product description.** The tab shows the product description instead of the content below. Default: off.
- **Tab content.** Rich text. Hidden once a page is chosen below.
- **Tab content from page.** If assigned, replaces the content above.

### Pop-up

- **Link label.** Default: `Size guide`. Shown once a page is chosen.
- **Page.** The content of this page opens in a pop-up.

### Share

- **Show label text.** Default: off.
- **Label.** Default: `Share`. Shown when **Show label text** is on.

### Product rating

No settings. Shows the product's star rating once the standard `reviews.rating` metafield holds a value, which a reviews app fills in. Nothing appears until a product has reviews.

### Icon with text

Three short lines, each with an icon or an image, such as shipping, payment and returns.

- **Layout.** **Horizontal** (default) or **Vertical**.
- **Icon / image size.** Range: 16 to 48 px in 2 px steps. Default: 24 px.
- **First heading**, **Second heading**, **Third heading.** Defaults: `Shipping`, `Payment` and `Returns`.
- **First icon source**, **Second icon source**, **Third icon source.** **Upload image** (default) or **Built-in icon**.
- **First image**, **Second image**, **Third image.** Used with **Upload image**. Shown at the icon size and never cropped; a square image of at least 96 x 96 px stays sharp.
- **First icon**, **Second icon**, **Third icon.** Used with **Built-in icon**: **Truck (shipping)**, **Shield (security)**, **Lock (secure payment)**, **Leaf (sustainability)**, **Package**, **Refresh (returns)**, **Heart**, **Star**, **Check (guarantee)**, **Clock (fast)** or **Credit card**. Defaults: Truck, Shield and Refresh.

### Custom Liquid

The theme's shared [Custom Liquid block](../theme-blocks/#custom-liquid).

### App blocks

Any block offered by an app installed on your store.

A few product page blocks aren't offered here: **Previous / next product**, **Delivery estimate**, **Details** and **Ask a question**. They belong on a product's own page.

## Tips

- **Trim the blocks.** A featured product doesn't need everything the product page carries. Heading, price, variant picker and buy buttons is usually the whole job. The section starts with three collapsible tabs (description, composition and care, shipping and returns); remove the ones this placement doesn't need.
- **Turn off the back link and breadcrumb.** They are on by default because the same defaults serve the product page, where they belong.
- **Use it for one hero product**, a launch or a bundle. For a row of several products use [New arrivals](../new-arrivals/).
- **It is not a replacement for the product page.** Search engines index the product page, not this section, and shoppers arriving from Google land there.

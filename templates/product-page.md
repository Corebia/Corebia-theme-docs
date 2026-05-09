---
title: Product page
layout: default
parent: Templates
nav_order: 2
permalink: /templates/product-page/
---

# Product page

The **Product page** displays a single product with its media, variants, price, and purchase controls. It uses the `product.json` template, which is JSON-based and customizable from the theme editor.

## URL

`https://yourstore.com/products/<product-handle>`

## Sections included by default

1. **Main product** — The core product display: media, title, price, variants, buy buttons.
2. **Product recommendations** — Related products row.
3. **Complementary products** — Curated cross-sell row.
4. **Recently viewed** — Customer's recent product views.
5. **Rich text with image** — A storytelling block (defaults to "Our story").
6. **Customer reviews** — Placeholder section for reviews-app blocks.
7. **FAQ** — Three-question FAQ.

## Main product section

Inside the **Main product** section, blocks make up the product information layout. Add, remove, or reorder these blocks from the theme editor.

### Available blocks

- **Vendor** — Displays the product's vendor.
- **Title** — Displays the product title.
- **Price** — Displays the price, with optional compare-at price and discount badge.
  - **Show compare-at price** — Toggle.
  - **Show discount badge** — Toggle.
  - **Tax note text** — Text shown below the price when taxes are included. Defaults to a translated string. Default: `Tax included`.
- **Text** — A free-form text block. Pick a text style: **Body**, **Subtitle**, **Uppercase**.
- **SKU** — Displays the variant SKU. Same text style options.
- **Inventory status** — Shows in-stock state and an optional low-stock alert.
  - **Low inventory threshold** — Below this number, a low-stock indicator is shown.
  - **Show inventory count** — Toggle to display the exact count.
- **Quantity selector** — Lets the customer pick a quantity before adding to cart.
- **Variant picker** — The size, color, and other option pickers.
  - **Type** — **Dropdown** or **Buttons**.
  - **Color option display** — **Color chip (dot + name)** or **Text buttons only**.
  - **Size guide page** — Optional Shopify page that opens in a popup as a size guide. Appears as a link next to the size option.
  - **Size guide link label** — Default: `Size guide`.
  - **Show size guide for all options** — When enabled, shows the size guide link on every option row, not just size-named options.
- **Buy buttons** — The Add to cart button and dynamic checkout buttons.
  - **Show dynamic checkout buttons** — Adds Shop Pay, PayPal, Apple Pay, Google Pay buttons depending on what is enabled in your store.
  - **Show recipient information form for gift card products** — Lets gift card buyers enter recipient details.
- **Product description** — The product's HTML description from the Shopify admin.
- **Collapsible tab** — An expandable section. Multiple tabs stack vertically.
  - **Heading** — The tab heading. Leave blank to use the heading from the kind below.
  - **Kind** — Pick a kind to use a translated default heading, or pick **Custom** and provide your own heading. Options: **Description**, **Composition and care**, **Shipping and returns**, **Custom**.
  - **Use product description** — When enabled, this tab automatically displays the product description.
  - **Tab content** — Rich text content for the tab.
  - **Tab content from page** — If assigned, replaces the content above with a Shopify page's content.
- **Pop-up** — A link that opens a Shopify page in a popup.
  - **Link label** — Default: `Size guide`.
  - **Page** — The page whose content appears in the popup.
- **Share** — Native share button.
  - **Show label text** — Toggle.
  - **Label** — Default: `Share`.
- **Product rating** — Star rating from the `reviews.rating` metafield. Displays automatically when a product has reviews populated in the metafield reviews.rating (via the Shopify Product Reviews app or any compatible third-party reviews app). Nothing is shown until reviews exist.
- **Icon with text** — Up to three rows of an icon paired with a heading. Useful for trust signals (free shipping, secure checkout, easy returns).
  - **Layout** — **Horizontal** or **Vertical**.
  - **Icon / image size**.
  - For each of the three rows: heading, icon source (**Upload image** or **Built-in icon**), icon (one of: Truck, Shield, Lock, Leaf, Package, Refresh, Heart, Star, Check, Clock, Credit card), and an upload-image option.
- **Custom Liquid** — Free-form Liquid code for app snippets or custom HTML.
- **App blocks** — Compatible Shopify apps can expose blocks that drop in here.

### Section settings

Configure the layout of the Main product section:

- **Show back link and breadcrumb** — Toggle the breadcrumb at the top.
- **Desktop media width** — How wide the media column is. Options: **Small**, **Medium**, **Large**.
- **Desktop media position** — Whether media is on the **Left** or **Right**.
- **Desktop gallery layout** — How the media gallery is structured. Options: **Stacked**, **2 columns**, **Thumbnails**, **Thumbnail slider**.
- **Mobile layout** — How the gallery looks on mobile. Options: **Show thumbnails**, **Hide thumbnails**, **2 columns**.
- **Enable sticky product information on desktop** — When enabled, the product info column stays visible while the customer scrolls through media.
- **Enable video looping** — Auto-loop product videos.
- **Color scheme** — Default: scheme-1.
- **Top padding** and **Bottom padding**.

## Special behaviors

- **Variant images** — When the customer picks a variant that has its own image, the gallery jumps to that image. The URL also updates with the `variant=...` parameter so the customer can share a specific variant.
- **Cart updates without a page reload** — Clicking **Add to cart** updates the cart count in the header instantly.
- **Selling plans** — Subscription products display a selling plan picker above the buy buttons. See [Selling plans](../../features/selling-plans/).
- **Pickup availability** — When local pickup is configured for any of your store locations, a pickup availability box appears below the buy buttons. See [Pickup availability](../../features/pickup-availability/).
- **Shop Pay Installments** — When the customer's store and Shop Pay setup support installments, a Shop Pay Installments banner is rendered automatically below the buy buttons. See [Shop Pay Installments](../../features/shop-pay-installments/).

## Sections that can be added

In addition to **Main product**, you can add any of the following sections to the product page:

- [Product recommendations](../../sections/product-recommendations/)
- [Complementary products](../../sections/complementary-products/)
- [Recently viewed](../../sections/recently-viewed/)
- [Rich text with image](../../sections/rich-text-image/)
- [Customer reviews](../../sections/customer-reviews/)
- [FAQ](../../sections/faq/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Newsletter](../../sections/newsletter/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Order the blocks by purchase decision order.** Customers typically read in this order: image → title → price → variants → buttons → description → details. Don't bury price below the description.
- **Use Collapsible tabs for less critical info.** Composition, care, and shipping details are better collapsed than always-visible.
- **Trust signals matter.** The Icon with text block at the bottom of the description is a high-converting placement for shipping and returns reassurance.

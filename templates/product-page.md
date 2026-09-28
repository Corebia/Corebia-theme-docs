---
title: Product page
layout: default
parent: Templates
nav_order: 2
permalink: /templates/product-page/
---

# Product page

The product page is built from the **Main product** section: a media column and a buy box, where almost everything in the buy box is a block you add, remove and reorder.

The media column is a fixed block called **Media**. It is always there and has no settings of its own; the gallery is controlled by the section settings below.

The buy box blocks are shared with [Featured product](../../sections/featured-product/), which puts a complete buy box on any other page. Four blocks are only available here: **Previous / next product**, **Delivery estimate**, **Details** and **Ask a question**.

## What the default template contains

Out of the box, `product.json` shows the gallery as **2 columns** in a **Large** media column, which differs from the section's own defaults listed below, and lays out the buy box as Media, Previous / next product, Vendor, Heading, a Text block for the subtitle, Price, Variant picker, Inventory status, Buy buttons, Product description, Details, two Collapsible tabs (composition and care, then shipping and returns), Share, Pop-up and Ask a question.

Below the main section it adds:

- [Product recommendations](../../sections/product-recommendations/) in **Complementary products** mode, then again in **Related products** mode.
- [Recently viewed](../../sections/recently-viewed/), showing 8 products.
- [Customer reviews](../../sections/customer-reviews/).
- [FAQ](../../sections/faq/) with three example questions to replace.

Two of the default blocks are connected to Shopify's standard product metafields: the subtitle Text block reads **Subtitle** (`descriptors.subtitle`) and the composition and care tab reads **Care guide** (`descriptors.care_guide`). Fill those metafields on a product and the text appears. You can reconnect either block to a different source in the theme editor.

The Pop-up block ships with the label `Shipping & returns` and no page, so it stays hidden until you choose a page for it.

Any section that isn't restricted to the header or footer can be added below the main section, and so can [Quick order list](../../sections/quick-order-list/), which only product templates accept.

## Section settings

- **Show back link and breadcrumb.** The back link returns to the previous page in your store, and the breadcrumb traces the path from the home page. Default: on.

### Media

- **Desktop media width.** **Small**, **Medium** (default) or **Large**. The default product template ships with **Large**.
- **Desktop media position.** **Left** (default) or **Right**.
- **Extend media to screen edge.** Runs the media column out to the edge of the window on its own side, while the buy box stays aligned with the rest of the page. The back link and breadcrumb stay on the page margin, where they start on every other template. Default: on.
- **Desktop gallery layout.** **Stacked**, **2 columns**, **Thumbnails** (default) or **Thumbnail slideshow**. The default product template ships with **2 columns**.
  - **Stacked** shows every media item one under another, on phones too.
  - **2 columns** shows a large first item over a two-column grid. When the grid would leave the last item alone beside an empty cell, that item takes the full row. On phones it uses the **Mobile layout** below.
  - **Thumbnails** and **Thumbnail slideshow** show one large item with its thumbnails below, wrapped in rows or scrolled with arrows.

  In every layout, a link to a particular variant, such as a product card's link to one color, opens the gallery on that variant's image. See [Product media](../../features/product-media/#variant-images).
- **Mobile layout.** **Carousel with dots** (default), **Carousel** or **2 columns**. Applies below 990 px. Both carousels swipe through one item at a time, with or without position dots, and **2 columns** shows every item in a grid. Shown for every desktop layout except **Stacked**.
- **Use sticky product information on desktop.** On screens 990 px and wider, keeps the buy box in view while the gallery scrolls. Default: on.
- **Hide other variant media after one is selected.** Once a variant is picked, the gallery shows that variant's media and any media not attached to a variant, and hides the media of the other variants. If that would leave the gallery empty, it shows everything. Default: off.
- **Enable image zoom.** Adds a zoom button to each product image that opens it full screen. Videos and 3D models are not zoomed. Default: on.
- **Use video looping.** Product videos, including YouTube and Vimeo, start again when they end. Default: off.

### General

- **Color scheme.** Default: scheme-1.
- **Top padding** / **Bottom padding.** Range: 0 to 100 px in 4 px steps. Default: 36 px each.

## Blocks

Add, remove and reorder these in the theme editor. The order you set is the order they appear in the buy box. Any block can be added more than once, so keeping to one Heading and one Price is up to you.

### Previous / next product

Links to the previous and next product in the collection the shopper came from. It only appears when the product was opened from a collection, and at either end of the collection the missing link is left out. No settings.

### Vendor

The product's vendor. No settings.

### Heading

The product title. No settings.

### Price

- **Show compare-at price.** The struck-through original. Default: on.
- **Show discount badge.** Default: on. How the badge is written is set store-wide under [Discount display](../../theme-settings/discount-display/).
- **Tax note text.** Shown below the price when taxes are included. Default: `Tax included`. Leave blank to use the default translation.

### Text

A free line of copy in the buy box. Empty text renders nothing, which is what makes it useful for connecting to a metafield.

- **Text.** Inline rich text. Default: `Text block`.
- **Text style.** **Body** (default), **Subheading** or **Uppercase**.

### SKU

- **Text style.** **Body** (default), **Subheading** or **Uppercase**.

### Inventory status

Shows only for variants whose inventory Shopify tracks.

- **Text style.** **Body** (default), **Subheading** or **Uppercase**.
- **Low inventory threshold.** The low stock message shows when a variant has this many or fewer in stock. Range: 0 to 100. Default: 10.
- **Show inventory count.** Shows the actual number remaining. Default: on.
- **Show stock bar when stock is low.** Adds a short meter under the status while stock is at or below the threshold. Default: on.
- **Pre-order message.** Shown when a tracked variant has no stock but keeps selling because **Continue selling when out of stock** is on for it. Default: `Pre-order: ships as soon as it's back in stock`.

### Variant picker

The picker's appearance is set store-wide under [Variant picker](../../theme-settings/variant-picker/); these settings are about the size guide.

- **Size guide page.** Appears as a link next to the size option and opens in a popup. To use a different guide on one product, add the page metafield `custom.size_guide` to that product; it takes priority over this setting.
- **Size guide link label.** Default: `Size guide`.
- **Show size guide for all options.** Shows the link on every option, not only on options named Size. Default: off.

### Buy buttons

- **Show quantity selector.** Default: on. The selector respects the variant's quantity rules (minimum, maximum and increment), and when a variant has a rule or volume pricing, the block spells it out under the button. Both are set in Shopify for B2B catalogs.
- **Show dynamic checkout buttons.** Using the payment methods available on your store, customers see their preferred option, like PayPal or Apple Pay. Default: on. See [Accelerated checkout](../../features/accelerated-checkout/).
- **Show recipient information form for gift card products.** Gift card products can optionally be sent direct to a recipient along with a personal message. Default: on. See [Gift cards](../../features/gift-cards/).

When the selected variant is sold out, the Add to cart button, the quantity selector and the unbranded **Buy it now** button are all disabled and dimmed together. Wallet buttons such as Shop Pay keep Shopify's own disabled look.

The Shop Pay Installments message appears under the buttons whenever installments are on in your payment settings. See [Shop Pay Installments](../../features/shop-pay-installments/).

### Personalization

A text field the shopper fills in before adding to cart, such as a monogram or an engraving. What they type is saved on the cart line and on the order.

- **Label.** The field's label on the page. Default: `Personalization`.
- **Property name.** Shown in the cart and saved on the order, for example `Monogram`. Default: `Personalization`.
- **Field type.** **Single line** (default) or **Multiple lines**.
- **Maximum characters.** Range: 5 to 250 in steps of 5. Default: 20.
- **Placeholder.** Example text shown in the empty field.
- **Required.** The product can't be added to the cart until the field is filled. Default: off.

### Delivery estimate

Tells the shopper when an order placed now ships and when it should arrive, for example "Order by 14:00 to ship today" followed by an arrival range. The dates are worked out in the shopper's browser, so they stay current even though Shopify caches the page. The block hides itself while the selected variant is sold out.

- **Order cutoff.** Orders placed before this hour on a working day are processed that day. Every hour from **00:00** to **23:00**. Default: **14:00**.
- **Time zone.** The shop's time zone, in which the cutoff and working days are read. A list of 29 zones, from **UTC** (default) and **London (GMT/BST)** through to **Buenos Aires (ART)**.

#### Working days

- **Monday** to **Sunday.** The days you dispatch orders. Default: Monday to Friday on, Saturday and Sunday off.
- **Processing days.** Working days from the order day until the order ships. At 0 it ships on the order day. Range: 0 to 10. Default: 0.
- **Minimum transit days** / **Maximum transit days.** The carrier's delivery window: working days from shipping to the earliest and the latest delivery date. A maximum below the minimum counts as the minimum. Range: 0 to 30. Default: 2 and 5.
- **Holidays.** Days with no dispatch or delivery, one per line as `YYYY-MM-DD`, for example `2026-12-25`.

### Product description

The description from the product itself. No settings.

### Collapsible tab

An accordion row in the buy box. Add as many as you need. A tab with nothing in it is not shown.

- **Heading.** Leave blank to use the default heading for the type below.
- **Content type.** **Description**, **Composition and care**, **Shipping and returns**, or **Custom** (default). Choose a type to use its translated default heading, or Custom to write your own.
- **Use product description.** The tab shows the product description instead of the content below. Default: off.
- **Tab content.** Rich text. Hidden once a page is chosen below.
- **Tab content from page.** If assigned, replaces the content above.

### Details

Label and value rows, in the same accordion style as the collapsible tabs. The block is left out when it has no rows to show.

- **Heading.** Leave blank to use the default heading.
- **Show category attributes.** Adds a row for each apparel attribute set in the product's category metafields: fabric, color, pattern, neckline, sleeve length, fit, waist rise, top length and pants length. Default: on.

#### First row, Second row, Third row, Fourth row

Up to four rows of your own, each under its own header with the same two settings.

- **Label** / **Value.** A row shows when both its label and its value are filled. Connect a value to a metafield to vary it per product.

### Pop-up

A link in the buy box that opens a page's content in a modal. Nothing shows until a page is chosen.

- **Link label.** Default: `Size guide`. Leave it blank to use the page's title.
- **Page.** The content of this page appears in the pop-up.

### Ask a question

A link that opens a contact form in a modal, so a shopper can ask about this product without leaving the page. The message reaches you like any other contact form submission, with the product name, the selected variant and the product URL attached.

- **Link label.** Default: `Ask a question`.

### Share

- **Show label text.** Default: off.
- **Label.** Shown when the label is on. Default: `Share`. See [Social sharing](../../features/social-sharing/).

### Product rating

Shows a product's star rating once the standard `reviews.rating` metafield holds a value. Nothing appears until a product has reviews. No settings.

### Icon with text

A row of up to three reassurance points: shipping, payment, returns.

- **Layout.** **Horizontal** (default) or **Vertical**.
- **Icon / image size.** Range: 16 to 48 px in 2 px steps. Default: 24 px.

Then the same four settings for each of the three points:

- **First heading**, **Second heading**, **Third heading.** Inline rich text. Defaults: `Shipping`, `Payment`, `Returns`.
- **First icon source**, **Second icon source**, **Third icon source.** **Upload image** (default) or **Built-in icon**.
- **First image**, **Second image**, **Third image.** Used when that source is Upload image. Shown at the icon size and never cropped; a square image of at least 96 x 96 px stays sharp.
- **First icon**, **Second icon**, **Third icon.** Shown when that source is Built-in icon. Choose from **Truck (shipping)**, **Shield (security)**, **Lock (secure payment)**, **Leaf (sustainability)**, **Package**, **Refresh (returns)**, **Heart**, **Star**, **Check (guarantee)**, **Clock (fast)** and **Credit card**. Defaults: Truck, Shield, Refresh.

### Custom Liquid

- **Liquid code.** See [Custom Liquid](../../sections/custom-liquid/).

### App block

Any block offered by an app installed on your store, rendered inside the buy box.

## Alternate templates

Pave ships three alternate product templates, **editorial**, **gift-card** and **quick-order**, described in [Alternate product templates](../product-templates/). You can also create your own from the theme editor's template picker and assign it per product under the product's **Theme template** setting.

## Tips

- **Order the blocks the way the decision is made.** Heading, price, variant picker, buy buttons is the spine. Everything else supports it and belongs below.
- **Sticky product information pays off on long pages.** With a tall media column, it keeps the add-to-cart button reachable without scrolling back.
- **Use collapsible tabs for what most shoppers skip.** Care instructions and returns policy belong there; the thing that sells the product does not.
- **Set the size guide once.** The block setting covers the whole catalog; the `custom.size_guide` metafield handles the products that need their own.
- **Keep the delivery estimate honest.** Enter your real cutoff, working days and holidays. A promised date that slips costs more goodwill than no date at all.
- **Fill in category attributes in the admin.** The Details block builds its rows from the product category's attributes, so setting a product's category, fabric and fit pays off here with no extra work.
- **Three icons, not six.** The row is reassurance, not a feature list, and past three it stops being read.

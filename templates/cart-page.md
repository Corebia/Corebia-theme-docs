---
title: Cart page
layout: default
parent: Templates
nav_order: 9
permalink: /templates/cart-page/
---

# Cart page

The cart at `/cart`, using the **Main cart** section. Its own settings are only color and spacing, because what the cart shows is decided store-wide under [Cart settings](../../theme-settings/cart-settings/), and the same settings drive the cart drawer.

## Cart drawer or cart page

Under **Theme settings > Cart**, **Cart type** is **Drawer** by default: the cart icon and **Add to cart** open a panel over the current page, and the shopper can keep browsing. Set it to **Page** to send shoppers to `/cart` instead.

The cart page exists either way. With the drawer, a shopper still reaches it from the drawer's **View cart** link or by going to `/cart` directly, and the drawer never opens on top of the cart page itself.

## Section settings

- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 110 px each. This is the padding on screens 1920 px and wider; it scales down on smaller screens.

## Blocks

- **App block.** Any block offered by an installed app. Upsell, trust badge and shipping-estimate apps usually go here.
- **Custom Liquid.** See [Custom Liquid](../../sections/theme-blocks/#custom-liquid).

Blocks render below the cart, and they render on the empty cart too.

## What the cart shows

The page opens with a `Continue shopping` back link to your catalog of all products, in the same style as the back link on other pages, and the `Your cart` heading.

None of the rest are set on the cart page itself. Each appears when the store, the line item or a [Cart settings](../../theme-settings/cart-settings/) option calls for it.

- **Line items**, with image, options, any line item properties, an editable quantity and a remove control.
- **Subscription details**: the selling plan's name on any line bought on a plan. See [Selling plans](../../features/selling-plans/).
- **Unit prices** where a product has them. See [Unit pricing](../../features/unit-pricing/).
- **A free shipping bar**, when **Free shipping threshold** is set. It counts down to the threshold in the shopper's currency and confirms once it is reached.
- **Discounts**, named with their amount, and a **You're saving** line for savings on individual lines. See [Discount codes](../../features/discounts/).
- **A gift wrap checkbox**, when a **Gift wrap product** is chosen and available.
- **A discount code field**, when **Show discount code field** is on.
- **The subtotal**, followed by a Shop Pay Installments message when **Show Shop Pay Installments** is on and installments are enabled in your payment settings. See [Shop Pay Installments](../../features/shop-pay-installments/).
- **Check out** and **accelerated checkout buttons**, for whichever wallets your store accepts. See [Accelerated checkout](../../features/accelerated-checkout/).
- **A tax note**: `Tax included.` when your prices include tax, and `Tax excluded.` for B2B buyers whose prices exclude it.
- **Order notes**, a message to you that arrives with the order. The field is collapsed unless **Open the order note by default** is on, and a note the shopper has already written always shows.
- **Product suggestions**, when **Show product suggestions** is on: up to four products not already in the cart. A product on sale shows its compare-at price struck through, as on its product card.

## The empty cart

An empty cart shows `Your cart is empty` and a button to the catalog rather than a blank page. Choose an **Empty cart suggestions** collection under Cart settings to show up to four of its products below the message, headed by the collection's name. On the cart page that heading takes the size of a section heading; in the drawer it stays small.

## Tips

- **Keep app blocks modest.** They sit below the checkout button, which is right; an app that pushes a large widget there still competes with the thing the shopper came to do.
- **Don't hide the discount field if you run promotions.** A shopper with a code who can't find where to put it will leave the checkout to look for one.
- **Match the free shipping threshold to your shipping rate.** The bar is a promise. If it says free shipping and checkout charges for it, the bar has cost you the sale.
- **Order notes are read by you, not by Shopify.** Nothing acts on them automatically; they arrive with the order in your admin.
- **Test the cart with a subscription product** if you sell any. The plan name has to be right before a shopper commits to a recurring charge.

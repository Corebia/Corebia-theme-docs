---
title: Cart page
layout: default
parent: Templates
nav_order: 6
permalink: /templates/cart-page/
---

# Cart page

The cart uses the **Main cart** section. It has almost no settings, because nearly everything on it follows your store rather than the theme.

## Section settings

- **Color scheme.** Default: scheme-1.

## Blocks

- **App block.** Any block offered by an installed app. Upsell and shipping-estimate apps usually go here.
- **Custom Liquid.** See [Custom Liquid](../../sections/custom-liquid/).

## What the cart always includes

None of these need configuring; they appear when the store or the line item calls for them.

- **Line quantities**, editable in place, with a remove control.
- **Order notes**, for a message to you with the order.
- **A discount code field**, when **Show discount code field** is on under [Cart settings](../../theme-settings/cart-settings/).
- **Discounts**, shown per line and on the order total as they apply. See [Discount codes](../../features/discounts/).
- **Subscription details** on any line bought on a selling plan, showing the plan name and its delivery frequency. See [Selling plans](../../features/selling-plans/).
- **Unit prices** where a product has them, for markets that require price per unit. See [Unit pricing](../../features/unit-pricing/).
- **Accelerated checkout buttons**, showing whichever methods your store accepts. See [Accelerated checkout](../../features/accelerated-checkout/).
- **Taxes and shipping note**, as Shopify calculates them for the shopper's market.

## The empty cart

An empty cart shows a message and a route back to shopping rather than a blank page. It needs no setup.

## Tips

- **Keep app blocks below the totals.** An upsell above the checkout button competes with the thing the shopper came to do.
- **Don't hide the discount field if you run promotions.** A shopper with a code who can't find where to put it will leave the checkout to look for one.
- **Order notes are read by you, not by Shopify.** Nothing acts on them automatically; they arrive with the order in your admin.
- **Test the cart with a subscription product** if you sell any. The plan name and frequency have to be right before a shopper commits to a recurring charge.

---
title: Follow on Shop
layout: default
parent: Features
nav_order: 10
permalink: /features/follow-on-shop/
---

# Follow on Shop

The **Follow on Shop** button lets a shopper follow your store from the Shop app, Shopify's consumer mobile app. Followers get told about new products and can buy in a tap with Shop Pay.

## Where it appears

In the navigation panel of the [Header](../../sections/header/), when its **Show Follow on Shop** setting is on. That setting is on by default.

## What you need

Nothing beyond the setting. The button is rendered by Shopify, not by the theme, and needs no app installed. It relies on the Shop channel, which is on by default for stores accepting Shop Pay.

## What a shopper sees

A button carrying the Shop logo and wordmark, translated to their locale. Tapping it:

- **On mobile with the Shop app** — opens the app and follows your store.
- **On mobile without it** — offers to install the app, then follows.
- **On desktop** — opens Shop on the web, or shows a code to scan.

## Its colours can't be changed

The button is branded by Shopify, and the Theme Store requires that branded checkout and accelerator button colours are not modified. The theme sets none, and neither should any custom CSS you add.

## Tips

- **Leave it on.** Followers are a channel that costs nothing to maintain and that reaches people who chose to hear from you.
- **It complements email, it doesn't replace it.** Followers get app notifications; subscribers get email. Different people prefer each. See [Newsletter](../newsletter/).
- **Don't expect it to work in the theme editor preview.** Like most Shopify-rendered components, it behaves properly on the live storefront.

## Troubleshooting

- **The button doesn't appear** — check **Show Follow on Shop** in the Header section, then confirm Shopify Payments is set up, since Shop is part of that stack.
- **Nothing happens on desktop** — expected. Without the app, desktop opens Shop on the web or shows a QR code.

## Related

- [Header section reference](../../sections/header/)
- [Shopify Help: Shop app](https://help.shopify.com/manual/shop)

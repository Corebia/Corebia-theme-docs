---
title: Accelerated checkout
layout: default
parent: Features
nav_order: 11
permalink: /features/accelerated-checkout/
---

# Accelerated checkout

Accelerated checkout buttons let customers skip the standard checkout flow and pay in one or two taps using a stored payment method. Pave displays accelerated checkout buttons on both the product page and the cart page.

## Where they appear

- **Product page** — In the **Buy buttons** block, below the **Add to cart** button. Toggle with **Show dynamic checkout buttons**.
- **Cart page** — Below the main checkout button.

## Available payment methods

Which buttons appear depends on what is enabled in `Shopify admin > Settings > Payments`:

- **Shop Pay** — Shopify's accelerated checkout. Enabled by default with Shopify Payments.
- **Apple Pay** — On iOS Safari and macOS Safari, when Shopify Payments is enabled.
- **Google Pay** — On Android Chrome and desktop Chrome, when Shopify Payments is enabled.
- **PayPal** — When PayPal is enabled as a payment method in your store.
- **Amazon Pay** — When Amazon Pay is enabled.

Pave doesn't pick which buttons appear; Shopify makes the choice based on what is enabled and what the customer's device supports.

## Customer experience

- **One-tap purchase** — Customers with a stored payment method (for example, anyone who has used Shop Pay before) check out in one or two taps.
- **Skip the form** — Address, payment, and shipping are all populated from the stored payment profile.
- **Faster on mobile** — The biggest impact is on mobile, where typing checkout details on a small keyboard is the biggest source of cart abandonment.

## Tips

- **Leave dynamic checkout buttons on.** They are the single biggest mobile conversion driver in any modern Shopify theme. Disable only with strong reason.
- **Test on multiple devices.** The button set differs on iPhone (Apple Pay shown) vs. Android (Google Pay shown). Test on both.
- **Don't position the standard Add to cart below dynamic buttons.** The standard button is the fallback for customers without stored payment methods. Keeping it primary preserves the cart-then-checkout flow for that audience.

## Troubleshooting

- **No accelerated buttons appear** — Confirm Shopify Payments is enabled and that **Show dynamic checkout buttons** is on in the Buy buttons block. If only some buttons appear, that is expected — the set is device- and locale-specific.
- **PayPal button doesn't appear** — Enable PayPal in `Shopify admin > Settings > Payments > Alternative payment methods`.
- **Shop Pay button doesn't pre-fill payment** — The customer needs to be signed into Shop Pay or have a recognized device. First-time Shop Pay users still see a signup flow.

## Related

- [Product page > Buy buttons block](../../templates/product-page/)
- [Cart page template reference](../../templates/cart-page/)
- [Shop Pay Installments](../shop-pay-installments/)

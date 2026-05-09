---
title: Cart page
layout: default
parent: Templates
nav_order: 6
permalink: /templates/cart-page/
---

# Cart page

The **Cart page** is the dedicated review-and-edit page for the shopping cart. It uses the `cart.json` template.

Pave does not use a slide-out cart drawer; clicking the cart icon takes the customer to this dedicated page.

## URL

`https://yourstore.com/cart`

## Sections included by default

1. **Main cart** — The full cart with line items, totals, and checkout.
2. **Recently viewed** — A row of products the customer recently looked at.

## Main cart section

- **Color scheme** — Default: scheme-1.

The cart's structure (line items, quantities, totals, checkout button, dynamic checkout buttons) is built into the section and is not configurable from the editor.

## Special behaviors

- **Live cart updates** — Changing a quantity or removing a line updates the totals without a page reload.
- **Discount code field** — Shown when **Enable discount code field** is on in **Theme settings > Cart**. See [Discount codes](../../features/discounts/).
- **Selling plan summaries** — Subscription line items show their selected selling plan and the recurring delivery cadence. See [Selling plans](../../features/selling-plans/).
- **Accelerated checkout buttons** — Shop Pay, PayPal, Apple Pay, Google Pay buttons appear under the main checkout button when those payment methods are enabled in your store. See [Accelerated checkout](../../features/accelerated-checkout/).
- **Unit pricing** — When a product is configured with a unit price (per kg, per liter, per item), the unit price is shown next to the line item. See [Unit pricing](../../features/unit-pricing/).
- **Cart order note** — A free-form note field where customers can leave a message for you (gift wrapping, delivery instructions). The note travels through to the order in your admin.

## Sections that can be added

You can add any of these sections below the **Main cart** section:

- [Recently viewed](../../sections/recently-viewed/)
- [Product recommendations](../../sections/product-recommendations/)
- [FAQ](../../sections/faq/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Newsletter](../../sections/newsletter/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Recently viewed below the cart** is a high-converting placement — customers reviewing their order are primed to add one more item.
- **Empty cart state** — When the cart is empty, the section shows a clear empty state with a link back to the storefront.
- **Tax inclusion** — Whether prices on the cart show inclusive or exclusive of tax depends on your `Shopify admin > Settings > Taxes and duties` configuration.

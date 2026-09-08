---
title: Selling plans
layout: default
parent: Features
nav_order: 6
permalink: /features/selling-plans/
---

# Selling plans

Selling plans are Shopify's mechanism for subscriptions, prepaid plans, and any recurring or scheduled order arrangement. Pave displays selling plans on the product page, cart, and customer order detail pages.

## Where selling plans appear

- **Product page.** The selling plan picker appears in the **Variant picker** block. Customers choose between one-time purchase or one of the available subscription / scheduled options.
- **Cart page.** Each cart line item that has a selling plan shows the chosen plan name and the recurring schedule.
- **Customer order detail page.** Past orders with selling plans show the plan and the recurring details.

## Prerequisites

To use selling plans, you need a **subscription app** installed in your store. Shopify itself does not provide a subscription engine. Apps such as:

- **Shopify Subscriptions** (free, official Shopify app)
- Recharge
- Loop Subscriptions
- Bold Subscriptions

are the most common choices. Each app exposes selling plans that get attached to your products.

After the app is installed, configure plans:

1. Open the subscription app.
2. Create a selling plan group (for example, "Monthly delivery, 10% off").
3. Attach the plan group to the products you want to make subscribable.
4. Save.

Pave reads the selling plans from the products automatically, so no theme configuration is needed.

## How customers buy with a selling plan

1. On the product page, the customer sees a "One-time purchase" option and one or more selling plan options (e.g., "Subscribe and save 10%").
2. The customer picks an option.
3. The buy buttons reflect the selected plan and price.
4. After Add to cart, the cart shows the plan and recurring schedule on that line.
5. Checkout proceeds normally; the subscription is created on the first order.

## Customer subscription management

Customers manage their subscriptions through the subscription app, typically from a **Manage subscriptions** link on their order detail page or in their account. The exact UI depends on the app.

## Tips

- **Pick a single subscription app and stick with it.** Migrating between apps is painful, because selling plan IDs are app-specific.
- **Be explicit about the savings.** "Subscribe and save 10%" performs better than "Subscribe".
- **Allow easy cancellation.** Subscription apps that hide cancellation hurt long-term trust. Customers who can cancel easily come back.
- **Test the full flow** end-to-end before launching: pick plan, checkout, receive confirmation, find the manage-subscription link.

## Troubleshooting

- **No selling plan options appear on a product.** Confirm the product is included in a selling plan group inside the subscription app, and that the plan group is active.
- **Selling plan price isn't updating.** Hard refresh the storefront (`Ctrl+F5` / `Cmd+Shift+R`) to clear any cached price.
- **Customer can't manage their subscription.** Check the subscription app's customer-facing settings; some require a separate URL or a customer account login.

## Related

- [Product page template reference](../../templates/product-page/): Variant picker block.
- [Cart page template reference](../../templates/cart-page/)
- [Customer pages template reference](../../templates/customer-pages/)

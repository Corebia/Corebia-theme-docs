---
title: Discount codes
layout: default
parent: Features
nav_order: 13
permalink: /features/discounts/
---

# Discount codes

Pave supports the full Shopify discount stack: customer-typed discount codes, automatic discounts, and order-level discounts. Discounts are visible at every relevant step: cart, checkout, order summary, order confirmation, and customer order detail.

## Discount code field on the cart

When the **Show discount code field** setting is on, under **Theme settings > Cart**, the cart page displays a field where customers can enter a discount code before reaching checkout. The code is applied immediately, and the cart totals update.

See [Cart settings](../../theme-settings/cart-settings/).

## How savings are presented

The badge wording, its colours and the minimum discount worth badging are all set once under [Discount display](../../theme-settings/discount-display/), and applies to product cards, product pages, featured products and the cart alike.

That page also covers promotion labels driven by product metafields, for offers Shopify's discount engine doesn't model.

## Discount codes at checkout

Even if you've disabled the cart-side discount code field, customers can still enter codes at checkout. Shopify's checkout always shows a "Gift card or discount code" field.

## Automatic discounts

Automatic discounts (configured in `Shopify admin > Discounts`) are applied at checkout based on cart contents, with no code required. Pave displays automatic discount line items in the cart's order summary and on the cart page totals area.

## Discounts in the cart

When a discount code is applied successfully:

- The cart shows the savings as a discount line in the totals.
- Each affected line item shows the discounted price (with the original crossed out, when relevant).
- Removing or changing a line item recalculates the discount.

When a discount code is invalid:

- An inline error message is displayed.
- The cart totals do not change.

## Discounts at the order level

For percentage-off, fixed-amount-off, or buy-X-get-Y discounts that apply to the whole order, the discount appears as a single line in the cart's order summary, labeled with the code or the discount name.

## Tips

- **Keep the cart discount code field enabled** unless you have a specific reason. Customers who have a code in hand expect to apply it before checkout.
- **Use automatic discounts for storewide promotions** (free shipping, percentage off). Codes are best for personalized or campaign-specific offers.
- **Test code discount logic.** Buy-X-get-Y and complex stacking rules behave differently in cart vs. checkout. Walk a real product through the flow before launching a campaign.

## Troubleshooting

- **Customer reports the code is invalid.** Confirm the code is active, within its date range, and that any conditions (minimum spend, specific products, customer eligibility) are met.
- **Discount field doesn't appear on the cart page.** Confirm **Enable discount code field** is on in **Theme settings > Cart**.
- **Discount applied at checkout but not in cart.** Some discount types (like checkout-only buy-X-get-Y) don't pre-calculate in the cart. They appear at checkout. This is Shopify's behavior, not a theme bug.

## Related

- [Cart page template reference](../../templates/cart-page/)
- [Cart settings](../../theme-settings/cart-settings/)
- [Shopify Help: Discounts](https://help.shopify.com/manual/discounts)

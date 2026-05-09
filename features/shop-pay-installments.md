---
title: Shop Pay Installments
layout: default
parent: Features
nav_order: 9
permalink: /features/shop-pay-installments/
---

# Shop Pay Installments

Shop Pay Installments lets customers split the cost of a qualifying purchase into 4 interest-free payments or longer monthly installments. Pave displays the Shop Pay Installments banner on the product page, letting customers see the pay-in-installments option before checkout.

## Where it appears

- The [Product page](../../templates/product-page/), below the buy buttons. The banner reads "or 4 interest-free payments of $X.XX. [Learn more]" or similar, depending on the price and customer eligibility.

## Prerequisites

Shop Pay Installments is available only when:

- Your store uses **Shopify Payments** as a payment method (configured in `Shopify admin > Settings > Payments`).
- **Shop Pay** is enabled (also in **Settings > Payments**).
- Your store is in a [supported country](https://help.shopify.com/manual/payments/shop-pay-installments) (currently the United States and a few other markets — check the Shopify Help Center for the latest list).
- The product price is within the allowed range for installments (typically $50 to $20,000 for 4-payment plans; longer terms have different ranges).

If any of these conditions are not met, the banner is automatically hidden.

## How customers use it

1. The customer sees the banner on the product page.
2. They click **Add to cart** and proceed to checkout.
3. At checkout, they choose **Shop Pay** as the payment method.
4. They opt into installments and pick a plan.
5. The first payment is charged at order time; subsequent payments are scheduled.

## Customer experience

- **No interest, no fees** for 4-payment plans (depending on Shopify's installment policy at the time of writing — verify in Shopify Help Center).
- **Soft credit check** for longer-term plans; doesn't affect the customer's credit score.
- **Reminders** — Customers receive email and app reminders before each payment.

## Tips

- **Don't promise installments in product copy.** The banner is conditional. Stating "Buy now, pay later" in product descriptions sets expectations for customers who may not qualify.
- **Eligible products only** — Products under $50 don't qualify for 4-payment plans. The banner won't appear on cheap items, which is correct behavior.
- **Test with a US-based store** — If you're outside the US, you may not see the banner at all. That is expected.

## Troubleshooting

- **The banner doesn't appear** — Confirm Shopify Payments and Shop Pay are enabled, your store is in a supported country, and the product price is within the eligible range.
- **The banner shows the wrong plan** — Plans are calculated by Shopify based on the price. There's no theme-level configuration; if the wrong plan is shown, contact Shopify Support.

## Related

- [Product page template reference](../../templates/product-page/)
- [Accelerated checkout](../accelerated-checkout/) — Shop Pay button at checkout.
- [Shopify Help: Shop Pay Installments](https://help.shopify.com/manual/payments/shop-pay-installments)

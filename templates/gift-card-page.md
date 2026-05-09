---
title: Gift card page
layout: default
parent: Templates
nav_order: 13
permalink: /templates/gift-card-page/
---

# Gift card page

The **Gift card page** is the page a recipient lands on when they receive a gift card from your store. It displays the gift card amount, code, expiry, and a QR code, and offers an Apple Wallet pass on iOS devices.

This page uses the `gift_card.liquid` template (Liquid, not JSON). It is intentionally minimal and self-contained — it does not include the storefront header, footer, or navigation panel, so the recipient sees only the gift card itself. As a result, the page is not customizable from the theme editor.

## URL

The URL is unique per gift card and is delivered to the recipient by email when the gift card is purchased.

## What the page shows

- **Shop name** — Your store name.
- **Gift card image** — The gift card product's image, when one is set.
- **Recipient name and message** — When the buyer used the gift card recipient form on the product page.
- **Balance** — The current balance, plus the original (initial) value when the card has been partially used.
- **Code** — A copy-to-clipboard ready code that the recipient enters at checkout to redeem.
- **QR code** — A scannable QR code that resolves to the same gift card URL.
- **Apple Wallet button** — On iOS, a button to add the card to Apple Wallet (when the gift card has an `pass_url`, which Shopify provides automatically).
- **Expiry information** — The expiry date, an "expired" badge if applicable, or "no expiry".
- **Print button** — Triggers the browser print dialog with print-friendly formatting.
- **Shop now link** — A link back to your storefront.

## Sending a gift card

1. In your Shopify admin, create a gift card product (`Products > Add product > Product type: gift card` or use the gift card-specific flow).
2. The gift card product appears on your storefront like any other product.
3. When buying a gift card, the customer can optionally fill in recipient information (name, message) using the gift card recipient form, which appears when **Show recipient information form for gift card products** is enabled in the **Buy buttons** block on the [Product page](../product-page/).
4. After purchase, Shopify automatically emails the recipient with a link to the gift card page.
5. The recipient redeems the code at checkout.

## Tips

- **Test the flow** — Issue a gift card to your own email address and walk through the entire flow: receive email, open page, copy code, redeem at checkout.
- **Apple Wallet** — Only iOS Safari renders the Apple Wallet button as a working link. On other devices the button still appears if a pass URL exists, but tapping it is platform-dependent.
- **Print** — The print stylesheet hides the copy button and reformats the code box for legibility. If you offer physical gift cards, the print button is a quick way for customers to take the page to a printer.
- **Customize content via Shopify admin** — The customer-facing email content (which contains the gift card link) is edited in `Shopify admin > Settings > Notifications > Customer notifications > Gift card created`.

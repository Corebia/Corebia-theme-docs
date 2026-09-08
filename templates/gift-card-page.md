---
title: Gift card page
layout: default
parent: Templates
nav_order: 13
permalink: /templates/gift-card-page/
---

# Gift card page

The page a recipient lands on when someone buys them a gift card. It shows the balance, the code, a QR code for redeeming in person, and, on an iPhone, a button to add the card to Apple Wallet.

It is a Liquid template, `gift_card.liquid`, not a JSON one, so it has **no sections and no settings**. It follows your color scheme, fonts and logo automatically.

## What the page shows

- **The gift card image and the shop name.**
- **The recipient's name**, when the buyer entered one, as `To: <name>`.
- **The balance**, in the card's currency.
- **The gift card code**, with a **Copy code** button that confirms with `Copied!`.
- **A QR code**, captioned `Scan to redeem`, for redeeming in a physical store.
- **The expiry**, as either `Expires <date>` or `No expiration date`. An expired card shows an `Expired` badge and the date it lapsed.
- **Add to Apple Wallet**, on devices that support it.
- **Print gift card**, which uses a print stylesheet so the printed sheet carries the code and QR without the surrounding page.
- **Continue shopping**, back to the store.

## Enabling gift cards

Gift cards are a product type. Create one under `Shopify admin > Products > Add product` and set its type to gift card, or use Shopify's built-in gift card product. Nothing needs enabling in the theme.

For letting a buyer send a card straight to someone else with a message, see the **Show recipient information form for gift card products** setting on the [Product page](../product-page/#buy-buttons), and [Gift cards](../../features/gift-cards/).

## Tips

- **Test with a real card.** Issue one to yourself from `Shopify admin > Products > Gift cards`, open the link from the email, and check the QR scans and the Wallet button installs. It is the one page you can't preview meaningfully from the theme editor.
- **Print is not an afterthought.** A gift card is often printed and put in an envelope, so the printed version is part of the product.
- **There is nothing here to configure.** The page renders whatever the card holds, and Shopify controls that data. If it looks wrong, the cause is almost always the card rather than the theme.

---
title: Gift card page
layout: default
parent: Templates
nav_order: 16
permalink: /templates/gift-card-page/
---

# Gift card page

The page a recipient lands on when someone buys them a gift card. It shows the balance, the code, a QR code for redeeming in person, and, on an iPhone, a button to add the card to Apple Wallet.

It is a Liquid template, `gift_card.liquid`, not a JSON one, so it has **no sections and no settings**. It is deliberately plain: black text on white in the device's own system font, with your shop name at the top as text rather than your logo. Your color schemes, fonts and logo settings don't apply to it. It does follow the shopper's language, including right-to-left languages.

## What the page shows

- **The shop name and the gift card image.**
- **The recipient's name and message**, when the buyer entered them, as `To: <name>` followed by the message.
- **The balance**, in the card's currency.
- **The gift card code**, with a **Copy code** button that confirms with `Copied!`.
- **A QR code**, captioned `Scan to redeem`, for redeeming in a physical store.
- **The expiry**, as either `Expires <date>` or `No expiration date`. An expired card shows an `Expired` badge and the date it lapsed.
- **Add to Apple Wallet**, when Shopify offers a wallet pass for the card.
- **Continue shopping**, back to the store.
- **Print gift card**, which prints a clean sheet with the code and QR code and without the buttons.

## Enabling gift cards

Gift cards are a product type. Create one under `Shopify admin > Products > Add product` and set its type to gift card, or use Shopify's built-in gift card product. Nothing needs enabling in the theme.

For letting a buyer send a card straight to someone else with a message, see the **Show recipient information form for gift card products** setting on the [Product page](../product-page/), and [Gift cards](../../features/gift-cards/). Pave also ships a product template laid out for gift cards: see [Alternate product templates](../product-templates/#gift-card).

## Tips

- **Test with a real card.** Issue one to yourself from `Shopify admin > Products > Gift cards`, open the link from the email, and check the QR scans and the Wallet button installs. It is the one page you can't preview meaningfully from the theme editor.
- **Print is not an afterthought.** A gift card is often printed and put in an envelope, so the printed version is part of the product.
- **There is nothing here to configure.** The page renders whatever the card holds, and Shopify controls that data. If it looks wrong, the cause is almost always the card rather than the theme.

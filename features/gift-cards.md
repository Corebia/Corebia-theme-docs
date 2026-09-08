---
title: Gift cards
layout: default
parent: Features
nav_order: 7
permalink: /features/gift-cards/
---

# Gift cards

Pave fully supports Shopify's gift card feature: a dedicated gift card landing page, recipient personalization, QR code redemption, and Apple Wallet pass support on iOS.

## Selling gift cards

1. In your Shopify admin, go to **Products > Add product**, then choose **Gift card** as the product type (or use the gift card-specific flow under `Products > Gift cards`).
2. Set up denominations: $25, $50, $100, etc.
3. Save.

The gift card now appears on your storefront as a regular product. The customer adds a denomination to cart and checks out.

## Recipient personalization

Pave's product page supports the gift card recipient form. When the customer is buying a gift card product, they can enter:

- The recipient's name
- The recipient's email
- A personal message

To enable this on the product page, in the **Buy buttons** block, enable **Show recipient information form for gift card products**. See [Product page](../../templates/product-page/).

When configured, the recipient receives the gift card by email at the time chosen by the buyer.

## Gift card landing page

When the recipient receives the gift card, they land on a dedicated gift card page (uses the `gift_card.liquid` template). The page shows:

- Your shop name and the gift card image.
- The buyer's recipient name and message (if provided).
- The current balance and original value.
- A copy-to-clipboard ready code.
- A QR code that scans to the same URL.
- An "Add to Apple Wallet" button on iOS, when Shopify provides a pass URL.
- The expiry date or "no expiry".
- A print button for physical printout.

See the [Gift card page](../../templates/gift-card-page/) reference for full detail.

## Redeeming a gift card

The recipient redeems the card at checkout:

1. They visit your storefront, add products to cart, proceed to checkout.
2. At checkout, they enter the gift card code in the **Gift card or discount code** field.
3. The balance is applied to the order.

If the order total exceeds the gift card balance, the customer pays the remainder with another payment method.

## Tips

- **Test gift cards with a real card** issued to your own email. Walk through purchase, redemption, and balance tracking.
- **Set a realistic gift card image.** Uploading a branded gift card image (one image per denomination if you wish) makes the recipient page feel premium.
- **Configure the gift card email** in `Shopify admin > Settings > Notifications > Customer notifications > Gift card created`. The default Shopify template is functional but bland; brand it.
- **Disable expiry** unless you have a specific reason to expire cards. Many jurisdictions regulate gift card expiry; check with your jurisdiction's rules.

## Troubleshooting

- **The recipient form doesn't appear.** Confirm **Show recipient information form for gift card products** is enabled in the **Buy buttons** block, and that the product type is Gift card.
- **Apple Wallet button doesn't appear.** Apple Wallet passes are issued by Shopify; on iOS Safari, the button should appear automatically. On other browsers, the button is not interactive in the same way.
- **The QR code doesn't render.** The QR code uses the `qrcode.js` library shipped with the theme. If you've heavily customized the gift card template, ensure the script tag is intact.

## Related

- [Gift card page template reference](../../templates/gift-card-page/)
- [Product page > Buy buttons block](../../templates/product-page/)

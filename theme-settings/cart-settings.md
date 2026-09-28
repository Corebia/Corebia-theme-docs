---
title: Cart settings
layout: default
parent: Theme settings
nav_order: 11
permalink: /theme-settings/cart-settings/
---

# Cart settings

How the cart opens and what it offers alongside the items: a free shipping bar, product suggestions, gift wrap and Shop Pay Installments. The settings live in the **Cart** group of theme settings.

Pave has two carts that share these settings: the **cart drawer**, which slides in over the page, and the [Cart page](../../templates/cart-page/) at `/cart`. The cart drawer and the product suggestions inside it are sections with no settings of their own, so everything about them is configured here.

## Settings

- **Show discount code field.** Adds a discount code field to the order summary on the cart page. Shoppers can also enter codes at checkout. Default: on.
- **Cart type.** What happens when a shopper opens the cart. **Drawer** (default) slides the cart in over the current page; **Page** takes them to the cart page.
- **Open the cart drawer after adding to cart.** Shown when **Cart type** is **Drawer**. Default: on. Off: the cart count in the header bumps instead.
- **Free shipping threshold.** In your store's currency. Must match your free shipping rate's minimum order price. Default: 0, which hides the bar.
- **Free shipping thresholds in other currencies.** One line per currency, for stores that sell in more than one. See [Free shipping bar](#free-shipping-bar) below.
- **Show product suggestions.** In the cart drawer and on the cart page, up to 4 products not already in the cart. Default: on.
- **Suggested products.** The products to suggest. Empty: Shopify's recommendations for the first product in the cart.
- **Suggestions heading.** Shown when suggestions are on. Default: `You may also like`.
- **Gift wrap product.** Shows an **Add gift wrap** checkbox in the cart. Hidden while the product is unavailable.
- **Empty cart suggestions.** A collection. Up to 4 of its products appear under the empty cart message, in the cart drawer and on the cart page.
- **Open the order note by default.** On the cart page. Default: off. A note the shopper has written always shows.
- **Show Shop Pay Installments.** In the cart drawer and on the cart page. Shows only when Shop Pay Installments is on in your payment settings. Default: on.

## Drawer or page

The drawer keeps shoppers where they were. They add a product, see the cart confirm it, and carry on browsing, which suits stores where people buy several things at once.

The page gives the cart room: order notes and the discount code field are only on the cart page, not in the drawer. With **Cart type** set to **Drawer**, the cart page still exists and the drawer links to it, so a shopper who wants the full view can get there.

With **Open the cart drawer after adding to cart** off, adding a product doesn't interrupt the shopper at all. Only the count on the header's cart icon changes, and the drawer opens when they click it.

## Free shipping bar

A progress bar in the cart that tells the shopper how much more to spend for free shipping, and confirms it once they have reached it. It appears only when the cart has items.

The bar compares the cart total after discounts with your threshold. It doesn't read your shipping rates, so **the threshold has to match the minimum order price of your free shipping rate** in `Shopify admin > Settings > Shipping and delivery`. If the two disagree, the cart promises something checkout doesn't deliver.

**Free shipping threshold** is in your store's own currency. For shoppers browsing in another currency, add a line per currency to **Free shipping thresholds in other currencies**:

```
EUR 49.50
GBP 45
CAD 75
```

- The currency code, a space, then the amount.
- Digits, with a point for decimals and no thousands separators: `EUR 1000`, not `EUR 1,000`.
- Each amount must match the minimum order price of that market's free shipping rate.
- Amounts are never converted. A currency without a line shows no bar, and a line the theme can't read is ignored.

## Product suggestions

Suggestions sit below the cart items, each with its price and an **Add** button, and leave out anything already in the cart. A product on sale shows its compare-at price struck through beside the sale price, as it does on a product card. Set **Suggested products** to choose them yourself, such as small add-ons that suit almost any order. Leave it empty and Shopify's recommendations for the first product in the cart are used instead.

**Empty cart suggestions** are separate. They fill the empty cart, in the drawer and on the page, so a shopper who opens it with nothing inside has somewhere to go.

## Gift wrap

Create gift wrap as an ordinary product with a price, then choose it in **Gift wrap product**. The cart shows an **Add gift wrap** checkbox with the price; ticking it adds the product's first available variant to the cart, and unticking removes it.

While no variant of the product is available to buy, the checkbox disappears, so a shopper is never offered wrap you can't add.

## What the cart does without any settings

Some of the cart's behavior isn't configurable, because it follows your store rather than the theme. Both carts include:

- **Line-item and order-level discounts**, shown as they are applied.
- **Subscription details** on any line bought on a selling plan.
- **Unit prices** where a product has them.
- **Accelerated checkout buttons**, showing whichever methods your store accepts.

The cart page also includes **order notes**, for a message to you with the order.

## Should the discount code field be on?

Turning it **on** is right for most stores. Shoppers who have a code will look for somewhere to enter it, and a cart with nowhere to do so sends them out to search for one, which often means leaving to find a coupon site.

Turning it **off** makes sense in two cases: if you never run code-based discounts, so the field is an empty invitation to go looking for one; or if you rely on automatic discounts, which apply without a code and show in the cart on their own.

Codes can still be applied at checkout either way. Hiding the field here doesn't disable discounts. See [Discount codes](../../features/discounts/).

## Tips

- **Set the free shipping threshold to your real rate, then leave it.** Change the rate in Shopify and the bar here in the same sitting.
- **Suggest cheap, universal add-ons.** Socks, care products, gift cards. A suggestion that costs more than the cart is a distraction.
- **Give the gift wrap product a clear image and title.** It appears as a cart line like any other, and in the order you receive.
- **Automatic discounts don't need the field.** They apply themselves and appear in the cart totals.
- **If you turn the field off, say so.** A store that runs promotions but hides the field will get support messages asking where to put the code.

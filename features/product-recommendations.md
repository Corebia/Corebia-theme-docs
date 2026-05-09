---
title: Product recommendations
layout: default
parent: Features
nav_order: 3
permalink: /features/product-recommendations/
---

# Product recommendations

Pave supports two kinds of cross-sell on the product page: **related products** (algorithmic) and **complementary products** (manually curated).

## Related products

Pave fetches related products using Shopify's recommendations API with `intent: related`. Shopify uses purchase history, product metadata, and store-wide browsing patterns to surface relevant products.

### Where it appears

- The [Product recommendations section](../../sections/product-recommendations/), placed by default on the product page below the description.

### How to influence the recommendations

- **Build purchase history.** Shopify learns from real orders. New stores have thin recommendation data; recommendations get sharper as orders accumulate.
- **Manually pin products** with the **Search & Discovery** app, in `Shopify admin > Apps > Search & Discovery > Recommendations`. You can override the algorithm for specific products.
- **Hide the section** if your store is brand new and the algorithmic results aren't useful yet — you can re-enable it later.

## Complementary products

Complementary products are manually curated cross-sells: products that complete a look or purchase. Unlike related products, they are not algorithmic — you choose them.

### Where they appear

- The [Complementary products section](../../sections/complementary-products/), placed by default on the product page.

### How to configure

1. Install the **Search & Discovery** app from the Shopify App Store (free, official Shopify app).
2. Open `Shopify admin > Apps > Search & Discovery > Product recommendations`.
3. Pick a source product.
4. Add complementary products.
5. Save.

If a source product has no complementary products configured, the section is hidden automatically on that product's page.

## Troubleshooting

- **No recommendations appear** — A new store with few orders has thin algorithmic data. Add complementary products manually in the meantime.
- **The section disappears on some products** — That product has no recommendations or complementary picks configured. This is the expected behavior — Pave hides empty sections rather than showing placeholder UI.
- **I added complementary products but don't see them** — Wait a few minutes for Shopify's API to propagate, then refresh the storefront with a hard refresh (`Ctrl+F5` / `Cmd+Shift+R`).

## Related

- [Product recommendations section](../../sections/product-recommendations/)
- [Complementary products section](../../sections/complementary-products/)
- [Recently viewed section](../../sections/recently-viewed/) — Different mechanism, surfaces the customer's own browsing history.

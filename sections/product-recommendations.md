---
title: Product recommendations
layout: default
parent: Sections
nav_order: 15
permalink: /sections/product-recommendations/
---

# Product recommendations

The **Product recommendations** section displays products related to the one the customer is currently viewing. Pave fetches recommendations from Shopify's recommendations API, which uses purchase history and product metadata to surface relevant products.

It is typically placed below the product description on the product page.

## Settings

- **Heading** — The section heading. Default: `You may also like`.
- **Subheading** — Optional supporting text.
- **Heading alignment** — Options: **Left**, **Center**, **Right**.
- **Maximum products to show** — Cap on how many products to display.
- **Number of columns on desktop** — Range: 2 to 5.
- **Color scheme** — The color scheme applied to the section. Default: scheme-1.

## How recommendations are generated

Pave requests recommendations with `intent: related`. Shopify uses your store's purchase history and product graph to return products commonly bought, viewed, or related to the current product.

If you want to influence the recommendations:

- **Install the Shopify Search & Discovery app** (free) and use its **Recommendations** tools to manually pin specific products to specific source products.
- **Build purchase history** — New stores have thin recommendation data. As orders accumulate, recommendations become more relevant.

If no recommendations are available (for example, on a brand-new store), the section is hidden automatically.

## Tips

- **Place below product description** — Customers who finish reading about a product are primed to discover similar ones.
- **Cap at 4–6 products** — Too many recommendations dilute the suggestion.
- **Use on product pages only.** Recommendations are calculated relative to the current product; on other pages, the API has no source product to work with.

## Related

- [Complementary products](../complementary-products/) — Manually curated cross-sell, distinct from the algorithmic related recommendations.
- [Recently viewed](../recently-viewed/) — A history-based alternative that doesn't require the algorithm.

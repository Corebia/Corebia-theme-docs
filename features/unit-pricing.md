---
title: Unit pricing
layout: default
parent: Features
nav_order: 12
permalink: /features/unit-pricing/
---

# Unit pricing

Unit pricing displays the price per unit of measurement (per kg, per liter, per item) alongside the regular price. Required by law in some jurisdictions for groceries, cosmetics, and bulk goods. Pave shows unit pricing wherever a price is displayed.

## Where it appears

- Product cards in collection grids and the search page.
- The product page price.
- Cart line items.
- Order confirmation pages.

## Configuring unit pricing for a product

1. In `Shopify admin > Products > [product] > Variants > [variant]`, expand the variant.
2. Scroll to **Unit price**.
3. Enable **Show unit price**.
4. Enter the **Unit price measurement**:
   - **Reference value** — The numeric quantity the unit price refers to (for example, 100 for "per 100 g").
   - **Reference unit** — The unit of measurement (g, kg, mL, L, pieces).
   - **Total quantity** — The total quantity in the package (for example, 500 for a 500 g item).
   - **Total unit** — The unit (g, kg, mL, L, pieces).
5. Save.

Pave reads these values and renders the unit price automatically. For a 500 g item priced at €10 with a reference of 100 g, the unit price displays as `€2.00 / 100 g`.

## Tips

- **Use units that customers expect.** Cosmetics in the EU are typically priced per 100 ml; bulk grain per kg.
- **Be consistent across the catalog.** Mixing units (some products per kg, some per 100 g for the same category) confuses customers comparing.
- **Required by law** — In the EU, the [Unit Price Directive](https://eur-lex.europa.eu/eli/dir/1998/6/oj) requires unit prices for many product categories. Check the regulations for the markets you sell in.

## Troubleshooting

- **Unit price doesn't appear on a product** — Confirm **Show unit price** is enabled on the variant and that all four fields are filled in.
- **The unit price calculation looks wrong** — Verify the **Reference value**, **Reference unit**, **Total quantity**, and **Total unit** are correctly set. The calculation is `(price / total quantity) × reference value`.

## Related

- [Product page template reference](../../templates/product-page/)
- [Cart page template reference](../../templates/cart-page/)

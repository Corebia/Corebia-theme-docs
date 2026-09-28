---
title: Quick order list
layout: default
parent: Sections
nav_order: 32
permalink: /sections/quick-order-list/
---

# Quick order list

**Quick order list** shows every variant of a product in one table, with a quantity field on each row, so a buyer can order several sizes or colors in one pass instead of picking them one at a time. It is built for wholesale and B2B buying, where one order often covers a whole size run.

It can only be added to product templates. The theme ships a ready-made one, `product.quick-order`, described in [Alternate product templates](../../templates/product-templates/#quick-order).

## Settings

- **Variants per page.** Range: 5 to 50 in steps of 5. Default: 50. A product with more variants than this gets previous and next page links under the table.
- **Show variant images.** Default: on. Shows the variant's own image beside its name, when it has one.
- **Show SKU.** Default: off.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 40 px each.

## How it works

- **Each quantity field is the cart.** Typing a quantity sets that variant's quantity in the cart straight away, and setting it to 0 removes it. There is no separate "add all" button. The table opens with whatever is already in the cart filled in.
- **Totals for this product.** Under the table, the number of items and the subtotal for this product's variants in the cart, with **Remove all** and **View cart** buttons.
- **Quantity rules and volume pricing.** When a variant has a minimum, maximum or increment, the field follows it and the rules are written under it. When it has quantity price breaks, a small volume pricing table appears under its price.
- **Sold-out variants** are listed with the field disabled and marked **Sold out**.

## Who sees what

The section isn't limited to B2B customers. Anyone who opens a product on a template carrying it sees the table.

What changes for a B2B buyer is the data. Quantity rules and volume pricing are set in a B2B catalog in Shopify admin, so they only exist for buyers logged in to a company location that uses that catalog. Other shoppers see the same table with your regular prices and no rules. That is usually fine, but it is the reason to assign the quick order template only to products you sell in volume.

## Tips

- **Assign it per product.** Open the product in Shopify admin and choose `product.quick-order` under **Theme template**. Products that sell one at a time are better served by the regular product page.
- **Keep the variant names short.** The name column is the only way a buyer tells rows apart, and long option combinations wrap on a phone.
- **Turn on Show SKU for trade buyers.** Buyers ordering from a list or a purchase order often work by SKU.
- **Set quantity rules in the B2B catalog, not in the product description.** The table enforces them; a sentence in the description doesn't.

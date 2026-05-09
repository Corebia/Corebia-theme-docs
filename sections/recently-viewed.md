---
title: Recently viewed
layout: default
parent: Sections
nav_order: 13
permalink: /sections/recently-viewed/
---

# Recently viewed

The **Recently viewed** section shows products the customer has previously visited on your store. Useful on the cart page or the product page to remind customers of items they considered.

The section is hidden when the customer has no view history (for example, on a first visit).

## Settings

- **Heading** — The section heading. Default: `Recently viewed`.
- **Subheading** — Optional supporting text.
- **Heading alignment** — Options: **Left**, **Center**, **Right**.
- **Maximum products to show** — Cap on how many products to display.
- **Show vendor** — When enabled, displays the product vendor on each card.

The section also exposes spacing settings.

## How recently viewed is tracked

Pave stores recently viewed product handles in the customer's browser (`localStorage`). Each product page visit appends to the list. The section reads that list on render and pulls the corresponding products from Shopify.

This means:

- **No login required** — Tracking works for guests and signed-in customers.
- **Local to the browser** — Customers who switch devices or browsers do not see their previous history on the new device.
- **Cleared with browser data** — Clearing the browser's storage clears the recently viewed list.

## Tips

- **Cart page is the highest-converting placement.** Customers reviewing their cart often add one more item.
- **Cap at 4–8 products.** More than 8 turns the section into an unfocused grid.
- **Hide on the home page.** First-time visitors with no view history would see an empty section. Use it on cart and product pages where the customer has navigated to multiple products.

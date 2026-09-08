---
title: Pickup availability
layout: default
parent: Features
nav_order: 8
permalink: /features/pickup-availability/
---

# Pickup availability

When local pickup is configured for any of your store locations, Pave automatically displays a pickup availability section on the product page so customers know which locations have the variant in stock.

## Where it appears

- The [Product page](../../templates/product-page/), below the buy buttons.

## Prerequisites

To enable pickup availability:

1. Go to `Shopify admin > Settings > Shipping and delivery`.
2. Under **Local pickup**, click **Manage** for each location where you want to offer pickup.
3. Enable local pickup, set pickup-ready time estimates and instructions, and save.

Once configured, Pave automatically renders the availability section on every product page where at least one location offers pickup.

## What customers see

For the currently selected variant, Pave shows:

- Whether the variant is **available** at the nearest pickup location.
- The pickup-ready time estimate (for example, "Usually ready in 24 hours").
- A "Check availability at other locations" link that opens a popup listing every pickup-enabled location and the variant's stock status at each.
- The pickup instructions, if you've configured any.

When the customer changes variant, the availability re-fetches and updates.

## Out-of-stock variants

If a variant is out of stock at every pickup location, the availability section shows that the variant is currently unavailable for pickup. Customers can still order with shipping if shipping is configured.

## Tips

- **Enable pickup at every location where you can fulfill it.** Even if your warehouse can't easily handle pickup, enabling it for one or two locations adds a fast option for nearby customers.
- **Set realistic pickup-ready times.** "Usually ready in 24 hours" sets expectations. "Usually ready in 1 hour" promises the customer something they may not get on busy days.
- **Be specific in pickup instructions.** "Use the front entrance, ask for [name]" is more useful than "Pickup available". Custom instructions appear after the customer places the order.

## Troubleshooting

- **The pickup section doesn't appear.** Confirm at least one location has local pickup enabled. If no location has pickup enabled, the section is hidden.
- **The wrong location appears as nearest.** Pave displays the location based on Shopify's data. Customers can click "Check availability at other locations" to see all locations.
- **Variant shows as unavailable but I have stock.** Confirm the variant is assigned inventory at the pickup location in `Shopify admin > Products > [product] > Inventory`.

## Related

- [Product page template reference](../../templates/product-page/)

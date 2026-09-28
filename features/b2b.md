---
title: B2B
layout: default
parent: Features
nav_order: 18
permalink: /features/b2b/
---

# B2B

Pave supports Shopify's B2B features: company accounts with their own locations, quantity rules, volume pricing and tax-exclusive prices. Everything on this page appears only for a signed-in buyer who belongs to a company, so retail shoppers and guests see the storefront exactly as before.

Companies, locations, catalogs, quantity rules and price breaks are all set up in your Shopify admin under `Customers > Companies` and `Products > Catalogs`. The theme reads what you set there and has no B2B settings of its own, apart from the quick order list below. Which B2B features your store can use depends on your Shopify plan.

## Company and location in the header

A B2B buyer sees who they are buying for: the company and location name, in the header's navigation panel and, from 990 px up, beside the account icon in the header bar. When the buyer has access to more than one location, the panel lists the others, and choosing one makes it the current location. Prices, catalogs and payment terms then follow that location.

Only the company and location names are shown. Tax registration numbers, addresses and other company details never appear in the storefront.

## Quantity rules

When a variant has a quantity rule in its B2B catalog, the quantity selector on the product page respects it: it starts at the minimum, steps by the increment and stops at the maximum. The rule is written out under the selector, for example `Minimum of 6` and `Increments of 6`, so a buyer knows why the number jumps.

## Volume pricing

When a variant has price breaks, the buyer sees them before adding to cart:

- **The price** reads `From` the lowest break price, with `Volume pricing available` under it. This applies on the product page and on product cards in every grid. A variant on sale keeps its struck-through compare-at price.
- **A Volume pricing table** on the product page lists each quantity from the minimum up, with its price per item.

## Quick order list

The **Quick order list** section puts every variant of a product in one table, so a buyer can order several sizes or colors at once instead of adding them one by one. Each row has its own quantity field that follows the variant's quantity rule, shows how many are already in the cart and the row total, and carries the variant's volume pricing. Under the table are the product's totals, a link to the cart and a **Remove all** button that clears the product from the cart.

Quantities go straight into the cart as the buyer types, so there is no add-to-cart button to press.

The section can only be placed on product templates. The theme ships one ready to use:

1. In `Shopify admin > Products`, open a product with many variants.
2. Under **Theme template**, choose `quick-order`.
3. Save. That product's page now shows the quick order list under the product information.

See [Quick order list](../../sections/quick-order-list/) for its settings and [Alternate product templates](../../templates/product-templates/#quick-order) for the template.

## Tax-exclusive prices

B2B prices are often shown without tax. When a B2B buyer's prices exclude tax, the product page price and the cart show `Tax excluded.`, so the number is not mistaken for a final total. Retail shoppers see the store's usual tax note, if any.

## Tips

- **Test as a real buyer.** Create a test company with two locations, sign in as its contact and walk through a product page, the cart and a location switch. The theme editor preview shows the retail storefront, not a buyer's.
- **Keep the quick order template for products with many variants.** On a product with two or three variants, the regular product page is quicker.
- **Name locations the way buyers know them.** The location name is what the buyer reads in the header, and a name like "Warehouse 2" means little to a store manager.

## Troubleshooting

- **The company name doesn't show in the header.** The buyer must be signed in as a contact of a company. Guests and retail customers never see it.
- **The quick order list doesn't show.** Check the product uses the `quick-order` template, or that you added the **Quick order list** section to the template it does use.
- **No volume pricing appears.** Price breaks come from the catalog assigned to the buyer's current location. Check that catalog in `Products > Catalogs`.

## Related

- [Quick order list](../../sections/quick-order-list/)
- [Alternate product templates](../../templates/product-templates/)
- [Customer accounts](../customer-accounts/)
- [Shopify Help: B2B](https://help.shopify.com/manual/b2b)

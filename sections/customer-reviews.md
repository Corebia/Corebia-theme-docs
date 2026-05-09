---
title: Customer reviews
layout: default
parent: Sections
nav_order: 11
permalink: /sections/customer-reviews/
---

# Customer reviews

The **Customer reviews** section provides a placeholder area where you can add review-app blocks. The Pave theme itself does not collect or store reviews — it is a host for the blocks exposed by review apps.

## Settings

- **Show heading** — Toggle the section heading.
- **Heading** — The section heading. Default: `Customer reviews`.
- **Subheading** — Optional supporting text.
- **Heading alignment** — Options: **Left**, **Center**, **Right**.

The section also exposes spacing settings.

## How to populate the section with reviews

1. Install a Shopify reviews app from the Shopify App Store. Compatible apps include the official **Shopify Product Reviews** (free), as well as Loox, Judge.me, Yotpo, and others.
2. After installation, the app exposes one or more **app blocks** that you can add to any section that supports app blocks (see [Custom code](../../customization/custom-code/) for the technical context).
3. In the theme editor, open the **Customer reviews** section, click **Add block**, and pick the app block exposed by your reviews app.
4. Configure the block per the app's documentation.

If you don't install a reviews app, the section renders the heading and subheading but no review content. Reviewers' UI styling is the responsibility of the app, not the theme.

## Tips

- **Pick one reviews app and stay with it.** Migrating reviews between apps usually requires manual export and re-import.
- **Star ratings on product cards** — These come from the `reviews.rating` metafield, not from this section. Most reviews apps populate that metafield automatically; see [Product page > Product rating block](../../templates/product-page/) for how Pave displays star ratings on individual products.
- **Hide the section if no app is installed.** A heading "Customer reviews" with no content below it confuses customers.

## Related

- [Product rating on the product page](../../templates/product-page/) — How star ratings render on individual product pages.

---
title: Alternate product templates
layout: default
parent: Templates
nav_order: 3
permalink: /templates/product-templates/
---

# Alternate product templates

Besides the default [Product page](../product-page/), Pave ships three product templates for products that need a different page: **editorial**, **gift-card** and **quick-order**. Each one uses the same **Main product** section and blocks, so everything on the product page reference applies. What changes is how they are set up and which sections follow.

## Assigning a template

1. In Shopify admin, open **Products** and choose the product.
2. Under **Theme template**, choose **editorial**, **gift-card** or **quick-order**, and save.
3. To edit the template, open the theme editor and pick it from the template menu at the top, under **Products**. Changes apply to every product assigned to that template.

A product left on **Default product** keeps the standard page.

## Editorial

`product.editorial.json` is for hero products that deserve a story: a flagship piece, a new material, a collaboration. The buy box stays the same, and the page below it tells the product's story in images and copy.

**Main product** is set to a **Large** desktop media width with the **Thumbnails** gallery, one large image at a time, where the default template shows **2 columns**. The buy box holds the same blocks as the default template, except that the description sits in a **Description** collapsible tab rather than in the open.

Below it:

1. [Rich text with image](../../sections/rich-text-image/), with a **Wide (16:9)** image, the heading `The material` and a line of copy to replace.
2. [Brand image](../../sections/brand-image/), in the **Cinematic (panoramic)** proportion, for a campaign photograph.
3. [Brand message](../../sections/brand-message/), set to **Image first**, with the subheading `Style notes`, the heading `How to wear it`, a paragraph to replace and a `Shop all` button.
4. [Product recommendations](../../sections/product-recommendations/) in **Related products** mode, showing 4 products.

The text in these sections is placeholder copy written for one product. Rewrite it, or connect it to product metafields so each product assigned to the template tells its own story.

## Gift card

`product.gift-card.json` is for your gift card product. It keeps the buy box short: no details, care or shipping tabs, since none of them apply to a gift card. **Buy buttons** has **Show recipient information form for gift card products** on, so the shopper can send the card straight to someone else with a message.

Below it, an [FAQ](../../sections/faq/) section with the heading `Gift card questions` answers three questions every gift card buyer asks: how it is delivered, whether it can be used more than once, and whether it expires. Check the answers against how your gift cards actually work before publishing.

Gift card products are created in Shopify admin under **Products > Gift cards**. See [Gift cards](../../features/gift-cards/) for the setup and for the page the recipient sees.

## Quick order

`product.quick-order.json` is for products bought in quantity across many variants, typically by wholesale or B2B buyers: a shirt in eight sizes and five colors, ordered by the box.

The main section is set up like the default template, with the description in a **Description** collapsible tab. Below it sits a [Quick order list](../../sections/quick-order-list/): a table of every variant with its price and a quantity field, so a buyer can set quantities for twenty variants without picking each one in the variant picker. Each quantity goes straight into the cart as it is changed, so there is no separate add button. It ships with 50 variants per page and with variant images and SKUs showing.

## Tips

- **Preview before you assign.** Open the template in the theme editor with one of your own products selected in the preview, and check it reads right before you switch products over.
- **Don't leave the editorial copy generic.** The placeholder text on the editorial template is written for a single product. On a product that doesn't match it, it reads as filler.
- **Keep the quick order template for the products that need it.** A variant table on a product with three sizes is more work for the shopper than the picker.

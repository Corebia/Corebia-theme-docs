---
title: FAQ
layout: default
parent: Support
nav_order: 3
permalink: /support/faq/
---

# Frequently asked questions

## Setup and customization

### How do I change the logo?

Open the theme editor (**Online Store > Themes > Customize** on Pave), click **Theme settings**, then open the **Logo** category. Upload your logo image and adjust the width. The logo appears in sections that have shop branding enabled. See [Logo](../../theme-settings/logo/).

### How do I change colors and fonts?

In **Theme settings**, the **Colors** category controls every color via reusable color schemes; the **Typography** category controls heading and body fonts and their scaling. See [Colors](../../theme-settings/colors/) and [Typography](../../theme-settings/typography/).

### How do I add products to the menu?

In your Shopify admin, go to **Online Store > Navigation**. Edit the **Main menu** (or any menu), and add menu items linking to your products, collections, or pages. The header and footer in Pave automatically render the menus you configure here. See [Navigation](../../features/navigation/).

### How do I add a new section to a page?

In the theme editor, click **Add section** at the position you want. Pick from the available sections. See [Sections](../../sections/) for what each one does.

### How do I create an alternate template for a specific product or page?

In the theme editor, click the page selector dropdown at the top, then **Create template**. Name the template (for example, `landing-page`) and customize the sections. Then in the Shopify admin, assign the template to the product, page, or article that should use it. See [Shopify Help: Alternate templates](https://help.shopify.com/en/manual/online-store/themes/templates).

## Features

### Why don't I see Shop Pay Installments?

Shop Pay Installments requires Shopify Payments, Shop Pay enabled, a supported country, and a product price within the eligible range. If any of these aren't met, the banner is hidden automatically. See [Shop Pay Installments](../../features/shop-pay-installments/).

### How do I configure multi-currency or multi-language?

Both are configured in your Shopify admin under `Settings > Markets` and `Settings > Languages`. Once you have at least two markets or two languages, the country and language selectors appear automatically in Pave's footer. See [Multi-currency and language](../../features/multi-currency-language/).

### Does the theme support a wishlist app, reviews app, or any other Shopify app?

Pave supports **Shopify app blocks** in many sections, which lets compatible apps drop their UI directly into the theme without code edits. The full list of compatible apps depends on the app developer and which Shopify APIs they target. For reviews, we recommend installing a Shopify reviews app and using the **Customer reviews** section. See [Customer reviews](../../sections/customer-reviews/).

### Does Pave support subscriptions?

Yes — Pave displays selling plans on the product page, cart, and order detail. You'll need a separate subscription app (like the free **Shopify Subscriptions** app) to create the plans. See [Selling plans](../../features/selling-plans/).

### How do I set up complementary products?

Install the Shopify **Search & Discovery** app (free), then under `Recommendations`, pick the complementary products for each source product. In the theme, add the **Product recommendations** section to the product template and set its **Recommendation type** to **Complementary products**. A product with no pairings shows nothing at all, so the section is safe to add before you have finished pairing your catalog. See [Complementary products](../../sections/complementary-products/).

## Updates and customizations

### How do I update Pave when a new version is released?

From `Shopify admin > Online Store > Themes`, click **Update** on Pave (the option appears when a new version is available). The new version is added to your library as a fresh copy. Test it, port any customizations, then publish when ready. See [Duplicate your theme](../../customization/duplicating-your-theme/).

### Do I lose my customizations when I update?

If you've only changed theme settings (colors, fonts, section settings), Shopify's update flow can carry these over to the new version. If you've edited theme code, those edits do not carry over and you'll need to re-apply them manually. See [Custom code](../../customization/custom-code/).

### Can I transfer the theme to another store?

A theme installed via the Shopify Theme Store is licensed to a single store. To use it on another store, purchase a separate license for that store. Shopify handles the licensing — see the [Shopify Help Center: Themes](https://help.shopify.com/manual/online-store/themes).

### How do I customize the theme beyond what the editor allows?

Hire a Shopify Partner. The [Shopify Partner Directory](https://www.shopify.com/partners/directory) lists verified developers who can extend Pave to your specific needs. See [Custom code](../../customization/custom-code/).

## Support

### How long does support take to respond?

Within 2 business days. Most tickets are answered the next business day. Critical bugs (issues affecting checkout or storefront availability) are addressed immediately. See [Support policy](../support-policy/).

### How do I report a bug?

Open the [contact form](../contact/) and include your store URL, theme version, browser and device, a description of the bug, steps to reproduce, and screenshots. The more detail, the faster we can fix it.

### How do I request a refund?

Themes purchased from the Shopify Theme Store are final sale. Refund requests are handled by Shopify Support, not by Corebia. Contact [Shopify Support](https://help.shopify.com/support) directly for refund inquiries.

### Is the theme compatible with [Shopify feature X]?

Pave supports every standard feature of Shopify Online Store 2.0, including section groups, app blocks, dynamic checkout, accelerated payment buttons, multi-currency, multi-language, gift cards, selling plans, pickup availability, and more. For a specific feature, search this documentation or reach out via the [contact form](../contact/).

### How do customer accounts work in Pave?

The account entry point sits in the header's navigation panel on every page. It is Shopify's own component, so it shows a signed-out or signed-in state by itself and needs no setup beyond enabling accounts in `Shopify admin > Settings > Customer accounts`.

The account pages themselves are rendered by Shopify, not by the theme. The one thing you control from the theme is which menu appears inside the account panel, through the header's **Customer account menu** setting. See [Customer accounts](../../features/customer-accounts/).

### What plan do I need?

Pave works on every Shopify plan. Some features (Shop Pay Installments, multi-currency via Shopify Payments, etc.) require Shopify Payments, which is available on every plan in supported countries.

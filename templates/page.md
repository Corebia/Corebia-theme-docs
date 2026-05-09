---
title: Page
layout: default
parent: Templates
nav_order: 10
permalink: /templates/page/
---

# Page

The **Page** template renders a Shopify page (created in `Shopify admin > Online Store > Pages`). It uses the `page.json` template. Use it for content like About, FAQ, Sustainability, or any other static page.

## URL

`https://yourstore.com/pages/<page-handle>`

## Sections included by default

1. **Main page** — The page body, rendering the title and rich text content from the Shopify admin.
2. **Newsletter** — Email signup form below the content.

## Main page section

- **Show back link and breadcrumb** — Toggle.
- **Color scheme** — Default: scheme-1.

The page title and body content come from `Shopify admin > Online Store > Pages > [page] > Title` and **Content**.

## Sections that can be added

In addition to **Main page**, you can add any of these sections:

- [Newsletter](../../sections/newsletter/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [FAQ](../../sections/faq/)
- [Featured product](../../sections/featured-product/)
- [Customer reviews](../../sections/customer-reviews/)
- [Collection list](../../sections/collection-list/)
- [Custom Liquid](../../sections/custom-liquid/)

## Special use: contact page

A separate template, `page.contact.json`, is used for the contact page. See [Contact page](../contact-page/).

## Alternate templates

If you want a specific page to use a different layout (for example, a long-form sustainability page with a hero banner), you can create an alternate template:

1. In the theme editor, click the page selector dropdown at the top.
2. Choose **Pages > Create template**.
3. Name your template (for example, `sustainability`).
4. Customize the sections.
5. In `Shopify admin > Online Store > Pages > [page] > Theme template`, pick your custom template.

See [Shopify Help: Alternate templates](https://help.shopify.com/en/manual/online-store/themes/templates).

## Tips

- **Replace the default newsletter** with a more contextual section if the page is about a specific topic (for example, an FAQ section on a help page).
- **Use rich text formatting** in the Shopify admin to structure your page content. Pave styles headings, lists, and quotes for editorial readability.
- **Don't put long-form copy in a Hero banner.** That's not what hero is designed for. Use the Page content area for body text.

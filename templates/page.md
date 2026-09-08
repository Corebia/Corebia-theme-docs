---
title: Page
layout: default
parent: Templates
nav_order: 10
permalink: /templates/page/
---

# Page

The default template for any page you create in `Shopify admin > Content > Pages`: About, Stockists, Size guide, Shipping information. It uses the **Main page** section, which renders the page's title and body.

## Section settings

- **Show back link and breadcrumb.** Default: on.
- **Color scheme.** Default: scheme-1.

## Blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/custom-liquid/).

## Building richer pages

The page body is a rich text field, which is enough for text and images but not for layout. For a landing page, such as an About page with a full-bleed image, a lookbook or a campaign page, add sections above and below the Main page section in the theme editor:

- [Hero banner](../../sections/hero/) for an opening image
- [Brand message](../../sections/brand-message/) and [Rich text with image](../../sections/rich-text-image/) for image-and-copy blocks
- [Brand image](../../sections/brand-image/) for a full-width photograph or video
- [Featured product](../../sections/featured-product/) to make one product buyable in place
- [FAQ](../../sections/faq/) for questions

Sections you add this way apply to **every** page using this template. To give one page its own arrangement, create an alternate template.

## Alternate templates

In the theme editor's template picker, choose **Create template** and base it on `page`. Then set that template on the page under its **Theme template** setting in the admin.

Pave ships one alternate page template already: [Contact page](../contact-page/).

## Tips

- **Use the page body for words and sections for layout.** Trying to lay out a page inside the rich text editor is where most of the frustration with Shopify pages comes from.
- **Turn the back link off on landing pages.** A breadcrumb above a full-bleed hero undercuts it.
- **Name templates for their shape, not their content.** `page.wide`, `page.lookbook`, so the next page of that shape can reuse them.

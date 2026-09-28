---
title: Page
layout: default
parent: Templates
nav_order: 12
permalink: /templates/page/
---

# Page

The default template for any page you create in `Shopify admin > Content > Pages`: Stockists, Shipping information, Terms of trade. It uses the **Main page** section, which renders the page's title and body.

## Section settings

- **Show back link and breadcrumb.** A back link and a `Home / <page title>` breadcrumb above the title. Default: on. The back link returns the shopper to the collection, search results or page they came from, and to the home page otherwise.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 110 px each. This is the padding on screens 1920 px and wider; it scales down on smaller screens.

## Blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/theme-blocks/#custom-liquid).

## Building richer pages

The page body is a rich text field, which is enough for text and images but not for layout. For a landing page, such as a campaign or a brand story, add sections below the Main page section in the theme editor:

- [Section](../../sections/section/), a free-form container for headings, text, images and buttons
- [Media with content](../../sections/media-with-content/) and [Rich text with image](../../sections/rich-text-image/) for image-and-copy blocks
- [Brand image](../../sections/brand-image/) for a full-width photograph or video
- [Featured product](../../sections/featured-product/) to make one product buyable in place
- [FAQ](../../sections/faq/) for questions, and [Contact form](../../sections/contact-form/) for a way to ask more

Sections you add this way apply to **every** page using this template. To give one page its own arrangement, use an alternate template.

## Alternate templates

Pave ships nine alternate page templates, each a ready-made arrangement of sections for a common kind of page:

- [Contact page](../contact-page/) (`contact`), a contact form beside your contact details.
- [About, Accessibility, Contact and stores, Drop, Editorial, FAQ, Lookbook and Size guide](../page-templates/).

To use one, open the page in `Shopify admin > Content > Pages` and pick it under **Theme template**. To make your own, open the theme editor's template picker, choose **Create template** and base it on an existing page template.

## Tips

- **Use the page body for words and sections for layout.** Trying to lay out a page inside the rich text editor is where most of the frustration with Shopify pages comes from.
- **Turn the back link off on landing pages.** A breadcrumb above a full-bleed opening image undercuts it.
- **Name templates for their shape, not their content.** `page.wide` or `page.campaign`, so the next page of that shape can reuse them.

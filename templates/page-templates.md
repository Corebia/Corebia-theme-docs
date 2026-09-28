---
title: Alternate page templates
layout: default
parent: Templates
nav_order: 14
permalink: /templates/page-templates/
---

# Alternate page templates

Besides the default [Page](../page/) template and the [Contact page](../contact-page/), Pave ships eight page templates, each a ready-made arrangement of sections for a kind of page most stores need. They save you building the layout from scratch; the words and images are yours to write. The sample text in each one describes what belongs there, such as the year you started or how your products are made, rather than telling another brand's story, and image slots start empty.

Every one of them starts with the **Main page** section, so the page's own title, and its body if it has one, come first. The sections below it are ordinary sections: select them in the theme editor to change them, reorder them, remove them or add others. The ones that carry running text, such as the accessibility statement, the size guide's measuring instructions, the lookbook's introduction and the store list, use the **Reading column** content width, so they continue the column of the page title above them.

## Using a template

1. Create the page in `Shopify admin > Content > Pages`, or open an existing one.
2. Under **Theme template**, pick the template by its name: `about`, `accessibility`, `contact-stores`, `drop`, `editorial`, `faq`, `lookbook` or `size-guide`.
3. Save, then open the page in the theme editor to replace the sample content.

Changes you make to a template's sections apply to every page using that template. A page's title and body stay per page.

## About

Template `about`. A brand story told in sections.

1. **Main page**, for the title and any opening words.
2. [Media with content](../../sections/media-with-content/), image on the left: a heading, a paragraph and a button, starting as `Tell your story`.
3. [Section](../../sections/section/) with a row of three figures, each a heading and a line of text, such as a founding year, a material and a place. They are [Group](../../sections/theme-blocks/#group) blocks holding [Heading](../../sections/theme-blocks/#heading) and [Text](../../sections/theme-blocks/#text) blocks.
4. [Media with content](../../sections/media-with-content/), image on the right, about how the products are made.
5. [Brand message](../../sections/brand-message/), closing with a promise and a link to the journal.

**When to use it:** the page your header or footer calls About, Our story or Who we are.

## Accessibility

Template `accessibility`. An accessibility statement.

1. **Main page**.
2. [Section](../../sections/section/) in the **Reading column** content width, with alternating [Heading](../../sections/theme-blocks/#heading) and [Text](../../sections/theme-blocks/#text) blocks: an opening paragraph, then **What we have done**, **Known limits** and **Report a barrier**.

The sample text states an aim of WCAG 2.2 level AA and points to your contact page for reporting problems.

**When to use it:** for a published accessibility statement, which some markets expect and many shoppers look for.

**Before publishing:** read every line and keep only what is true of your store. A statement describes your own store, including any apps you have added, so it has to be checked by you rather than inherited from the theme. The **Report a barrier** text links to `/pages/contact`; change the link if your contact page has a different address.

## Contact and stores

Template `contact-stores`. For stores with physical locations.

1. **Main page**.
2. [Store locations](../../sections/store-locations/) in the **Reading column** content width, with no heading of its own, so the page title heads it, and a line of introduction. It holds two example stores, each with a name, address and opening hours.
3. [Contact form](../../sections/contact-form/), headed `Get in touch`, with the phone field on.

**When to use it:** when shoppers can visit you. With no shops, the [Contact page](../contact-page/) template, with its details panel, is the better fit.

**Before publishing:** replace both example stores. Their names and addresses are placeholders and would otherwise go live.

## Drop

Template `drop`. A product or collection launch at a set date and time.

1. **Main page**.
2. [Drop](../../sections/drop/): before the launch, a heading, text, a countdown and a waitlist signup; from the launch moment, the live heading and text with links to the product and collection you chose.

**When to use it:** for a limited release you are building anticipation for. Set the date, time and timezone on the Drop section, and it switches from the countdown to the live content on its own, without anyone reloading the page.

## Editorial

Template `editorial`. A shoppable campaign page.

1. **Main page**.
2. [Shoppable videos](../../sections/shoppable-videos/), headed `Shop the video`, with three video blocks and autoplay off.
3. [Complete the look](../../sections/complete-the-look/): one look image and the products that make it up.
4. [Scrollytelling](../../sections/scrollytelling/): three chapters, each with text and product hotspots, that change as the shopper scrolls.

**When to use it:** for a season's campaign, a collaboration or a story you want shoppers to buy from as they read.

**Before publishing:** choose a video and a product for each video block, the image and products for Complete the look, and an image and the hotspot products for each chapter. The template ships without them, and those parts stay empty until you do.

## FAQ

Template `faq`. A full-page set of questions and answers.

1. **Main page**.
2. [FAQ](../../sections/faq/), with its **Show heading** off so it doesn't repeat the page title, and seven questions on shipping, returns, sizing, care, payment, gift cards and changing an order.
3. [Contact form](../../sections/contact-form/), headed `Still have a question?`.

**When to use it:** as the one page your footer's Help or FAQ link points to.

**Before publishing:** rewrite each answer for your store. The sample answers are generic, and one links to your refund policy, which only works once that policy is written in `Shopify admin > Settings > Policies`.

## Lookbook

Template `lookbook`. A visual page for a collection or a season.

1. **Main page**.
2. [Section](../../sections/section/) in the **Reading column** content width, with a heading and an introduction.
3. [Shoppable image](../../sections/shoppable-image/): a campaign photograph with three product hotspots.
4. [Collage](../../sections/collage/), headed `The edit`, with five image tiles, each linked to a collection.
5. [Media with content](../../sections/media-with-content/), image on the right, with a button to the collection.

**When to use it:** to show products worn and styled rather than in a grid. For a lookbook-style collection page with filters, see [Lookbook collection page](../lookbook-collection/).

## Size guide

Template `size-guide`. A standalone size guide page.

1. **Main page**, whose body carries your size chart.
2. [Section](../../sections/section/) in the **Reading column** content width, headed `How to measure`, with measuring instructions for chest, waist, hips and inside leg.

**When to use it:** together with the product page's size guide link. On the [Product page](../product-page/), the **Variant picker** block's **Size guide page** setting puts a size guide link next to the size option, and it opens the chosen page in a popup. A product can point to a different page through the `custom.size_guide` metafield.

**How the two fit together:** the popup shows only the page's **body**, not the sections of this template. So put the size chart itself in the page body, where both the popup and the standalone page show it, and keep the longer measuring advice in the How to measure section, which shoppers see when they open the page itself.

## Tips

- **Replace every sample before publishing.** Headings like `Tell your story` and the example store names read as placeholders to a shopper.
- **Settings belong to the template, not the page.** Two pages on the `drop` template share one Drop section, so they would count down to the same moment. For two launches running at once, create a second template from the first in the theme editor.
- **Duplicate before you change a template for one page.** Editing a template's sections changes every page using it. To give one page its own arrangement, create a new template from the theme editor's template picker, based on the one you want.

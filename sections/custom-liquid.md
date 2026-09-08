---
title: Custom Liquid
layout: default
parent: Sections
nav_order: 20
permalink: /sections/custom-liquid/
---

# Custom Liquid

**Custom Liquid** is an empty section that renders whatever Liquid, HTML, CSS or JavaScript you put in it. It is the escape hatch: the place for an app snippet, or for something the theme's own sections don't cover.

It can be added to any template that takes sections.

## Settings

- **Liquid code** — Add app snippets or custom code. Use with care: invalid Liquid can break the page.

## The block, as well as the section

Several sections also offer a **Custom Liquid block**, which does the same thing inside an existing layout rather than as a section of its own. The block is available on the product page, the collection and catalog pages, the cart, articles, blog, pages, policies, customer reviews and featured product.

Use the **block** when the code belongs inside a section that is already there — a badge under the buy buttons, say. Use the **section** when it needs its own slot in the page.

## What to put in it

Good candidates:

- A snippet an app gave you to paste.
- A one-off announcement or seasonal note that doesn't warrant a section.
- A small piece of markup you want on one page only.

Poor candidates:

- **Anything you'll want on many pages.** Repeating the same snippet in ten places means changing it in ten places.
- **Large blocks of code.** They are hard to edit inside a settings field and are invisible to anyone reading the theme's files. Put those in the theme code — see [Custom code](../../customization/custom-code/).

## Tips

- **Test on a duplicate theme.** Invalid Liquid can break the page it sits on, and the theme editor will not always stop you saving it. Duplicating first costs a minute — see [Duplicate your theme](../../customization/duplicating-your-theme/).
- **Quote your attributes.** Unquoted HTML attributes that contain Liquid output are the most common way this section breaks a layout.
- **Liquid objects are available.** `product`, `collection`, `cart` and the rest resolve according to the page the section is on, so the same snippet can behave differently on different templates.
- **Custom Liquid is not covered by theme support.** Code you add here is yours. See the [Support policy](../../support/support-policy/).

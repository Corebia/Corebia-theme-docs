---
title: Custom Liquid
layout: default
parent: Sections
nav_order: 17
permalink: /sections/custom-liquid/
---

# Custom Liquid

The **Custom Liquid** section provides a free-form area where you can add Shopify Liquid code, app snippets, or HTML directly into a page through the theme editor.

{: .warning }
> Custom Liquid is an advanced feature. Invalid Liquid can break the page that contains it. Custom code added here is not covered by support — see [Custom code](../../customization/custom-code/).

## Settings

- **Liquid code** — The code to render. Add app snippets or custom code. Use with care: invalid Liquid can break the page.

## When to use

- **App snippets** — Some Shopify apps provide a Liquid snippet you can paste into your theme. The Custom Liquid section is the place to drop it without editing theme files.
- **One-off announcements** — A bespoke holiday banner, a campaign-specific HTML widget, an embed from a third-party tool.
- **Quick experiments** — Test a markup change on a single page without editing the section files.

## When not to use

- **Recurring patterns** — If you find yourself pasting the same code into multiple Custom Liquid sections, consider asking a Shopify Partner to build a proper section instead. See [Custom code](../../customization/custom-code/).
- **Large blocks of code** — The setting accepts up to ~50 KB of code, but anything over a few dozen lines is hard to maintain through the theme editor.
- **Dynamic state** — JavaScript that reads or writes Shopify cart state should be added carefully. Use a Shopify Partner.

## Tips

- **Test in a duplicate theme.** Bad Liquid raises a parse error and prevents the page from rendering. Always test changes in a duplicate before publishing.
- **Quote everything.** Pasting code from a chat tool or document can introduce smart quotes that break Liquid syntax. Type code directly into the editor or use a plain-text source.
- **Reference Shopify objects.** Custom Liquid in this section runs in the storefront context, so you have access to `product`, `collection`, `cart`, `shop`, etc. depending on the page.

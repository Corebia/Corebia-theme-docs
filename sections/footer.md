---
title: Footer
layout: default
parent: Sections
nav_order: 2
permalink: /sections/footer/
---

# Footer

The **Footer** section appears at the bottom of every page. It is composed of three areas: a giant brand name, navigation columns made up of blocks, and a bottom bar with social icons, payment icons, language and country selectors, and the Follow on Shop button.

## Settings

- **Brand text** — The large editorial brand text shown at the top of the footer. Default: `ATELIER`.
- **Show social media icons** — Toggle the row of social icons in the bottom bar. Reads URLs from **Theme settings > Social media**. Default: on.
- **Show payment icons** — Toggle the row of payment provider icons. Reads enabled providers from `Shopify admin > Settings > Payments`. Default: on.
- **Show Follow on Shop** — Toggle the Follow on Shop button. Lets customers follow your store from the Shop app. Default: on.
- **Color scheme** — The color scheme applied to the footer. Default: scheme-1.

## Blocks

The footer accepts two block types. Add blocks via **Add menu** or **Add text**. Each block becomes a column.

### Menu

Renders a Shopify navigation as a column of links.

- **Heading** — Column heading. Default: `Quick links`.
- **Menu** — The Shopify navigation to render.

### Text

Renders a column of free-form rich text.

- **Heading** — Column heading. Default: `About us`.
- **Text** — Rich text body. Default: `Share store details, promotions, or brand content with your customers.`

## Fixed elements (bottom bar)

The bottom bar always contains:

- **Country selector** — Shown when more than one country is configured in `Shopify admin > Settings > Markets`. See [Multi-currency and language](../../features/multi-currency-language/).
- **Language selector** — Shown when more than one language is published. See [Multi-currency and language](../../features/multi-currency-language/).

These are rendered automatically; there are no settings to control them in the footer section.

## Tips

- **Three to four blocks** is the sweet spot for a balanced footer. With one or two columns the footer feels sparse; with six or more it crowds.
- The **Brand text** is intentionally oversized — it acts as a closing brand statement, not a logo replacement. Use your brand name or a short tagline.
- For a smaller footprint, disable the social and Follow on Shop rows and reduce blocks to two columns.

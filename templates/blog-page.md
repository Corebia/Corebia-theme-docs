---
title: Blog page
layout: default
parent: Templates
nav_order: 8
permalink: /templates/blog-page/
---

# Blog page

The list of articles in a blog, using the **Main blog** section. Every element on the card is a switch, and every string is editable: image, date, author and excerpt.

## Section settings

- **Color scheme.** Default: scheme-1.

### Layout

- **Heading.** Leave blank to use the blog's own title.
- **Number of columns.** Range: 2 to 4. Default: 3.
- **Articles per page.** Range: 3 to 24 in steps of 3. Default: 9.
- **Image ratio.** **Portrait (3:4)** (default), **Landscape (4:3)** or **Square (1:1)**.

### Card elements

- **Show featured image.** Default: on.
- **Show heading.** Default: on.
- **Show date.** Default: on.
- **Show author.** Default: off.
- **Show excerpt.** Default: on.
- **Excerpt word count.** Range: 10 to 50 in steps of 5. Default: 20.
- **Date format.** `January 01, 2026` (default), `01 January 2026`, `01/01/2026 (day/month/year)`, `01/01/2026 (month/day/year)` or `2026-01-01`.

### Text content

Every visible string, so the blog can be reworded without translations.

- **Article count label.** Leave blank to show a correctly pluralized count (1 article / 2 articles).
- **Read more button text.** Default: `Read more`.
- **Empty state message.** Default: `No articles yet`.
- **Previous page text.** Default: `Previous`.
- **Next page text.** Default: `Next`.
- **Pagination label.** Default: `Page`.

## Blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/custom-liquid/).

## Excerpts

The excerpt comes from the article's own **Excerpt** field in `Shopify admin > Content > Blog posts`. When that is empty, the theme takes the opening of the article body and trims it to the word count set above.

Writing a real excerpt is worth the minute: the automatic version starts wherever the article starts, which is often mid-thought.

## Tips

- **Pick a date format and use it everywhere.** The article page has its own date format setting; two different formats across two pages of the same blog looks like an error.
- **Author is off by default** because most store blogs are written by the store. Turn it on if you publish guest pieces or if the writer is part of the appeal.
- **Match the image ratio to the blog's photography.** Portrait suits editorial and fashion; landscape suits how-to and product photography.
- **Nine per page and three columns** fill three even rows. Choosing counts that divide by your column count avoids a ragged last row.

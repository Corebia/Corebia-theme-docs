---
title: Blog page
layout: default
parent: Templates
nav_order: 10
permalink: /templates/blog-page/
---

# Blog page

The list of articles in a blog, using the **Main blog** section. It lays the articles out as a grid, a list or a grid led by one large article, can filter by tag, and lets you switch every element of the article card on or off.

## Section settings

- **Color scheme.** Default: scheme-1.
- **Show back link and breadcrumb.** A back link and a `Home / <blog title>` breadcrumb above the heading. The back link returns to the previous page in your store, and the breadcrumb traces the path from the home page. Default: on.

### Layout

- **Heading.** Leave blank to use the blog's own title.
- **Listing layout.** **Grid** (default), **List** (one article per row, image beside the text) or **Featured first** (the newest article spans the whole row, image beside the text, above the grid; first page only).
- **Number of columns.** Range: 2 to 4. Default: 3. Not shown with the List layout.
- **Show tag filter.** A row of links, one per tag used in the blog, plus **All**. Default: on. It only appears once the blog has tagged articles.
- **Articles per page.** Range: 3 to 24 in steps of 3. Default: 9.
- **Image ratio.** **Portrait (3:4)** (default), **Landscape (4:3)** or **Square (1:1)**. Shown when **Show featured image** is on.

### Card elements

- **Show featured image.** Default: on.
- **Show heading.** Default: on.
- **Show date.** Default: on.
- **Show author.** Default: off.
- **Show reading time.** An estimate such as `4 min read`, worked out from the length of the article. Default: off.
- **Show excerpt.** Default: on.
- **Excerpt word count.** Range: 10 to 50 in steps of 5. Default: 20. Shown when **Show excerpt** is on.
- **Date format.** Shown when **Show date** is on.
  - **January 1, 2026, in the shopper's language** (default)
  - **Jan 1, 2026, in the shopper's language**
  - **01/01/2026 (day/month/year)**
  - **01/01/2026 (month/day/year)**
  - **2026-01-01**

  The first two write the month name in the language the shopper is browsing in.

### Text content

Visible strings you can reword here.

- **Article count label.** Leave blank to show a correctly pluralized count (1 article / 2 articles). Text typed here replaces the count's wording and can't pluralize, so blank is usually right.
- **Read more button text.** Default: `Read more`.
- **Empty state message.** Default: `No articles yet`.
- **Previous page text.** Default: `Previous`.
- **Next page text.** Default: `Next`.
- **Pagination label.** Default: `Page`.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 110 px each. This is the padding on screens 1920 px and wider; it scales down on smaller screens.

## Blocks

- **App block.** Any block offered by an installed app.
- **Custom Liquid.** See [Custom Liquid](../../sections/theme-blocks/#custom-liquid).

## Excerpts

The excerpt comes from the article's own **Excerpt** field in `Shopify admin > Content > Blog posts`. When that is empty, the theme takes the opening of the article body and trims it to the word count set above.

Writing a real excerpt is worth the minute: the automatic version starts wherever the article starts, which is often mid-thought.

## Tips

- **Pick a date format and use it everywhere.** The article page's Date block has its own format setting; two different formats across two pages of the same blog look like an error.
- **Author is off by default** because most store blogs are written by the store. Turn it on if you publish guest pieces or if the writer is part of the appeal.
- **Tag with a small, fixed vocabulary.** The tag filter shows every tag you have used, so twenty one-off tags turn it into noise. Four to eight recurring themes make it a real way in.
- **Featured first rewards a strong lead image.** The newest article gets the most space, so it suits blogs where each post has a photograph worth leading with.
- **Match the image ratio to the blog's photography.** Portrait suits editorial and fashion; landscape suits how-to and product photography.
- **Nine per page and three columns** fill three even rows. Choosing counts that divide by your column count avoids a ragged last row.

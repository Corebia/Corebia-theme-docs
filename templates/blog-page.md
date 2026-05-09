---
title: Blog page
layout: default
parent: Templates
nav_order: 8
permalink: /templates/blog-page/
---

# Blog page

The **Blog page** lists all articles in a blog. It uses the `blog.json` template.

## URL

`https://yourstore.com/blogs/<blog-handle>`

## Sections included by default

1. **Main blog** — The grid of article cards with pagination.

## Main blog section

### Layout

- **Heading** — The blog heading.
- **Number of columns** — Range slider.
- **Articles per page** — Number of articles to load per page. Pagination loads more.
- **Image ratio** — Options: **Portrait (3:4)**, **Landscape (16:9)**, **Square (1:1)**.

### Card elements

Toggle which fields are shown on each article card.

- **Show featured image** — Toggle.
- **Show title** — Toggle.
- **Show date** — Toggle.
- **Show author** — Toggle.
- **Show excerpt** — Toggle.
- **Excerpt word count** — Cap on excerpt length.
- **Date format** — Options: **January 01, 2026**, **01 January 2026**, **01/01/2026** (DMY), **01/01/2026** (MDY), **2026-01-01**.

### Text content

- **Article count label** — Word used after the article count. Default: `articles`.
- **Read more button text** — Default: `Read more`.
- **Empty state message** — Shown when the blog has no articles. Default: `No articles yet`.
- **Previous page text** — Default: `Previous`.
- **Next page text** — Default: `Next`.
- **Pagination label** — Default: `Page`.

### Other

- **Color scheme** — Default: scheme-1.

## Sections that can be added

In addition to **Main blog**, you can add any of these sections:

- [Newsletter](../../sections/newsletter/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [FAQ](../../sections/faq/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Show the excerpt** to give customers a reason to click into a specific article. Without the excerpt, only the title and image carry information.
- **Image ratio** — Pick **Landscape (16:9)** for editorial content where the image carries the article. **Portrait (3:4)** works for fashion editorials.
- **Date format** — Match the format to your locale. The MDY and DMY formats both render as `01/01/2026` but differ in interpretation; pick the one matching customer expectation.

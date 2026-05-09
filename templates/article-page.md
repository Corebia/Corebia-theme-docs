---
title: Article page
layout: default
parent: Templates
nav_order: 9
permalink: /templates/article-page/
---

# Article page

The **Article page** displays a single blog article. It uses the `article.json` template.

## URL

`https://yourstore.com/blogs/<blog-handle>/<article-handle>`

## Sections included by default

1. **Main article** — The article body with title, image, date, content, and tags.

## Main article section

The Main article section is built from blocks. The default layout includes:

1. Title
2. Published date
3. Author
4. Featured image
5. Content
6. Separator
7. Tags
8. Back button

You can add, remove, and reorder these blocks from the theme editor.

### Available blocks

- **Featured image** — The article hero image.
  - **Image width** — Options: **Constrained (800px)**, **Full width**.
  - **Image ratio** — Options: **Original**, **Landscape (16:9)**, **Portrait (3:4)**.
- **Title** — The article title.
- **Date** — The published date.
  - **Date format** — Options: **January 01, 2026**, **01 January 2026**, **01/01/2026** (DMY), **01/01/2026** (MDY), **2026-01-01**.
- **Author** — The article author.
  - **Author prefix text** — Default: `By`.
- **Content** — The article body HTML.
- **Tags** — The article's tags.
  - **Tags label text** — Default: `Tags`.
- **Separator** — A horizontal divider.
- **Back button** — A link back to the blog index.
  - **Back button text** — Default: `Go back`.
- **Quote** — A pull quote inside the body.
  - **Quote text** — The quote content.
  - **Source / author** — The quote attribution.
- **Comments** — The article's comments thread (when comments are enabled in `Shopify admin > Online Store > Blog posts > Comments`).

### Section settings

- **Color scheme** — Default: scheme-1.

## Special behaviors

- **Comments** — Whether the comments block renders depends on the blog's comment setting. With moderation, comments appear after approval.
- **Reading time** is not built in. If you need it, install a Shopify app or add a Custom Liquid block.
- **Article-specific Open Graph image** — The article's featured image is automatically used as the social share image when the article is shared.

## Sections that can be added

In addition to **Main article**, you can add any of these sections:

- [Newsletter](../../sections/newsletter/)
- [Recently viewed](../../sections/recently-viewed/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [FAQ](../../sections/faq/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Featured image width** — **Full width** works for editorial articles with hero photography. **Constrained** works for instructional or text-heavy articles.
- **Pull quotes (Quote block)** — Use sparingly. One pull quote in a long article gives the reader a breather; multiple feel busy.
- **Comments** — Disable on most stores. Comments require moderation and rarely add value compared to maintenance overhead.

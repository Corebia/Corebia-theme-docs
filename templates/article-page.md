---
title: Article page
layout: default
parent: Templates
nav_order: 11
permalink: /templates/article-page/
---

# Article page

A single blog post, using the **Main article** section. Like the product page, it is built from blocks you order yourself, so the byline can sit above or below the featured image, and a **Back button** block can go at the top or the end.

Below it, the template ships a [Related articles](../../sections/related-articles/) section.

## Blocks it ships with

A fresh install lays the article out in this order: **Heading**, **Date**, **Reading time**, **Author**, **Featured image**, **Content**, **Separator**, **Tags**, **Comments** and **Back button**. Drag them into any order, remove the ones you don't want, and add **Quote** blocks where the text needs a pause.

## Section settings

- **Show back link and breadcrumb.** A back link and a `Home / <blog title> / <article title>` breadcrumb above the article, as on the other templates. Default: on. The back link returns to the previous page in your store, or to the blog when there is none, and the blog's name in the breadcrumb links to the blog. It is separate from the **Back button** block, so with both you get a link at the top and a button wherever you placed the block.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 110 px each. This is the padding on screens 1920 px and wider; it scales down on smaller screens.

## Blocks

### Heading

The article title. No settings.

### Date

- **Date format.**
  - **January 1, 2026, in the shopper's language** (default)
  - **Jan 1, 2026, in the shopper's language**
  - **01/01/2026 (day/month/year)**
  - **01/01/2026 (month/day/year)**
  - **2026-01-01**

### Reading time

An estimate such as `4 min read`, worked out from the number of words in the article at 200 words a minute, rounded up. No settings.

### Author

- **Author prefix text.** Default: `By`.

### Featured image

- **Image width.** **Constrained (800px)** (default) or **Full width**.
- **Image ratio.** **Original** (default), **Landscape (16:9)** or **Portrait (3:4)**.

### Content

The article body, as written in Shopify. No settings.

### Tags

- **Tags label text.** Default: `Tags`.

### Quote

A pull quote. It shows nothing until it has text.

- **Quote text.**
- **Source / author.**

### Separator

A horizontal rule, for pacing a long article. No settings.

### Back button

A link back to the blog the article belongs to.

- **Back button text.** Default: `Go back`. Clear it to show the arrow on its own; screen readers still announce it as a back link.

### Comments

The comment list and form. No settings. See [Turning comments on](#turning-comments-on) below.

### Custom Liquid

See [Custom Liquid](../../sections/theme-blocks/#custom-liquid).

### App block

Any block offered by an installed app.

## Turning comments on

The Comments block renders only when comments are enabled for that blog, under `Shopify admin > Content > Blogs > Manage blog`. With them disabled, the block is skipped rather than showing a form whose messages would go nowhere, so it is safe to leave in the template while you decide.

Shopify offers three modes: disabled, enabled with moderation, and enabled without. Moderation is the sensible default for a store blog.

## Related articles

The [Related articles](../../sections/related-articles/) section under the article shows other articles from the same blog: first the ones that share a tag with this article, newest first, then the newest of the rest, up to the number you set. It can only be added to article templates, and it hides itself when the blog has no other articles.

## Wide tables in article content

Tables written in the article body scroll horizontally on narrow screens rather than being cut off. This is automatic and has no setting.

## Tips

- **Constrained image width reads better for text-led posts**; full width suits a photo essay.
- **Use Separator blocks to pace a long read.** They give the eye somewhere to rest, which excerpts and subheadings alone don't.
- **Put the Back button at the end.** A reader who has finished wants a way onward; one who has just arrived doesn't need an exit.
- **Match the date format to the blog page.** Both have their own setting, and they should agree.
- **Tag articles to get better related articles.** Without shared tags the section falls back to your newest posts, which is fine, but a shared tag is what makes the suggestion feel chosen.

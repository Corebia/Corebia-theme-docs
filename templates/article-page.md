---
title: Article page
layout: default
parent: Templates
nav_order: 9
permalink: /templates/article-page/
---

# Article page

A single blog post, using the **Main article** section. Like the product page, it is built from blocks you order yourself — so the byline can sit above or below the featured image, and the back link can be at the top or the end.

## Section settings

- **Color scheme** — Default: scheme-1.

## Blocks

### Featured image

- **Image width** — **Constrained (800px)** (default) or **Full width**.
- **Image ratio** — **Original** (default), **Landscape (16:9)** or **Portrait (3:4)**.

### Heading

Limit 1. The article title. No settings.

### Date

Limit 1.

- **Date format** — `January 01, 2026` (default), `01 January 2026`, `01/01/2026 (day/month/year)`, `01/01/2026 (month/day/year)` or `2026-01-01`.

### Author

Limit 1.

- **Author prefix text** — Default: `By`.

### Content

The article body, as written in Shopify. No settings.

### Tags

Limit 1.

- **Tags label text** — Default: `Tags`.

### Separator

A horizontal rule, for pacing a long article. No settings.

### Back button

Limit 1.

- **Back button text** — Default: `Go back`.

### Quote

A pull quote.

- **Quote text**
- **Source / author**

### Comments

Limit 1. The comment list and form. No settings.

### Custom Liquid

- **Liquid code** — See [Custom Liquid](../../sections/custom-liquid/).

### App block

Any block offered by an installed app.

## Comments

The Comments block renders only when comments are enabled for that blog, under `Shopify admin > Content > Blogs > Manage blog`. With them disabled, the block is silently skipped rather than showing an empty form — so it is safe to leave in the template while you decide.

Shopify offers three modes: disabled, enabled with moderation, and enabled without. Moderation is the sensible default for a store blog.

## Wide tables in article content

Tables written in the article body scroll horizontally on narrow screens rather than being cut off, and a table that scrolls is reachable with the keyboard. This is automatic and has no setting.

## Tips

- **Constrained image width reads better for text-led posts**; full width suits a photo essay.
- **Use Separator blocks to pace a long read.** They give the eye somewhere to rest, which excerpts and subheadings alone don't.
- **Put the Back button at the end.** A reader who has finished wants a way onward; one who has just arrived doesn't need an exit.
- **Match the date format to the blog page.** Both have their own setting, and they should agree.

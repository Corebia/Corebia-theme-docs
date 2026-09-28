---
title: Related articles
layout: default
parent: Sections
nav_order: 41
permalink: /sections/related-articles/
---

# Related articles

**Related articles** closes an article with a short row of other articles from the same blog, so a reader who reached the end has somewhere to go next.

It can only be added to the article template, where it already sits below the main article. See [Article page](../../templates/article-page/).

## Settings

- **Color scheme.** Default: scheme-1.
- **Heading.** Default: `Related articles`.
- **Articles shown.** Range: 2 to 4. Default: 3.
- **Show image.** The article's featured image on each card. Default: on.
- **Show reading time.** Default: off.

Each card always shows the title and the date.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 60 px and 110 px. This is the padding on screens 1920 px and wider; it scales down on smaller screens.

## How articles are chosen

1. Articles from the same blog that share at least one tag with the one being read, newest first.
2. If that leaves room, the blog's other newest articles fill the rest.

The article being read is never included. Only the blog's 50 newest articles are considered. A blog with a single article has nothing to show, and the section stays hidden on your storefront; the theme editor shows a note in its place.

## Tips

- **Tag your articles.** Without tags the row is simply your latest posts. With them it becomes genuinely related reading.
- **Three is the natural number.** Two looks thin under a long article, and four makes small cards on a laptop.
- **Turn on reading time for long-form blogs.** It helps a reader decide whether to start the next one now.

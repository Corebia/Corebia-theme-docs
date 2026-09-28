---
title: Journal
layout: default
parent: Sections
nav_order: 40
permalink: /sections/journal/
---

# Journal

**Journal** puts up to three blog articles on a page as editorial cards, a grid or a plain list, with an optional "View all" link through to the blog. You can pick each article by hand, or let the section show the latest ones from a blog.

It can go on any template, and can't be placed in the header or footer groups. The home page ships with one, pointed at the `news` blog.

## Settings

- **Color scheme.** Default: scheme-1.

### Content

- **Subheading.** Optional. Small text above the heading.
- **Heading.** Default: `From the journal`.
- **Blog.** Where the "View all" link points. It also fills any Article block you leave empty, with the blog's article at the same position: the first block gets the latest article, the second block the one before it, and so on.
- **Show "View all" link.** Default: on.
- **"View all" label.** Default: `View all`. Shown when the link is on.

### Card

- **Layout.** **Editorial** (default), **Grid** or **List**. List shows each article's date, title and first tag, without images.
- **Show editorial numerals (01, 02, 03).** Default: on.
- **Show article tag.** Shows the article's first tag on the card. Default: off.
- **Show one-line excerpt.** Default: off.
- **Image ratio.** **Landscape (3:2)** (default), **Square (1:1)** or **Portrait (4:5)**.

The last four settings are hidden with the **List** layout, which has no images or numerals.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 120 px in 4 px steps. Default: 80 px each.

## Blocks

Up to **three** Article blocks.

- **Article.** The article to show in this slot. Leave it empty to show the chosen blog's article at this position instead.

The section hides itself only when no article is picked and no blog is chosen. A blog with no articles yet still shows the heading, so the section stays visible while you set it up.

## Tips

- **Leave the blocks empty to keep it current.** With a **Blog** chosen and the Article blocks left empty, the section always shows your latest posts. Pick articles by hand only when you want to hold a particular story in place.
- **Give every featured article a featured image.** The card is mostly image, and an article without one leaves a gap the numerals can't fill.
- **Use List for text-led blogs.** When your articles don't have strong photography, the List layout keeps the section tidy instead of showing weak images large.
- **Numerals or tags, rarely both.** The numerals give the row its editorial rhythm; tags give it information. Turning on both crowds the card.
- **Excerpts are off for a reason.** The cards are designed to work on headline and image alone. Turn excerpts on only if your headlines are too oblique to stand by themselves.

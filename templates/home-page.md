---
title: Home page
layout: default
parent: Templates
nav_order: 1
permalink: /templates/home-page/
---

# Home page

The storefront entry point, at `/`. It uses `index.json`, so the entire section list is yours to arrange from the theme editor.

## Sections it ships with

A fresh install of Pave opens with these seven, in this order:

1. [Hero banner](../../sections/hero/) — a full-height photograph carrying the brand name.
2. [New arrivals](../../sections/new-arrivals/) — a row of hand-picked products.
3. [Brand message](../../sections/brand-message/) — copy beside an image, with a button.
4. [Collection list](../../sections/collection-list/) — collections as image tiles.
5. [Journal](../../sections/journal/) — up to three blog articles.
6. [Brand image](../../sections/brand-image/) — a full-width photograph, no text.
7. [Newsletter](../../sections/newsletter/) — email signup.

Select any of them in the editor to change its settings, or use **Add section** to insert others.

## Sections you can add

Any section not restricted to the header or footer group:

- [Hero banner](../../sections/hero/)
- [New arrivals](../../sections/new-arrivals/)
- [Brand message](../../sections/brand-message/)
- [Collection list](../../sections/collection-list/)
- [Brand image](../../sections/brand-image/)
- [Journal](../../sections/journal/) — home page only
- [Newsletter](../../sections/newsletter/)
- [Rich text with image](../../sections/rich-text-image/)
- [Customer reviews](../../sections/customer-reviews/)
- [FAQ](../../sections/faq/)
- [Recently viewed](../../sections/recently-viewed/)
- [Featured product](../../sections/featured-product/)
- [Product recommendations](../../sections/product-recommendations/)
- [Custom Liquid](../../sections/custom-liquid/)

The [Newsletter popup](../../sections/newsletter-popup/) also appears here in the editor, though it overlays every page rather than sitting in the home page's flow.

## What the home page does differently

- **The header branding is hidden.** The hero already carries the brand, so the top-left logo or wordmark is suppressed here and shown on every other page.
- **The navigation panel opens on hover.** The hover trigger zone in the top-right corner is active only on the home page; everywhere else the panel opens on click.

## Tips

- **Lead with brand, then product.** Pave is designed for a hero-first home page. Move products higher only if your traffic already knows what it wants.
- **Four to seven sections.** Fewer feels unfinished; more turns the home page into a scroll nobody reaches the end of.
- **Replace every default string before publishing.** `Crafted with intention`, `Collections`, `From the journal` and the sample paragraphs all ship with the theme and read as sample text.
- **Don't put Recently viewed here.** A first-time visitor has no history, so the section renders nothing; a returning one is shown their own past before anything new.
- **Set the Journal articles when you publish.** They are chosen by hand and stay chosen until you change them.

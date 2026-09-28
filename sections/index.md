---
title: Sections
layout: default
nav_order: 4
has_children: true
permalink: /sections/
---

# Sections

Sections are the building blocks of every page in Pave. Most can be added, removed and reordered from the theme editor without touching code, and many take blocks you can add, reorder and duplicate inside them.

The pages below document every section a merchant can configure. **Header**, **Announcement bar** and **Footer** live in the header and footer groups and appear on every page. The **Newsletter popup** is part of the theme's layout and stays off until you turn it on. The rest are added to individual templates.

Sections that make up a specific template, such as the product page, the cart and the blog, are documented under [Templates](../templates/) instead, because they can't be moved between templates.

## Global

- [Header](header/)
- [Footer](footer/)
- [Announcement bar](announcement-bar/)
- [Predictive search](predictive-search/)
- [Newsletter popup](newsletter-popup/)

## Banners and storytelling

- [Hero banner](hero/)
- [Slideshow](slideshow/)
- [Media with content](media-with-content/)
- [Brand image](brand-image/)
- [Brand message](brand-message/)
- [Rich text with image](rich-text-image/)
- [Marquee](marquee/)
- [Collage](collage/)
- [Scrollytelling](scrollytelling/)
- [Section](section/)

## Products and collections

- [New arrivals](new-arrivals/)
- [Collection list](collection-list/)
- [Collection links](collection-links/)
- [Collection tabs](collection-tabs/)
- [Shop by colour](shop-by-color/)
- [Featured product](featured-product/)
- [Shoppable image](shoppable-image/)
- [Shoppable videos](shoppable-videos/)
- [Complete the look](complete-the-look/)
- [Product recommendations](product-recommendations/)
- [Complementary products](complementary-products/), a mode of Product recommendations
- [Recently viewed](recently-viewed/)
- [Quick order list](quick-order-list/)
- [Drop](drop/)

## Content and engagement

- [Journal](journal/)
- [Related articles](related-articles/)
- [Newsletter](newsletter/)
- [Customer reviews](customer-reviews/)
- [FAQ](faq/)
- [Contact form](contact-form/)
- [Store locations](store-locations/)

## Advanced

- [Custom Liquid](custom-liquid/)
- [Theme blocks](theme-blocks/): the headings, text, buttons, images, groups and other blocks that several sections share

## Where each section can go

| Section | Where it can be placed |
|---|---|
| Header, Announcement bar | Header group only |
| Footer | Footer group only |
| Newsletter, Section | Any template and the footer group, not the header group |
| Custom Liquid | Anywhere, including the header and footer groups |
| Quick order list | Product templates only |
| Related articles | Article template only |
| Newsletter popup | Part of the layout on every page; it can't be added or moved |
| Everything else | Any template, not the header or footer groups |

A few sections can't be added from the editor at all, because the theme uses them behind the scenes: **Predictive search** fills the search results panel, **Search empty state** fills that panel before anything is typed, **Product card fragment** lets [Recently viewed](recently-viewed/) fetch one product card at a time, **Product quick view** fills the quick view popup, and **Cart drawer** and **Cart suggestions** render the cart drawer and its product suggestions. What you can change about them lives in theme settings: see [Search](../theme-settings/search/), [Product cards](../theme-settings/product-cards/) and [Cart settings](../theme-settings/cart-settings/).

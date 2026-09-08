---
title: Sections
layout: default
nav_order: 4
has_children: true
permalink: /sections/
---

# Sections

Sections are the building blocks of every page in Pave. Most can be added, removed and reordered from the theme editor without touching code.

The pages below document every section a merchant can configure. **Header**, **Footer**, **Announcement bar** and **Predictive search** live in the header and footer groups and appear on every page; the rest are added to individual templates.

Sections that make up a specific template, such as the product page, the cart and the blog, are documented under [Templates](../templates/) instead, because they can't be moved between templates.

## Global

- [Header](header/)
- [Footer](footer/)
- [Announcement bar](announcement-bar/)
- [Predictive search](predictive-search/)

## Home page and content

- [Hero banner](hero/)
- [New arrivals](new-arrivals/)
- [Brand message](brand-message/)
- [Collection list](collection-list/)
- [Brand image](brand-image/)
- [Journal](journal/)
- [Newsletter](newsletter/)
- [Newsletter popup](newsletter-popup/)
- [Rich text with image](rich-text-image/)
- [Customer reviews](customer-reviews/)
- [FAQ](faq/)

## Product and merchandising

- [Recently viewed](recently-viewed/)
- [Featured product](featured-product/)
- [Product recommendations](product-recommendations/)
- [Complementary products](complementary-products/)

## Advanced

- [Custom Liquid](custom-liquid/)

## Where each section can go

| Section | Where it can be placed |
|---|---|
| Header, Predictive search | Header group only |
| Announcement bar | Header group only |
| Footer | Footer group only |
| Journal | Home page only |
| Newsletter | Any template except the header group |
| Everything else | Any template except the header and footer groups |

One further section, **Product card fragment**, has no settings and can't be added from the editor. It exists so that [Recently viewed](recently-viewed/) can fetch one product card at a time over the network, keeping card markup identical to every other grid in the theme. It needs no configuration.

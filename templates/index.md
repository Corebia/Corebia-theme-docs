---
title: Templates
layout: default
nav_order: 5
has_children: true
permalink: /templates/
---

# Templates

A **template** is the layout used to render one kind of page. Pave ships a template for every page type Shopify recognises. Most are JSON templates, which means their sections can be added, removed and reordered from the theme editor.

- [Home page](home-page/)
- [Product page](product-page/)
- [Collection page](collection-page/)
- [Catalog page](catalog-page/)
- [Collections list page](collection-list/)
- [Cart page](cart-page/)
- [Search page](search-page/)
- [Blog page](blog-page/)
- [Article page](article-page/)
- [Page](page/)
- [Contact page](contact-page/)
- [404 page](404-page/)
- [Gift card page](gift-card-page/)
- [Password page](password-page/)
- [Policy page](policy-page/)
- [Customer pages](customer-pages/)

## Which are editable in the theme editor

| Template | Type | Sections |
|---|---|---|
| Home, product, collection, catalog, collections list, cart, search, blog, article, page, contact, 404, password | JSON | Add, remove and reorder freely |
| Gift card, policy | Liquid | Fixed layout, no editor sections |
| Customer pages | n/a | Rendered by Shopify; see [Customer pages](customer-pages/) |

## Alternate templates

An alternate template is a variant you assign to individual products, collections, pages or articles, leaving the rest on the default.

Pave ships two:

- **Catalog** (`collection.all.json`), the `/collections/all` page, documented as [Catalog page](catalog-page/).
- **Contact** (`page.contact.json`), documented as [Contact page](contact-page/).

To make your own, open the theme editor's template picker and choose **Create template**, then assign it to a product or page under that item's **Theme template** setting in the Shopify admin. See [Shopify Help: Alternate templates](https://help.shopify.com/en/manual/online-store/themes/templates).

---
title: Templates
layout: default
nav_order: 5
has_children: true
permalink: /templates/
---

# Templates

A **template** is the layout used to render one kind of page. Pave ships a template for every page type Shopify recognizes, plus a set of alternate templates for products, collections and pages that need a different layout. Most are JSON templates, which means their sections can be added, removed and reordered from the theme editor.

- [Home page](home-page/)
- [Product page](product-page/)
- [Alternate product templates](product-templates/)
- [Collection page](collection-page/)
- [Catalog page](catalog-page/)
- [Lookbook collection page](lookbook-collection/)
- [Collections list page](collection-list/)
- [Search page](search-page/)
- [Cart page](cart-page/)
- [Blog page](blog-page/)
- [Article page](article-page/)
- [Page](page/)
- [Contact page](contact-page/)
- [Alternate page templates](page-templates/)
- [404 page](404-page/)
- [Gift card page](gift-card-page/)
- [Password page](password-page/)
- [Policy page](policy-page/)
- [Customer pages](customer-pages/)

## Which are editable in the theme editor

| Template | Type | Sections |
|---|---|---|
| Home, product, collection, catalog, collections list, search, cart, blog, article, page, 404, password, and every alternate template | JSON | Add, remove and reorder freely |
| Gift card, policy | Liquid | Fixed layout, no editor sections |
| Customer pages | n/a | Rendered by Shopify; see [Customer pages](customer-pages/) |

## Alternate templates

An alternate template is a variant you assign to individual products, collections or pages, leaving the rest on the default. Pave ships these:

| Template | For | Documented in |
|---|---|---|
| `product.editorial` | A product with a story told below the buy box | [Alternate product templates](product-templates/#editorial) |
| `product.gift-card` | Your gift card product | [Alternate product templates](product-templates/#gift-card) |
| `product.quick-order` | Ordering many variants at once | [Alternate product templates](product-templates/#quick-order) |
| `collection.all` | The `/collections/all` catalog | [Catalog page](catalog-page/) |
| `collection.lookbook` | A collection presented as a campaign | [Lookbook collection page](lookbook-collection/) |
| `page.contact` | A contact page with a form and your details | [Contact page](contact-page/) |
| `page.about` | An about page | [Alternate page templates](page-templates/#about) |
| `page.accessibility` | An accessibility statement | [Alternate page templates](page-templates/#accessibility) |
| `page.contact-stores` | Store locations with a contact form | [Alternate page templates](page-templates/#contact-and-stores) |
| `page.drop` | A product launch, with a waitlist until it goes live | [Alternate page templates](page-templates/#drop) |
| `page.editorial` | A shoppable editorial story | [Alternate page templates](page-templates/#editorial) |
| `page.faq` | Frequently asked questions | [Alternate page templates](page-templates/#faq) |
| `page.lookbook` | A shoppable lookbook | [Alternate page templates](page-templates/#lookbook) |
| `page.size-guide` | A size guide | [Alternate page templates](page-templates/#size-guide) |

### Assigning an alternate template

1. In Shopify admin, open the product, collection or page.
2. Under **Theme template**, choose the template by its name, such as **editorial** or **faq**, and save.
3. To edit an alternate template, open the theme editor and choose it from the template menu at the top, under **Products**, **Collections** or **Pages**. Changes apply to everything assigned to that template.

### Making your own

Open the template menu in the theme editor and choose **Create template**. Name it, pick the template to base it on, then change its sections. Assign it the same way as above. See [Shopify Help: Alternate templates](https://help.shopify.com/en/manual/online-store/themes/templates).

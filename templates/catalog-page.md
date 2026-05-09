---
title: Catalog page
layout: default
parent: Templates
nav_order: 4
permalink: /templates/catalog-page/
---

# Catalog page

The **Catalog page** is the all-products view at `/collections/all`. It uses a separate `collection.all.json` template that renders the **Main catalog** section, which includes a sidebar with quick navigation and the full product grid.

## URL

`https://yourstore.com/collections/all`

## Sections included by default

1. **Main catalog** — The full catalog with sidebar.

## Main catalog section

### Catalog heading

- **Show catalog heading** — Display a heading above the sidebar and on mobile.
- **Catalog heading** — The heading text. Leave empty to hide. Default: `Catalog`.
- **Heading link** — Optional URL the heading links to.
- **Quick navigation menu** — Menu shown at the top of the sidebar. Set to a Shopify menu (for example, the main menu) to give customers a way to filter by category from the catalog page.

### Filters and toolbar

- **Show filters** — Toggle the filter panel.
- **Show sort options** — Toggle the sort dropdown.

### Product grid

- **Products per page** — How many products to load per page.
- **Desktop columns** — Options: **2 columns**, **3 columns**, **4 columns**.
- **Show vendor** — Display vendor on each card.
- **Show second image on hover** — Displays alternate product image on hover.
- **Show quick view button** — Adds a quick-view button on hover.

### Other

- **Show back link and breadcrumb** — Toggle.
- **Color scheme** — Default: scheme-1.

## Special behaviors

- **Sidebar navigation** — The catalog page is unique in showing a persistent left sidebar with the quick-navigation menu, filters, and sort. Customers can scope by collection without leaving the catalog view.
- **Mobile** — The sidebar collapses into a slide-in drawer on mobile to preserve grid space.

## When to use

The catalog page is ideal for stores where customers want to browse the full catalog rather than dive into specific collections. If your store is collection-driven (each collection has a strong identity and customers usually arrive via a collection link), you may not need to feature the catalog page at all.

## When not to use

If your catalog is small (under ~30 products), the catalog page and the home page can feel redundant. Consider using a single Collection list section on the home page instead and routing customers directly to collections.

## Tips

- **Quick navigation menu** — Use a flat list of top-level collection links. Avoid deep nesting in this menu — the sidebar is a quick filter, not a full menu.
- **Heading link** — If you want the heading to link back to the home page or a marketing landing page, set the URL here. Leave blank for a non-clickable heading.

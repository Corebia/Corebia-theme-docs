---
title: Navigation
layout: default
parent: Features
nav_order: 1
permalink: /features/navigation/
---

# Navigation

Pave navigates from a side panel. A button fixed at the top right opens a panel from the right carrying the menu, search, the customer account, the cart and your policy links. On the home page the panel also opens on hover, in the top-right corner.

There is no mega-menu. The design puts one focused panel in front of the shopper rather than a bar of dropdowns.

## Menus live in Shopify, not in the theme

Pave stores no menus of its own. Build them under `Shopify admin > Online Store > Navigation`, then point a block at one.

| Menu | Used by | Default handle |
|---|---|---|
| Main menu | The **Navigation** block on the [Header](../../sections/header/) | `main-menu` |
| Footer | The **Footer navigation** block on the [Footer](../../sections/footer/) | `footer` |
| Customer account menu | The account panel in the header | none — optional |

## Three levels in the panel

The header panel renders up to three levels of nesting:

1. A top-level link.
2. Its children.
3. Their children.

Sub-menus expand in place, inside the panel. To build them, drag a menu item under another in the Shopify navigation editor so it indents.

The footer renders **one** level. Sub-menus in a footer menu are not shown, so give each footer column its own flat menu rather than nesting.

## Adding a link that isn't in a menu

The header also takes **Custom link** blocks — a label and a URL, added directly in the theme editor. Use them for one-off links that don't belong in your main navigation structure.

## What is in the panel without configuration

Search, the customer account, the cart count and your policy links all appear on their own. Policy links show only for the policies you have actually written under `Shopify admin > Settings > Policies`.

## Tips

- **Keep the top level short.** Five to seven items is what a shopper can take in. Depth belongs on levels two and three.
- **Name links for what a shopper wants, not for how your catalog is organised.** "Coats" beats "Outerwear FW26".
- **Order the footer menu differently from the header.** The footer is where people look for help, policies and contact, not for products.
- **Test the panel on a phone.** It takes the full screen there, and three levels of a deep menu is a lot of tapping.

## Related

- [Header section reference](../../sections/header/)
- [Footer section reference](../../sections/footer/)
- [Search](../search/)

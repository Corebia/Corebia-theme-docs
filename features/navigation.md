---
title: Navigation
layout: default
parent: Features
nav_order: 1
permalink: /features/navigation/
---

# Navigation

Pave navigates from two places that share one menu: a bar across the top of the page on desktop, and a side panel that opens from the menu button.

## The desktop bar

From 990 px wide, the header shows an inline bar with your logo, the top-level links of your main menu, search and the cart. This is the default. The header's **Desktop menu style** setting switches it to **Menu panel (hamburger only)**, which keeps the menu button as the only navigation, for a quieter page.

In the bar, a top-level link that has children opens a **mega menu**: one column per child link, each with its own children listed below it, plus a link to the parent itself. The **Navigation** block's **Menu style** decides what the columns look like:

- **Text columns.** Headings and links only.
- **Collection images.** Each column that points at a collection shows the collection's image.
- **Product images.** Each column that points at a product shows the product's image.

Images come from the collection or product the menu item links to, so there is nothing to upload. A **Menu promotion** block adds an image tile with a heading, text and a link at the end of every mega menu.

## The side panel

Below 990 px, and on desktop when the bar is turned off, the menu button opens a panel carrying the menu, search, the cart and your policy links. The customer account icon sits beside the menu button rather than inside the panel, so it is always one tap away. On the home page, the panel also opens when the pointer rests in the top corner of the screen; **Hover trigger size** sets how large that corner is.

With the inline bar, desktop screens show the menu button only when the panel carries something the bar doesn't: a **Custom link** block, a second **Navigation** block, the Follow on Shop button, or a B2B buyer's locations. When the bar already shows everything, the menu button and the hover corner are left out, and the bar is the only navigation on desktop.

The panel renders up to three levels of nesting. Sub-menus expand in place, inside the panel. To build them, drag a menu item under another in the Shopify navigation editor so it indents.

## Menus live in Shopify, not in the theme

Pave stores no menus of its own. Build them under `Shopify admin > Online Store > Navigation`, then point a block at one.

| Menu | Used by | Default handle |
|---|---|---|
| Main menu | The **Navigation** block on the [Header](../../sections/header/), for both the bar and the panel | `main-menu` |
| Footer | The **Footer navigation** blocks on the [Footer](../../sections/footer/) | `footer` |
| Customer account menu | The account sheet opened from the account icon | none, optional |

The footer renders **one** level. Sub-menus in a footer menu are not shown, so give each footer column its own flat menu rather than nesting.

## Adding a link that isn't in a menu

The header also takes **Custom link** blocks: a label and a URL, added directly in the theme editor. Use them for one-off links that don't belong in your main navigation structure.

## What is there without configuration

Search, the customer account icon, the cart count and your policy links all appear on their own. Policy links show only for the policies you have actually written under `Shopify admin > Settings > Policies`.

## Other navigation settings

The [Header](../../sections/header/) section also sets:

- **Sticky header.** Whether the header stays on screen as the page scrolls, reappears when the shopper scrolls up, or scrolls away.
- **Show back-to-top button.** A button that appears after about a screen of scrolling. Off by default.
- **Show mobile bottom navigation.** A bar fixed to the bottom of the screen below 990 px, with links to the home page, search, the cart and the account. Off by default.

Most pages also open with a back link and a breadcrumb trail, controlled by each template's **Show back link and breadcrumb** setting. The back link returns to the previous page in your store, and the breadcrumb traces the path from the home page, so an article reads `Home / <blog title> / <article title>`. Policy pages have a back link only, under **Show back link**, and the cart page opens with a back link to your catalog. Long page names are shortened with an ellipsis so the row stays on one line.

## Tips

- **Keep the top level short.** Five to seven items fit the desktop bar and are what a shopper can take in. Depth belongs in the mega menu.
- **Name links for what a shopper wants, not for how your catalog is organized.** "Coats" beats "Outerwear FW26".
- **Point mega menu columns at collections.** With **Collection images** it is the collection's own image that shows, so a menu of collections looks finished with no extra work.
- **Order the footer menu differently from the header.** The footer is where people look for help, policies and contact, not for products.
- **Test the panel on a phone.** It takes the full screen there, and three levels of a deep menu is a lot of tapping.

## Related

- [Header section reference](../../sections/header/)
- [Footer section reference](../../sections/footer/)
- [Search](../search/)

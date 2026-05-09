---
title: Header
layout: default
parent: Sections
nav_order: 1
permalink: /sections/header/
---

# Header

The **Header** section renders Pave's signature side-panel navigation. It appears on every page of the storefront. The toggle button (hamburger) sits fixed at the top right; opening it slides in a panel from the right with the menu, search, account, cart, and policy links.

On the home page, the panel can also open by hovering over the top-right corner of the page (a **Hover trigger size** zone).

## Settings

### Branding

- **Show shop branding** — Displays the shop logo or name in the top left of every page except the home page. Default: off.
- **Brand text** — Defaults to the shop name if left empty. Only visible when no logo is set.
- **Brand text size** — Size of the brand text in pixels. Range: 10 to 32 px in 1 px steps. Default: 16 px.
- **Brand link** — The URL the top-left brand element links to. Defaults to the home page if left empty.

### Navigation panel

- **Shop name link** — The URL the large shop name inside the panel links to. Defaults to the home page if left empty.
- **Menu title text** — The large heading shown at the top of the navigation panel. Defaults to the shop name if left empty.
- **Menu title size** — Size of the menu title in pixels. Range: 16 to 48 px in 2 px steps. Default: 28 px.
- **Panel width** — Width of the navigation panel as a percentage of the viewport. Range: 25% to 50% in 5% steps. Default: 35%. On mobile the panel always takes the full screen.
- **Hover trigger size** — Size of the invisible hover zone at the top-right of the home page that opens the panel on hover. Range: 80 to 300 px in 10 px steps. Default: 150 px.
- **Color scheme** — The color scheme applied to the navigation panel. Default: scheme-1.

## Blocks

The header accepts two block types. Add blocks via **Add navigation menu** or **Add custom link**. You can mix and match in any order.

### Navigation menu

Renders a Shopify navigation as a vertical link list inside the panel. Supports up to three nesting levels (parent, sub-menu, sub-sub-menu).

- **Menu** — The Shopify navigation to render. Default: `main-menu`.

### Custom link

Adds a single inline link to the panel.

- **Link label** — The text to display.
- **Link URL** — The URL the link points to.

## Fixed elements

The following are always rendered and are not configurable:

- **Cart link** — Reads `Cart (n)` showing the live cart item count.
- **Search trigger** — Opens an inline expandable search field with predictive search results.
- **Account link** — Shown when customer accounts are enabled in your Shopify admin. Switches between **Account** (signed in) and **Log in** (signed out) automatically.
- **Legal footer** — Privacy policy, Terms of service, Refund policy, and Shipping policy links. Each link is rendered only if the corresponding policy is configured in `Shopify admin > Settings > Policies`.

## Tips

- **Show shop branding** is intentionally off on the home page — the hero banner already carries the brand. On other pages, the branding is the entry point back to the home page.
- **Hover trigger size** only applies on the home page. On all other pages, the panel only opens on click. Lower the value for a calmer experience; raise it if customers are missing the trigger.
- For a large catalog, structure the **main-menu** in your Shopify admin with parent items and sub-menus. The panel renders all three levels.

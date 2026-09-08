---
title: Header
layout: default
parent: Sections
nav_order: 1
permalink: /sections/header/
---

# Header

The **Header** section renders Pave's side-panel navigation. It appears on every page of the storefront. The toggle button sits fixed at the top right; opening it slides in a panel from the right carrying the menu, search, the customer account, the cart and your policy links.

On the home page the panel can also open by hovering over the top-right corner, inside the zone set by **Hover trigger size**.

The Header lives in the `header` section group, so it can't be removed or placed on an individual template.

## Settings

### Branding

- **Show shop branding** — Displays the shop logo or name in the top left of every page except the home page. Default: off.
- **Brand text** — Defaults to the shop name if left empty. Only visible when no logo is set.
- **Brand text size** — Range: 10 to 32 px in 1 px steps. Default: 16 px.
- **Brand link** — Where the top-left brand element links to. Defaults to the home page if left empty.

### Navigation panel

- **Shop name link** — Where the large shop name inside the panel links to. Defaults to the home page if left empty.
- **Navigation heading text** — The large heading at the top of the panel. Defaults to the shop name if left empty.
- **Navigation heading size** — Range: 16 to 48 px in 2 px steps. Default: 28 px.
- **Panel width** — Width of the panel as a percentage of the viewport. Range: 25% to 50% in 5% steps. Default: 35%. On mobile the panel always takes the full screen.
- **Customer account menu** — The menu shown inside the customer account panel. Leave empty to use the default account links.
- **Show Follow on Shop** — Lets shoppers follow your store on the Shop app from the navigation panel. Default: on.
- **Hover trigger size** — Size of the invisible hover zone at the top right of the home page that opens the panel. Range: 80 to 300 px in 10 px steps. Default: 150 px.
- **Color scheme** — Applied to the navigation panel. Default: scheme-1.

## Blocks

The header takes two block types, in any order and any mix.

### Navigation

Renders a Shopify navigation as a vertical link list inside the panel. Three nesting levels are supported: parent, sub-menu and sub-sub-menu.

- **Main menu** — The Shopify navigation to render. Default: `main-menu`.

### Custom link

A single inline link in the panel.

- **Link label** — The text to display.
- **Link URL** — Where it points.

## Always present, and not configurable

- **Cart link** — Reads `Cart (n)` with the live item count.
- **Search** — An inline expandable field backed by predictive search. What it returns is configured in the [Predictive search](../predictive-search/) section.
- **Customer account** — Shopify's own account component. It shows a signed-out or signed-in avatar automatically and needs no setup beyond enabling customer accounts in your Shopify admin. Its colors and fonts follow the theme, but its contents are rendered by Shopify, so the only thing the theme controls is which menu appears inside it — see **Customer account menu** above.
- **Follow on Shop button** — Rendered by Shopify when **Show Follow on Shop** is on. Its colors can't be changed, by Theme Store rule.
- **Policy links** — Privacy policy, Terms of service, Refund policy and Shipping policy. Each appears only if that policy is filled in under `Shopify admin > Settings > Policies`.

## Tips

- **Branding starts switched off for a reason.** The home page opens with the hero, which already carries the brand; on every other page the branding is the way back to the home page. Turn it on if your hero doesn't include a wordmark.
- **Hover trigger only applies to the home page.** Everywhere else the panel opens on click. Lower the value for a calmer feel, raise it if shoppers are missing the trigger.
- **Structure the menu in Shopify, not here.** For a large catalog, build `main-menu` in your admin with parent items and sub-menus; the panel renders all three levels without further setup.
- **Leave the customer account menu empty unless you have a reason.** The default account links cover the usual flows. Set a menu when you want to add something of your own, such as a loyalty page.

---
title: Header
layout: default
parent: Sections
nav_order: 1
permalink: /sections/header/
---

# Header

The **Header** appears on every page of the storefront. It has two parts that work together:

- **A desktop bar.** With the default **Inline bar** style, screens 990 px and wider get a header bar with your logo, the top-level links of your menu, search, the country and language selectors and the cart.
- **A navigation panel.** The menu button at the top right opens a panel carrying the full menu, search, the cart, Follow on Shop, the country and language selectors and your policy links. On phones and tablets it is the only navigation, and on desktop it stays available next to the bar.

Wherever the bar isn't shown, a cart icon with the item count and the customer account button sit beside the menu button.

The Header lives in the `header` section group, so it can't be removed or placed on an individual template.

## Settings

### Branding

- **Show shop branding.** Displays the shop logo or name in the top left of every page except the home page. Default: on. On the home page the brand shows only when an **Inverse logo** is set in [Logo](../../theme-settings/logo/), because the hero already carries your name there. From 990 px up, the inline bar shows your logo or brand text in its own place, so this setting governs smaller screens and the **Menu panel** style.
- **Brand text.** Defaults to the shop name if left empty. Only visible when no logo is set.
- **Brand text size.** Range: 10 to 32 px in 1 px steps. Default: 16 px.
- **Brand link.** Where the brand links to. Defaults to the home page if left empty. The logo in the desktop bar uses the same link.

**Brand text**, **Brand text size** and **Brand link** are shown when **Show shop branding** is on.

### Navigation panel

- **Shop name link.** Where the large shop name at the top of the panel links to. Defaults to the home page if left empty.
- **Navigation heading text.** The large heading at the top of the panel. Defaults to the shop name if left empty.
- **Navigation heading size.** Range: 16 to 48 px in 2 px steps. Default: 28 px.
- **Panel width.** Width of the panel as a percentage of the screen. Range: 25% to 50% in 5% steps. Default: 35%.
- **Customer account menu.** The menu shown inside the customer account panel. Leave empty to use the default account links.
- **Show Follow on Shop.** Lets shoppers follow your store on the Shop app from the navigation panel. Default: on.
- **Show country/region selector.** Lets shoppers pick the country they are shopping from, and the currency they see. Only shown when your store sells to more than one country. Default: off.
- **Show language selector.** Lets shoppers pick the storefront language. Only shown when your store has more than one language published. Default: off.
- **Hover trigger size.** Size of the invisible zone at the top right of the home page that opens the panel when a mouse rests on it. Range: 80 to 300 px in 10 px steps. Default: 150 px.

The panel's colors come from theme settings rather than from this section. See [Popovers and drawers](../../theme-settings/popovers/).

### Desktop layout

- **Desktop menu style.** Applies from 990 px up.
  - **Inline bar (links, search and cart in the header)** (default) adds the header bar with the menu's top-level links, search and the cart. Links with children open a mega menu.
  - **Menu panel (hamburger only)** keeps the menu button as the only navigation on every screen size.
- **Logo position.** Where the logo sits in the inline bar. **Left** (default) or **Center**. Shown when **Desktop menu style** is set to the inline bar.
- **Sticky header.** Whether the header stays on screen while the page scrolls. **Always visible** (default), **Show on scroll up** or **Scrolls away with the page**.
- **Show back-to-top button.** Appears after about one screen of scrolling. Returns to the top of the page and moves keyboard focus there. Default: off.
- **Show mobile bottom navigation.** A fixed bar below 990 px with links to the home page, search, the cart and the account. The account link appears only when customer accounts are turned on. Default: off.
- **Color scheme.** Applied to the header bar and the menu button. Default: scheme-1.

## Blocks

The header takes three block types, in any order. It ships with one **Navigation** block pointing at `main-menu`.

### Navigation

Renders a Shopify menu. In the panel it becomes a vertical list with up to three levels: parent, sub-menu and sub-sub-menu. In the inline desktop bar its top-level links become the bar's links, and a link with children opens a mega menu.

- **Main menu.** The Shopify menu to render. Default: `main-menu`.
- **Menu style.** How the desktop mega menu lays out a top-level link's children. **Text columns** (default), **Collection images** or **Product images**. Images come from the collection or product a menu item points at, so an item that links anywhere else shows as text.

Only the first **Navigation** block feeds the desktop bar. Any further menus appear in the panel.

### Custom link

A single link in the navigation panel. It doesn't appear in the desktop bar.

- **Link label.** The text to display.
- **Link URL.** Where it points.

### Menu promotion

A tile shown at the end of every mega menu in the inline desktop bar. With the **Menu panel** style it renders nothing, and it stays hidden until at least one of its fields is filled. The link shows only when both **Link label** and **Link URL** are set.

- **Image.**
- **Heading.**
- **Text.**
- **Link label.**
- **Link URL.**

## Always present, and not configurable

- **Cart.** Reads `Cart (n)` with the live item count in the panel and the desktop bar, and shows as an icon with a count beside the menu button where there is no bar. It opens the cart drawer or the cart page, depending on **Cart type** in [Cart settings](../../theme-settings/cart-settings/).
- **Search.** An expandable field with predictive search, in the panel and in the desktop bar. What it shows before a shopper types is set in [Search](../../theme-settings/search/) in theme settings.
- **Customer account.** Shopify's own account component, shown next to the menu button when customer accounts are turned on in your Shopify admin. It shows a signed-out or signed-in avatar by itself. Its contents are rendered by Shopify, so the only thing the theme controls is which menu appears inside it. See **Customer account menu** above.
- **Follow on Shop button.** Rendered by Shopify when **Show Follow on Shop** is on. Its colors can't be changed, by Theme Store rule.
- **B2B location.** For a signed-in B2B buyer, the company and location they are buying for, with a way to switch location in the panel. Nobody else sees it. See [B2B](../../features/b2b/).
- **Policy links.** Privacy policy, Terms of service, Refund policy and Shipping policy. Each appears only if that policy is filled in under `Shopify admin > Settings > Policies`.

## Tips

- **Build the menu in Shopify, not here.** For a large catalog, set up `main-menu` in your admin with parent items and sub-menus. The panel renders all three levels and the desktop bar turns parents into mega menus without further setup.
- **Point mega menu items at collections for image menus.** **Collection images** only has pictures to show when the child links go to collections, and **Product images** when they go to products.
- **Give the home page an inverse logo.** On phones, and with the **Menu panel** style, the brand is left off the home page so it doesn't sit on top of the hero. A light version of your logo, set as **Inverse logo** in [Logo](../../theme-settings/logo/), brings it back in a version that reads over photography.
- **Switch the selectors on when you sell internationally.** The country and language selectors hide themselves while there is only one choice, so turning them on early does no harm, but there is nothing to show until you add markets or languages.
- **Leave the customer account menu empty unless you have a reason.** The default account links cover the usual flows. Set a menu when you want to add something of your own, such as a loyalty page.

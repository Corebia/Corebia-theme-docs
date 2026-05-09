---
title: Navigation
layout: default
parent: Features
nav_order: 1
permalink: /features/navigation/
---

# Navigation

Pave uses a side-panel navigation pattern. A hamburger button at the top right opens a panel from the right that contains the main menu, search, account, cart, and policy links.

## Where it appears

- The hamburger button and side navigation panel are part of the **Header** section, which is included on every page via the header section group.
- The footer renders one or more menu columns (configured as **Menu** blocks on the Footer section).

## Menus

Navigation in Pave is driven by Shopify menus. Pave does not store menus in theme settings — you create and edit them in `Shopify admin > Online Store > Navigation`.

### Default menus referenced by Pave

- **Main menu** — Used by the **Navigation menu** block in the header.
- **Footer** — Conventionally used as a column in the footer.

### Multi-level menus

Pave's navigation panel supports up to **three levels** of nesting:

1. Top-level link.
2. Sub-menu link (children of a top-level link).
3. Sub-sub-menu link (children of a sub-menu link).

Sub-menus expand on tap (mobile) or hover/tap (desktop), inside the same panel. There is no full-screen mega-menu in Pave — the design favors a focused, editorial side panel.

## Configuring the main menu

1. In `Shopify admin > Online Store > Navigation`, open or create the **Main menu**.
2. Add menu items. Each item can link to a collection, page, blog, article, product, or external URL.
3. To create a sub-menu, drag a menu item under another item, indented to the right.
4. Save.

The header automatically renders the menu in the navigation panel.

## Adding navigation menus to the header

1. Open the theme editor.
2. In the **Header** section, click **Add block**.
3. Pick **Navigation menu**.
4. Set **Menu** to the navigation you created in your admin.

You can add multiple navigation menu blocks to display secondary menus. Reorder them in the section.

## Custom inline links

To add a single link to the panel (not a full menu), use the **Custom link** block on the **Header** section. Set **Link label** and **Link URL**.

## Footer menus

Each **Menu** block in the **Footer** section becomes a column. Set the **Heading** and the **Menu** to render.

## Fixed links

Some links in the navigation panel are always rendered and not configurable:

- **Cart** — Always shown. Reads the live cart count.
- **Search** — Always shown. Opens an inline expandable search field.
- **Account / Log in** — Shown when customer accounts are enabled in your Shopify admin.
- **Policy links** — Privacy policy, Terms of service, Refund policy, Shipping policy. Each appears only if the corresponding policy is configured in `Shopify admin > Settings > Policies`.

## Troubleshooting

- **My menu doesn't appear** — Check that you have a **Navigation menu** block in the header section, and that the **Menu** dropdown points to a real navigation in your admin.
- **My sub-menu items don't appear** — Pave supports up to 3 levels. Items nested at level 4 or deeper are not rendered.
- **I see "Log in" but I'm signed in** — Sign out and sign back in. If the issue persists, check `Shopify admin > Settings > Customer accounts` to confirm accounts are enabled.

## Related

- [Header section reference](../../sections/header/)
- [Footer section reference](../../sections/footer/)

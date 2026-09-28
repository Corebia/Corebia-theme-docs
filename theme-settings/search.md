---
title: Search
layout: default
parent: Theme settings
nav_order: 16
permalink: /theme-settings/search/
---

# Search

What shoppers see when they open search and haven't typed anything yet. These settings fill the empty search drawer, and the same panel on the search page, with products, popular searches and the shopper's own recent searches.

The results that appear once a shopper starts typing come from the [Predictive search](../../sections/predictive-search/) section. See also [Search](../../features/search/) for how search works across the store.

## Settings

- **Featured collection.** Products shown in the search drawer before a shopper types. Leave it empty to show none.
- **Products to show.** Shown once a featured collection is set. Range: 2 to 10. Default: 4.
- **Popular searches menu.** Each menu item becomes a link in the search drawer. Leave it empty to show none.
- **Show recent searches.** Lists the shopper's last 5 searches in the search drawer. The terms are kept in their own browser only, and they can remove any of them. Default: off.

With all three left empty or off, the drawer opens with just the search field. There is deliberately no fallback to every product in the store.

## Building the popular searches menu

Create a menu under `Shopify admin > Content > Menus`, for example called `Popular searches`, and add one item per link. Each item can point anywhere: a collection, a product, a page, or a search results URL such as `/search?q=linen`. The item's title is what the shopper sees.

Then choose that menu in **Popular searches menu**.

## Tips

- **Feature what people come for.** New arrivals or best sellers make a better featured collection than a seasonal edit most visitors won't recognize.
- **Four products fit a phone.** More than four means scrolling before the shopper has typed a word.
- **Keep popular searches short and real.** Five or six links, taken from what shoppers actually search for, which the reports under `Shopify admin > Analytics` can show you.
- **Recent searches help returning shoppers.** Stores where people come back to compare, such as furniture or gifts, benefit most. The terms never leave the shopper's browser.

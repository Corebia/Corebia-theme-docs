---
title: Customer pages
layout: default
parent: Templates
nav_order: 16
permalink: /templates/customer-pages/
---

# Customer pages

The pages a customer uses to manage their account: signing in, viewing orders, editing addresses.

**Pave ships no customer templates, and that is deliberate.** These pages are rendered by Shopify, not by the theme, so there is nothing in the theme editor to configure and no sections to add. They follow your store's branding rather than the theme's sections.

## How customers reach their account

The account entry point lives in the navigation panel of the [Header](../../sections/header/). It is Shopify's own account component: it shows a signed-out or a signed-in state automatically, and needs no setup beyond enabling customer accounts.

The one thing the theme controls is which menu appears inside the account panel, through the header's **Customer account menu** setting. Leave it empty to use Shopify's default account links.

## Turning accounts on

Under `Shopify admin > Settings > Customer accounts`. Shopify offers:

- **Accounts are optional** — customers can create one or check out as a guest.
- **Accounts are required** — customers must sign in to check out.
- **Accounts are disabled** — guest checkout only. The account entry point in the header disappears.

Shopify's current customer accounts use a code sent by email rather than a password. Order history, order detail, addresses and profile all live on Shopify's own pages.

## What customers can do there

- **Order history** — past orders with status and totals.
- **Order detail** — line items, addresses, fulfilment status and tracking.
- **Addresses** — saved shipping addresses for faster checkout.
- **Subscriptions** — where you sell on selling plans, the schedule and management options your subscription app provides.

## Tips

- **Decide before launch.** Requiring accounts reduces guest-checkout friction to zero at the cost of some conversion; optional is the safe default for most stores.
- **Account emails are yours to write.** The sign-in code, order confirmation and shipping notifications are configured under `Shopify admin > Settings > Notifications`, not in the theme.
- **Test signed in and signed out.** Some of the storefront changes between the two — the [Newsletter popup](../../sections/newsletter-popup/), for instance, never shows to a signed-in customer.

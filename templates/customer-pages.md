---
title: Customer pages
layout: default
parent: Templates
nav_order: 19
permalink: /templates/customer-pages/
---

# Customer pages

The pages a customer uses to manage their account: signing in, viewing orders, editing addresses.

**Pave ships no customer templates, and that is deliberate.** These pages are rendered by Shopify, not by the theme, so there is nothing in the theme editor to configure and no sections to add. They follow the branding you set for customer accounts in your Shopify admin rather than the theme's sections.

## How customers reach their account

The account entry point sits in the [Header](../../sections/header/), at the top right, beside the menu button when there is one, on every page and at every screen size. It is Shopify's own account component: it shows a signed-out or a signed-in avatar automatically, opens its own account sheet, and needs no setup beyond enabling customer accounts.

The one thing the theme controls is which menu appears inside that sheet, through the header's **Customer account menu** setting. Leave it empty to use Shopify's default account links.

On phones and tablets, the header's fixed bottom bar also links to the account when **Show mobile bottom navigation** is on.

## Turning accounts on

Under `Shopify admin > Settings > Customer accounts`. Shopify offers:

- **Accounts are optional.** Customers can create one or check out as a guest.
- **Accounts are required.** Customers must sign in to check out.
- **Accounts are disabled.** Guest checkout only. The account entry point in the header disappears.

Shopify's current customer accounts use a code sent by email rather than a password. Order history, order detail, addresses and profile all live on Shopify's own pages.

## What customers can do there

- **Order history.** Past orders with status and totals.
- **Order detail.** Line items, addresses, fulfillment status and tracking.
- **Addresses.** Saved shipping addresses for faster checkout.
- **Subscriptions.** Where you sell on selling plans, the schedule and management options your subscription app provides.

## B2B buyers

Buyers who sign in to a company account see the company and location they are buying for in the header, and, where they can buy for more than one location, can switch location from the menu panel. See [B2B](../../features/b2b/).

## Tips

- **Decide before launch.** Requiring accounts removes guest checkout entirely, at the cost of some conversion; optional is the safe default for most stores.
- **Account emails are yours to write.** The sign-in code, order confirmation and shipping notifications are configured under `Shopify admin > Settings > Notifications`, not in the theme.
- **Test signed in and signed out.** Some of the storefront changes between the two. The [Newsletter popup](../../sections/newsletter-popup/), for instance, never shows to a signed-in customer.

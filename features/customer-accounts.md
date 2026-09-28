---
title: Customer accounts
layout: default
parent: Features
nav_order: 17
permalink: /features/customer-accounts/
---

# Customer accounts

Pave puts a customer account entry point in the header on every page, so a shopper can sign in, check an order or reorder without hunting for it.

## Where it appears

In the [Header](../../sections/header/), as an avatar icon at the top right, beside the menu button when there is one, on both desktop and mobile. It is always present while customer accounts are enabled, with no setting to hide it, and it shows a signed-out or a signed-in state on its own. When **Show mobile bottom navigation** is on in the header, the bottom bar also carries an account link.

## It is rendered by Shopify

The account entry point is Shopify's own component, not theme markup. That has three consequences worth knowing:

- **It needs no setup.** Enable customer accounts in your admin and it works.
- **Its contents are Shopify's.** Order history, addresses and profile live on Shopify's pages, and the theme ships no customer templates. See [Customer pages](../../templates/customer-pages/).
- **Its colors and fonts follow the theme**, but its structure does not. There is nothing to lay out.

## What you control

One thing: the menu shown inside the account sheet, through the header's **Customer account menu** setting. Leave it empty to use Shopify's default account links, or point it at a menu of your own to add something like a loyalty page or a returns portal.

## Turning accounts on

Under `Shopify admin > Settings > Customer accounts`:

- **Accounts are optional.** Customers can create one or check out as a guest. The safe default.
- **Accounts are required.** Customers must sign in to check out.
- **Accounts are disabled.** Guest checkout only, and the entry point disappears from the header.

## B2B buyers

A customer who buys for a company sees the company and location they are ordering for in the header, and can switch location there when they have more than one. See [B2B](../b2b/).

## Signing in

Shopify's current customer accounts sign in with a code sent by email rather than a password, so there is no password to reset and nothing for the theme to render.

## Tips

- **Optional accounts suit most stores.** Requiring them removes guest checkout, which costs conversion on a first purchase.
- **Signing in changes the storefront.** A signed-in customer never sees the [Newsletter popup](../../sections/newsletter-popup/), so test both states.
- **Account emails are yours.** The sign-in code and order notifications are written under `Shopify admin > Settings > Notifications`, not in the theme.

## Related

- [Header section reference](../../sections/header/)
- [Customer pages](../../templates/customer-pages/)
- [Follow on Shop](../follow-on-shop/)
- [B2B](../b2b/)

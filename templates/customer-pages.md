---
title: Customer pages
layout: default
parent: Templates
nav_order: 16
permalink: /templates/customer-pages/
---

# Customer pages

**Customer pages** are the pages a signed-in customer uses to manage their account: log in, register, view orders, view a single order, and edit addresses.

Pave uses Shopify's classic customer accounts, which means the visual style of customer pages follows the theme's base styling but is largely controlled by Shopify, not by per-template sections. There are no per-template editor sections for customer pages.

## URLs

- `https://yourstore.com/account/login` — Log in
- `https://yourstore.com/account/register` — Create an account
- `https://yourstore.com/account/recover` — Reset password
- `https://yourstore.com/account` — Account home (signed in)
- `https://yourstore.com/account/orders/<id>` — Order detail
- `https://yourstore.com/account/addresses` — Saved addresses

## When customer accounts are enabled

Whether customers can log in at all is controlled in `Shopify admin > Settings > Customer accounts`. Three modes are available:

- **Customer accounts not required** — Customers can check out as guests; signed-in flows are optional.
- **Customer accounts optional** — Customers can create an account or check out as guests.
- **Customer accounts required** — Customers must sign in to check out.

The header's **Account** / **Log in** link is shown when customer accounts are enabled. When disabled, the link is hidden automatically.

## New customer accounts

Shopify also offers a newer **Customer accounts** experience that uses email-based passwordless login and a different account UI hosted by Shopify. If you've enabled this newer flow in your admin, customers are redirected to a Shopify-hosted account page rather than the classic theme-rendered customer pages.

Pave is compatible with both the classic and new customer accounts. Pick the flow that matches your customer expectations and store maturity in `Shopify admin > Settings > Customer accounts`.

## What customers see in their account

- **Order history** — Past orders with status, total, and a link to the order detail.
- **Order detail** — Line items, shipping address, billing address, fulfillment status, tracking link, and a reorder option.
- **Addresses** — Saved shipping addresses for faster checkout.
- **Profile** — Email and password (classic accounts only).

## Tips

- **Test the login flow** end-to-end on a development store: register, log out, log in, view an order, edit an address.
- **Email notifications** — Account-related emails (welcome, password reset, order confirmation) are configured in `Shopify admin > Settings > Notifications`. Customize subject lines and copy from there.
- **Selling plans (subscriptions)** are visible on the order detail page, including the recurring schedule and the ability to manage the subscription if your selling-plan app supports it.

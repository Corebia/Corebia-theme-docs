---
title: Policy page
layout: default
parent: Templates
nav_order: 15
permalink: /templates/policy-page/
---

# Policy page

The **Policy page** template is used for your store's policies: Privacy policy, Terms of service, Refund policy, Shipping policy, and any other policies configured in `Shopify admin > Settings > Policies`.

It uses the `policy.liquid` template (Liquid, not JSON), so it is not customizable from the theme editor section by section. Instead, the rendered look is controlled by **Main policy** section settings. The page content itself is edited in your Shopify admin.

## URL

Each policy has its own URL:

- `https://yourstore.com/policies/privacy-policy`
- `https://yourstore.com/policies/terms-of-service`
- `https://yourstore.com/policies/refund-policy`
- `https://yourstore.com/policies/shipping-policy`

## What the page shows

- The policy title (from your Shopify admin).
- The policy content (rich text from your admin).
- An optional "last updated" date.
- An optional back link / breadcrumb.

## Settings

- **Color scheme** — Default: scheme-1.
- **Show back link and breadcrumb** — Toggle.
- **Show back link (legacy)** — A legacy back-link toggle kept for compatibility.
- **Show divider** — A horizontal divider between the title and the content.
- **Show last updated date** — Toggle.
- **Last updated date** — A free-form field for the date string. Example: `January 2026`.

## Editing the content

1. In your Shopify admin, go to **Settings > Policies**.
2. Edit each policy. Shopify provides templates as a starting point.
3. Save. Changes appear immediately on your storefront.

## Where policy links appear in Pave

Pave automatically renders policy links in two places, based on which policies are configured:

- The **Header** navigation panel (legal footer area).
- The **Footer** section (when added as menu blocks pointing to your policies).

If a policy is not configured, its link is automatically hidden.

## Tips

- **Use the Shopify templates as a starting point** — they cover the common legal requirements but should be reviewed by your own legal counsel for the jurisdictions you sell into.
- **Set a "last updated" date** when you make material changes. Customers who have purchased before may want to know when policies changed.
- **Cookie consent banner** — Pave does not include a cookie banner. Use a Shopify app or `Shopify admin > Settings > Customer privacy` to configure.

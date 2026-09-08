---
title: Policy page
layout: default
parent: Templates
nav_order: 15
permalink: /templates/policy-page/
---

# Policy page

Your store policies — refund, privacy, terms of service, shipping, and any others Shopify supports. Each is written in `Shopify admin > Settings > Policies` and rendered by the **Policy page** section.

The content itself is not editable from the theme. These settings control the frame around it.

## Section settings

- **Color scheme** — Default: scheme-1.

### Content

- **Show back link and breadcrumb** — Default: on.
- **Show home page link** — An additional link back to the home page. Default: off.
- **Show divider** — A rule between the heading and the policy text. Default: on.
- **Show last updated date** — Default: off.
- **Last updated date** — The text to show. For example, `January 2026`.

### Spacing

- **Top padding** / **Bottom padding** — Range: 0 to 300 px in 5 px steps. Default: 80 px each.

## Blocks

- **App block** — Any block offered by an installed app.
- **Custom Liquid** — See [Custom Liquid](../../sections/custom-liquid/).

## The last updated date is typed, not automatic

It is a text field, so it says whatever you write and does not update itself when you edit a policy. That is a deliberate trade: Shopify does not expose a reliable edited-at date for policies, and a date that silently goes stale is worse than none.

If you turn it on, put a reminder somewhere to change it when you change a policy. If you'd rather not maintain it, leave it off — nothing requires it.

## Which policies appear

Only the policies you have actually written. An empty policy has no page and no link, so the footer and header show links only for the ones that exist.

Some markets require specific policies to be published. Shopify offers templates for each under `Settings > Policies`, and they are a starting point rather than legal advice.

## Tips

- **Write the refund policy first.** It is the one shoppers look for before buying, and the one that generates support mail when it is missing.
- **Keep the divider on.** Policy text is long and undifferentiated; the rule gives the eye a start line.
- **Link them from the footer**, which is where shoppers expect them. The header panel already carries them automatically.

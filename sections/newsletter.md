---
title: Newsletter
layout: default
parent: Sections
nav_order: 10
permalink: /sections/newsletter/
---

# Newsletter

**Newsletter** is the in-page email signup. Addresses collected here land in `Shopify admin > Customers`, tagged as accepting marketing, ready for Shopify Email or any marketing app you connect.

It can't be placed in the header group. For the timed overlay version, see [Newsletter popup](../newsletter-popup/).

## Settings

- **Heading** — Default: `Subscribe to the newsletter`.
- **Subheading** — Default: `Sign up to hear about new arrivals and store news.`
- **Social proof text** — Shown below the form. Default: `Join our community`. Leave blank to hide.

### Form

- **Submit style** — **Inline arrow (editorial)** (default) or **Pill button with visible label**. The inline arrow reads as a quiet editorial close; the pill button competes more assertively for attention. Both are accessible and submit identically — pick the mood the section should set in its slot.

### Consent

- **Show consent checkbox** — Default: on. Required for EU markets under GDPR. Without the checkbox, the form records consent when it's submitted.
- **Consent text** — Inline rich text, and it may contain links. Ships pointing at `/policies/privacy-policy`.

### Colors and spacing

- **Color scheme** — Default: scheme-1.
- **Top padding** / **Bottom padding** — Range: 0 to 300 px in 5 px steps. Default: 80 px each.

## Tips

- **Say what the shopper gets.** "Sign up" alone converts poorly. Name the thing — early access, a restock note, one email a month.
- **Leave the consent checkbox on if you sell into the EU.** It is the difference between recorded consent and assumed consent, and it costs one line of layout.
- **Point the consent text at a real policy.** The default link assumes you have a privacy policy published under `Shopify admin > Settings > Policies`. If you haven't, the link 404s.
- **Pick the submit style by neighbourhood.** The inline arrow suits a newsletter sitting between two quiet editorial sections; the pill button suits one placed at the end of a busy page where it has to be found.

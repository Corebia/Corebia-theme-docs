---
title: 404 page
layout: default
parent: Templates
nav_order: 12
permalink: /templates/404-page/
---

# 404 page

The **404 page** is shown when a customer visits a URL that does not exist. It uses the `404.json` template.

## URL

Any URL that does not match a real page on the storefront. Customers do not navigate here intentionally; they arrive via a typo or an outdated link.

## Sections included by default

1. **404 page** — The error message and navigation back, optionally with a featured collection.

## 404 page section

### Content

- **Heading** — The headline shown to the customer. Default: `We can't find that page`.
- **Subtext** — Supporting text. Default: `It looks like the page you were looking for has moved or no longer exists.`
- **Button label** — Call-to-action button text. Default: `Back to home page`.
- **Button link** — The URL the button points to. Defaults to the home page if left empty.

### Featured collection

The 404 page can show a row of products from a chosen collection to keep the customer engaged.

- **Featured collection** — The collection to feature.
- **Number of products** — Range: 0 to 12.
- **Products section heading** — Default: `You might like`.
- **Show product vendor** — Toggle.

### Other

- **Color scheme** — Default: scheme-1.

## Special behaviors

- **Built-in HTTP 404 status** — The 404 template is automatically associated with HTTP 404 responses. Search engines recognize this so unknown URLs are not mistakenly indexed.
- **Search box in the header** — Customers can immediately search from the header even on the 404 page.

## Tips

- **Feature your top sellers** in the featured collection. Most customers landing on a 404 are mistakenly typing a URL or following a stale link; a strong product surface keeps them on the store.
- **Don't be apologetic to the point of being long.** A short heading and one supporting sentence works. Long apologetic copy reads as theatrical.
- **Test the page** by visiting a non-existent URL like `https://yourstore.com/this-doesnt-exist`.

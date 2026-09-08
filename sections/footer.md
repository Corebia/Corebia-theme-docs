---
title: Footer
layout: default
parent: Sections
nav_order: 2
permalink: /sections/footer/
---

# Footer

The **Footer** closes every page. It carries a wordmark, whatever blocks you add, and — when you switch them on — your social and payment icons.

The Footer lives in the `footer` section group, so it can't be removed or placed on an individual template.

## Settings

- **Wordmark** — Shown as a small wordmark at the top of the footer. Falls back to your shop name if empty.
- **Show social media icons** — Default: on. The icons come from the links you fill in under [Social media](../../theme-settings/social-media/); an empty link shows no icon.
- **Show payment icons** — Default: on. The icons are the payment methods actually enabled on your store, so this list is managed by Shopify, not by the theme.
- **Color scheme** — Default: scheme-1.

## Blocks

### Footer navigation

- **Heading** — Default: `Quick links`.
- **Footer menu** — The Shopify navigation to render. Default: `footer`.

### Text

- **Heading** — Default: `About us`.
- **Text** — Rich text. Replace the sample copy before you go live.

### Contact

- **Heading** — Default: `Contact`.
- **Email** — Rendered as a `mailto:` link.
- **Phone** — Rendered as a `tel:` link.
- **Address** — Rich text.

## Country and language selectors

These appear automatically, and have no settings of their own:

- The **country and currency selector** appears once your store sells in more than one country. Set them up in `Shopify admin > Settings > Markets`.
- The **language selector** appears once your store publishes more than one language. Add languages in `Shopify admin > Settings > Languages`.

If you only sell in one country and one language, neither selector renders and the footer closes tighter. That's expected — see [Multi-currency and language](../../features/multi-currency-language/).

## Tips

- **Three or four blocks is the sweet spot.** A footer that runs past that starts to read as a sitemap rather than a close.
- **Use the Contact block for a real address.** Some markets require a business address on the storefront, and a footer block is the conventional place for it.
- **Build the footer menu in Shopify.** The block renders one level; sub-menus in a footer navigation are ignored.

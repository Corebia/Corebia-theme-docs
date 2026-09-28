---
title: Footer
layout: default
parent: Sections
nav_order: 2
permalink: /sections/footer/
---

# Footer

The **Footer** closes every page. It carries a wordmark, the columns you build from blocks, a copyright line and, when you switch them on, your social and payment icons.

The Footer lives in the `footer` section group, so it can't be removed or placed on an individual template. The group ships with a [Newsletter](../newsletter/) section above the footer, which you can remove or replace.

## Settings

- **Wordmark.** Shown as a small wordmark at the top of the footer. Falls back to your shop name if empty.
- **Show social media icons.** Default: on. The icons come from the links you fill in under [Social media](../../theme-settings/social-media/); an empty link shows no icon.
- **Show payment icons.** Default: on. The icons are the payment methods actually enabled on your store, so this list is managed by Shopify, not by the theme.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 65 px top and 30 px bottom. These are the largest values, used on screens 1920 px and wider, and they scale down on smaller screens.

## Blocks

Each block becomes a column. The footer ships with two **Footer navigation** blocks: one headed `Shop` showing `main-menu`, and one showing your `footer` menu.

### Footer navigation

- **Heading.** Default: `Quick links`.
- **Footer menu.** The Shopify menu to render. Default: `footer`. Only the top level is shown; sub-menus are ignored.
- **Collapse into an accordion on mobile.** Folds the column under its heading on screens narrower than 750 px. Default: off, so the column stays open at every width.

A menu with no links renders no column at all.

### Text

- **Heading.** Default: `About us`.
- **Text.** Rich text. Replace the sample copy before you go live.

### Contact

- **Heading.** Default: `Contact`.
- **Email.** Rendered as a `mailto:` link.
- **Phone.** Rendered as a `tel:` link.
- **Address.** Rich text.

### Email signup

A compact newsletter form. Addresses land in `Shopify admin > Customers`, tagged `newsletter` and marked as accepting marketing.

- **Heading.** Default: `Newsletter`.

### Follow on Shop

Shopify's Follow on Shop button, which lets shoppers follow your store in the Shop app. Its colors are Shopify's and can't be changed. If Shopify doesn't render the button for your store, the column is left out.

- **Heading.** Default: `Follow us`.

### Image

An image column, such as a certification mark or a second logo.

- **Heading.** Optional.
- **Image.** The block renders nothing until an image is set. Alt text is read from the image itself, falling back to your shop name.
- **Image width.** Range: 40 to 400 px in 10 px steps. Default: 160 px.
- **Link.** Optional. Makes the image a link.

### Store policies

Links to every policy you have filled in under `Shopify admin > Settings > Policies`. A store with no policies gets no column.

- **Heading.** Default: `Policies`.

## Country and language selectors

These appear automatically at the top of the footer, and have no settings of their own:

- The **country and currency selector** appears once your store sells in more than one country. Set them up in `Shopify admin > Settings > Markets`.
- The **language selector** appears once your store publishes more than one language. Add languages in `Shopify admin > Settings > Languages`.

If you only sell in one country and one language, neither selector renders. That's expected. See [Multi-currency and language](../../features/multi-currency-language/).

## Tips

- **Three or four columns is the sweet spot.** A footer that runs past that starts to read as a sitemap rather than a close.
- **Use the Contact block for a real address.** Some markets require a business address on the storefront, and a footer block is the conventional place for it.
- **Don't collect emails twice in a row.** The footer group already opens with a Newsletter section. If you add an **Email signup** block too, remove one of them.
- **Accordions help long menus on phones.** Turn on **Collapse into an accordion on mobile** for a menu with many links, and leave short ones open so shoppers don't have to tap to see three links.

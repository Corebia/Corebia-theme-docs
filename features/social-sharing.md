---
title: Social sharing
layout: default
parent: Features
nav_order: 16
permalink: /features/social-sharing/
---

# Social sharing

Pave provides a Share button on the product page that uses the browser's native share API on mobile and falls back to a copy-link interaction on desktop. The theme also outputs Open Graph and Twitter Card metadata on every page so that shared URLs render with a preview image and description.

## Where it appears

- **Product page** — When the **Share** block is added to the **Main product** section.

## Share block settings

In the **Share** block on the product page:

- **Show label text** — Toggle whether the word "Share" appears next to the icon.
- **Label** — The label text. Default: `Share`.

## How sharing works

- **Mobile** — Tapping the button opens the device's native share sheet (iOS share sheet, Android share). The customer picks an app (Messages, WhatsApp, Email, etc.) and shares the URL with title and description.
- **Desktop** — Clicking the button copies the URL to the clipboard, with a small confirmation message.

## Open Graph and Twitter Card metadata

Pave outputs the following metadata in the `<head>` of every page:

- **og:title** — The page title.
- **og:description** — The page meta description (or shop description as fallback).
- **og:image** — The page's image (product image, article image, or **Social share image** from theme settings).
- **og:url** — The canonical URL.
- **og:type** — `product` for products, `article` for articles, `website` otherwise.
- **twitter:card** — `summary_large_image`.
- **twitter:title**, **twitter:description**, **twitter:image** — Mirror of the og: tags.

This metadata makes shared URLs render with rich previews on Facebook, X, LinkedIn, WhatsApp, Slack, and most messaging apps.

## Configuring the social share image

The fallback social share image (used on pages without their own image) is set in **Theme settings > Favicon > Social share image**. See [Favicon](../../theme-settings/favicon/).

## Tips

- **Add the Share block.** It's a quick conversion lift on consideration purchases (gifts, fashion, home goods). Customers want to text or email a product to a friend.
- **Verify your share preview.** Use [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) and [X Card Validator](https://cards-dev.twitter.com/validator) to confirm your previews look right and to clear platform caches after image changes.
- **Open Graph image dimensions** — The recommended size is `1200 by 628 px`. Smaller images render small in feeds; larger images cost bandwidth.

## Troubleshooting

- **The Share button doesn't appear** — Confirm the **Share** block is added to the **Main product** section in the theme editor.
- **The share preview shows the wrong image** — Social platforms cache previews. Clear the cache with the platform's debugger tool.
- **The share preview shows no image** — On product pages, the product's first image is used. Confirm the product has at least one image. On generic pages, the **Social share image** in theme settings is the fallback.

## Related

- [Product page > Share block](../../templates/product-page/)
- [Favicon settings](../../theme-settings/favicon/)

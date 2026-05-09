---
title: Favicon
layout: default
parent: Theme settings
nav_order: 5
permalink: /theme-settings/favicon/
---

# Favicon

The **Favicon** category in **Theme settings** controls the small icon that appears in browser tabs and the image that is used when your store is shared on social media.

## Settings

- **Favicon image** — The icon shown in browser tabs and bookmarks. `32 by 32 px .png recommended`.
- **Social share image** — Used as the Open Graph and Twitter image when a page does not have its own. `1200 by 628 px recommended`.

## Where each image is used

### Favicon image

Rendered in the `<link rel="icon">` tag in the page head. Browsers use it for:

- The icon next to the page title in browser tabs.
- The icon next to bookmarks.
- The home screen icon when customers add your site to their phone's home screen.

### Social share image

Rendered as the `og:image` and `twitter:image` meta tag in the page head. Used by:

- Facebook, LinkedIn, X, WhatsApp, Slack, and other social and messaging platforms when your store URL is shared.
- Search engine result snippets that show preview images.

If a specific page (product, article, or page with a featured image) has its own image, that image is used for the share preview. The **Social share image** is the fallback used when a page has no image of its own (for example, the home page or a policy page).

## Recommendations

### Favicon

- **Format:** `.png` with transparency.
- **Size:** `32 by 32 px`. Browsers downscale larger images automatically, but uploading at the target size keeps the image crisp.
- **Design:** A simple mark, monogram, or single letter works best at this size. Detailed logos turn into blurry blobs.

### Social share image

- **Size:** `1200 by 628 px` (1.91:1 ratio). This is the recommended Open Graph size and renders cleanly across Facebook, LinkedIn, and X.
- **Format:** `.jpg` or `.png`. JPEG keeps file size lower for photography; PNG is better for graphics and text.
- **Composition:** Center your important content. Some platforms crop the edges in different ways.
- **Text overlays:** Keep text large and high-contrast. The image is often shown at small sizes (200–300 px wide) in feed previews.

## How to upload

1. Open the theme editor.
2. Click **Theme settings** in the left sidebar.
3. Open the **Favicon** category.
4. Click **Favicon image > Select image** to upload your favicon.
5. Click **Social share image > Select image** to upload the share image.
6. Click **Save**.

## Verifying

- **Favicon:** Open your storefront in a browser. The favicon should appear in the tab. If it doesn't, hard-refresh with `Ctrl+F5` (Windows) or `Cmd+Shift+R` (Mac) to bypass the browser cache.
- **Social share image:** Use a tool like [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) or [X Card Validator](https://cards-dev.twitter.com/validator) to test how your URL renders, and to clear the cache after updating the image.

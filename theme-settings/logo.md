---
title: Logo
layout: default
parent: Theme settings
nav_order: 9
permalink: /theme-settings/logo/
---

# Logo

Your logo, and an optional light version of it for dark backgrounds.

## Settings

- **Logo image.** Shown in sections that display branding. Falls back to the shop name.
- **Logo width.** Shown once a logo is set. Range: 50 to 300 px in 10 px steps. Default: 120 px.
- **Mobile logo width.** Shown once a logo is set. Used below 750 px, independently of the desktop width. Range: 50 to 200 px in 10 px steps. Default: 90 px.
- **Inverse logo.** A light version of the logo, for the transparent header over the home page hero. Leave it empty to keep the header as it is.

## Where the logo appears

- In the [Header](../../sections/header/), when **Show shop branding** is on, which it is by default. On the home page the header normally leaves the branding out, because the hero carries the brand there. Upload an **Inverse logo** and the home page shows it over the hero instead.
- On the [Password page](../../templates/password-page/), when its **Show logo** setting is on.
- In your store's structured data, where search engines read it as your organization's logo.

With no logo uploaded, the header and the password page fall back to the shop name as text.

## Preparing the file

- **Use a transparent PNG or an SVG.** A logo on a white rectangle will show that rectangle against every color scheme that isn't white.
- **Upload it at roughly twice the display width.** At the 120 px default that means about 240 px wide, so it stays sharp on high-density screens.
- **Crop the empty space out of the file.** Padding baked into the image is padding the theme can't remove, and it makes the logo look smaller than the width setting suggests.
- **Set the alt text on the file itself**, in `Shopify admin > Content > Files`. That is what a screen reader announces.
- **Make the inverse logo the same size and crop as the main one.** Only the colors should differ, so the header doesn't shift between the home page and the rest of the store.

## Tips

- **Width is the only control.** Height follows the image's own proportions, so a very wide wordmark and a square mark set to the same width will not look the same size. Adjust by eye, not by number.
- **Set the mobile width separately.** A logo that sits comfortably at 120 px on desktop can crowd the icons in a phone's header. The mobile width exists so you don't have to compromise.
- **Check it against every scheme you use.** A dark logo disappears on a dark color scheme, and the theme can't recolor it for you. The inverse logo only covers the home page hero.
- **A wordmark often beats a logo here.** The header branding is small and sits in a corner; a detailed emblem rarely survives at that size, whereas type does.

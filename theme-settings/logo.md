---
title: Logo
layout: default
parent: Theme settings
nav_order: 4
permalink: /theme-settings/logo/
---

# Logo

## Settings

- **Logo image.** Shown in sections that display branding. Falls back to the shop name.
- **Logo width.** Range: 50 to 300 px in 10 px steps. Default: 120 px.

## Where the logo appears

- In the [Header](../../sections/header/), when **Show shop branding** is on. That setting is off by default, and the home page never shows the header branding, because the hero carries the brand there.
- On the [Password page](../../templates/password-page/), when its **Show logo** setting is on.

With no logo uploaded, both fall back to the shop name as text, styled with the theme's heading font.

## Preparing the file

- **Use a transparent PNG or an SVG.** A logo on a white rectangle will show that rectangle against every color scheme that isn't white.
- **Upload it at roughly twice the display width.** At the 120 px default that means about 240 px wide, so it stays sharp on high-density screens.
- **Crop the empty space out of the file.** Padding baked into the image is padding the theme can't remove, and it makes the logo look smaller than the width setting suggests.
- **Set the alt text on the file itself**, in `Shopify admin > Content > Files`. That is what a screen reader announces.

## Tips

- **Width is the only control.** Height follows the image's own proportions, so a very wide wordmark and a square mark set to the same width will not look the same size. Adjust by eye, not by number.
- **Check it against every scheme you use.** A dark logo disappears on a dark color scheme, and the theme can't swap it for you.
- **A wordmark often beats a logo here.** The header branding is small and sits in a corner; a detailed emblem rarely survives at that size, whereas type does.

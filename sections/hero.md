---
title: Hero banner
layout: default
parent: Sections
nav_order: 10
permalink: /sections/hero/
---

# Hero banner

The **Hero banner** is the full-height opening image at the top of the home page, or of any template that takes sections. It pairs a large photograph, or a looping video, with your brand name, and can add a subheading, up to two buttons, a vertical side rail and a scroll cue.

It can't be placed in the header or footer groups. Three presets are available when you add it: **Hero banner**, **Hero with button** and **Hero with video**.

## Settings

### Image

- **Background image.** The desktop background image.
- **Mobile image (optional).** 4:5 aspect ratio recommended. Falls back to the main image.
- **Background video.** Plays muted and on a loop over the image once the page has loaded, with a pause button. The image stays as the poster, and it is all that visitors who ask for reduced motion see.
- **Image focal point.** Where the desktop image crops. **Top** (default), **Center** or **Bottom**. Used only when the image has no focal point of its own: a focal point set on the image in the image picker takes its place.
- **Mobile image focal point.** **Top** (default), **Center**, **Bottom**, **Left** or **Right**. The same rule applies to the image shown on mobile.
- **Overlay opacity.** Darkens the image so the text stays legible. Range: 0% to 80% in 5% steps. Default: 35%.

**Mobile image (optional)** and the two focal point settings are shown once a background image is set.

### Text

- **Show brand name.** Default: on. Turn it off when the header logo already shows over the hero. On the home page the name stays in place as the page heading for screen readers.
- **Brand name.** The large text over the image. Defaults to the shop name if empty.
- **Subheading.** Optional one-liner below the brand name. For example, `Crafted slowly. Built to last.`
- **Font size scale.** Scales the brand text. Range: 50% to 150% in 5% steps. Default: 100%.
- **Text position.** **Bottom left** (default) or **Bottom center**.
- **Color scheme.** Applied to the text overlay. Default: scheme-1.

### Editorial accents

- **Show side rail.** A vertical metadata strip on the left edge, desktop only. Default: on.
- **Side rail text.** Defaults to the shop name if empty. Shown when the side rail is on.
- **Show scroll indicator.** Default: on.
- **Scroll indicator label.** Default: `Scroll`. Shown when the scroll indicator is on.

### Spacing

- **Top padding.** Range: 0 to 300 px in 5 px steps. Default: 110 px. Applies on mobile only: on desktop the content sits at the bottom of the banner.
- **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 65 px.

Both are the largest values, used on the widest screens, and they scale down on smaller ones.

## Blocks

Up to **two** [Button](../theme-blocks/#button) blocks, shown below the subheading. Give one the **Primary** style and the other **Secondary** so the two don't compete.

## Tips

- **Use a high-resolution image.** The hero spans the full viewport on every screen; anything under about 2400 px wide goes soft on large desktop displays.
- **Always set the image, even with a video.** The image is what shows while the video loads, and it is all that shoppers who reduce motion ever see.
- **Keep the video short and quiet.** It plays muted on a loop, so a slow 10 to 20 second clip without cuts suits it better than an edited film.
- **Plan for the text.** Photographs with quiet space at the bottom, such as sky, floor or a plain wall, carry the brand name best. Busy compositions fight it.
- **Give mobile its own crop.** A wide desktop hero squashes on a phone. A 4:5 portrait version in **Mobile image (optional)** fixes it in one step.
- **Raise the overlay before you shrink the text.** 35% suits most photography; light or busy images usually want 45% to 55%.
- **One hero per page.** Two stacked heroes read as an error rather than an intention.

## When to use

The hero is the visual anchor of the home page. Its job is to say who you are at first glance, not to sell one product. To promote a specific product or collection in the same register, use [Brand image](../brand-image/) or [Rich text with image](../rich-text-image/). To rotate several messages, use [Slideshow](../slideshow/).

## When not to use

If your storefront is catalog-driven rather than brand-driven, open with [Collection list](../collection-list/) or [New arrivals](../new-arrivals/) instead and keep the hero for category landing pages.

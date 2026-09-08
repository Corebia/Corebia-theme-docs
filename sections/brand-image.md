---
title: Brand image
layout: default
parent: Sections
nav_order: 8
permalink: /sections/brand-image/
---

# Brand image

**Brand image** is a full-width image or background video with no text over it. It is the section for letting a photograph breathe between two blocks of content.

It can't be placed in the header or footer groups.

## Settings

### Image

- **Image** — Used on desktop, and on mobile when no mobile image is set. Alt text is read from the image asset itself — set it in the file editor, for screen readers and for SEO.
- **Mobile image** — Optional. Shown on screens narrower than 750 px. Leave empty to use the same image with the mobile focal point below.
- **Desktop focal point** — Where the image crops on screens 750 px and wider. **Top**, **Center** (default) or **Bottom**.
- **Mobile focal point** — Where the image crops on narrower screens when no mobile image is set. **Top**, **Center** (default), **Bottom**, **Left** or **Right**.
- **Proportion** — **Cinematic (panoramic)**, **Balanced (default)** or **Portrait (taller)**.
- **Prioritize loading** — Use when this section is the first thing on its template. Turns off the fade-in reveal so the image appears sooner. Default: off.

### Video (optional)

- **Video** — When set, replaces the image with an autoplay, muted, looping background video. The image above stays as the poster and as the accessibility fallback. Respects `prefers-reduced-motion` and Data Saver.
- **Mobile video** — Optional. Shown on screens narrower than 750 px. Leave empty to use the desktop video.

### Colors

- **Color scheme** — Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding** — Range: 0 to 300 px in 5 px steps. Default: 0 px each, so the image meets the sections above and below edge to edge.

## Tips

- **Turn on Prioritize loading only for the topmost section.** It exists to get the first image on screen sooner. Used further down the page it just removes an animation for no gain.
- **Always set the poster image, even when using video.** It is what shows before the video loads, what shoppers on Data Saver see, and what a screen reader reads.
- **No text means the photograph carries everything.** If the image needs a caption to make sense, you want [Rich text with image](../rich-text-image/) instead.
- **Focal points beat re-cropping.** Set them here rather than uploading two crops of the same photograph.

## When not to use

Don't use it as a second hero at the top of the home page — that is what [Hero banner](../hero/) is for, and it handles the brand name, the overlay and the scroll cue that a top-of-page image needs.

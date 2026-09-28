---
title: Slideshow
layout: default
parent: Sections
nav_order: 11
permalink: /sections/slideshow/
---

# Slideshow

**Slideshow** shows up to eight full-bleed slides, each an image with its own heading, text and button laid over it. Shoppers move between slides with the arrows, the dots or a swipe; the slides only change on their own if you turn that on.

It can't be placed in the header or footer groups. Two presets are available when you add it: **Slideshow**, full width and full screen, and **Slideshow inset**, page width and large, with 40 px of padding above and below.

## Settings

- **Width.** **Full width** (default) runs edge to edge; **Page width** keeps the slides inside the page margins.
- **Slide height.** **Full screen** (default), **Large** or **Medium**. Full screen fills the window below the announcement bar.
- **Change slides automatically.** Default: off. When on, a pause button appears on the slideshow, and rotation stops while the pointer rests on it and for good once keyboard focus enters it. It never runs for shoppers who ask their device for reduced motion.
- **Time per slide.** Shown when automatic change is on. Range: 3 to 10 s in 1 s steps. Default: 5 s.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 0 px each.

## Blocks

Up to **eight** Slide blocks. A slideshow with no slides shows nothing on the storefront; with one slide there are no arrows or dots.

### Slide

- **Image.** The slide's image. Without one, a full-color placeholder scene fills the slide under a fixed darkening veil, so the text stays readable while you set the slide up.
- **Mobile image.** Shown on screens narrower than 750 px. Leave it blank to use the image.
- **Content position.** Where the heading, text and button sit on the slide. **Bottom left** (default), **Bottom center**, **Center** or **Top left**.
- **Overlay opacity.** Darkens the whole slide evenly so the text stays readable. It applies once the slide has an image. Range: 0% to 80% in 5% steps. Default: 30%.

Each slide takes [Heading](../theme-blocks/#heading), [Text](../theme-blocks/#text) and [Button](../theme-blocks/#button) blocks, in any order. A new slide starts with one of each.

## Tips

- **Put the most important slide first.** Many shoppers never press the arrow, and with automatic change off the first slide is the only one they see.
- **Three slides is plenty.** Past that, the later slides are rarely reached.
- **Give each slide a mobile image.** A landscape photo cropped to a phone screen loses its subject; a portrait version in **Mobile image** avoids that.
- **Leave automatic change off unless the slides tell one story.** Moving content competes with the text on it, and shoppers who are still reading lose their place.

## When to use

A slideshow suits a home page that has more than one thing to announce at once, such as a new season and a sale. For a single message, [Hero banner](../hero/) or [Media with content](../media-with-content/) says it without hiding anything behind an arrow.

---
title: Rich text with image
layout: default
parent: Sections
nav_order: 15
permalink: /sections/rich-text-image/
---

# Rich text with image

**Rich text with image** lays text over a background image. Unlike [Brand message](../brand-message/), where the text sits beside the picture, here it sits on top of it, so the image is chosen for what it can carry rather than for what it shows.

On a phone (below 750px) the section stacks instead: the image shows at its aspect ratio with no overlay, and the heading, text and button follow it underneath in the section's color scheme.

It can't be placed in the header or footer groups.

## Settings

### Image

- **Image.** The background image.
- **Image aspect ratio.** **Ultra-wide (21:9)**, **Wide (16:9)** (default), **Standard (4:3)**, **Square (1:1)** or **Portrait (3:4)**. From 750px the ratio is a minimum: when the text needs more room, the section grows taller and the image is cropped, so the text is never cut off. On a phone the ratio is the image's own shape, above the text.
- **Overlay darkness.** Higher values darken the image so the text stays legible. It applies from 750px; on a phone the text sits below the image, so there is no overlay. Range: 0% to 80% in 5% steps. Default: 35%. Set to 0 to remove the overlay.

### Colors

- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 80 px each.

## Blocks

Up to **six** blocks in total, in any mix of these theme blocks:

- [Heading](../theme-blocks/#heading). Ships with `Our story`.
- [Text](../theme-blocks/#text). Ships with sample copy; replace it before you go live, because it is shown to customers on the storefront.
- [Button](../theme-blocks/#button). **Primary** or **Secondary** style.

The section is added with one of each.

## Tips

- **Order the blocks the way they should read.** The stack is rendered top to bottom in the order you arrange it, so a heading placed after a paragraph will appear after it.
- **Raise the overlay until the text is comfortable, then stop.** Anything past about 60% stops being a photograph and becomes a colored panel.
- **Choose the ratio for the amount of text.** Ultra-wide holds a heading and one line. Portrait holds a heading, a paragraph and a button without crowding.
- **One button is usually enough.** You can add more, but a section with two competing calls to action converts worse than one with a single clear one. If you do add a second, give it the **Secondary** style.

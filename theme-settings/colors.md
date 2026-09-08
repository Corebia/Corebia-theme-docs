---
title: Colors
layout: default
parent: Theme settings
nav_order: 1
permalink: /theme-settings/colors/
---

# Colors

Pave uses Shopify's **color schemes**. A scheme is a complete named palette; every section then chooses which scheme it uses, through its own **Color scheme** setting. Change a color once here and it updates everywhere that scheme is in use.

The theme ships with two schemes. You can add more, rename them and delete them from the theme editor.

## Settings in a scheme

### Backgrounds

- **Background.** The page background. Default: `#FAFAF7`.
- **Background gradient.** An optional gradient that replaces the flat background.
- **Surface.** The second surface tier, used for cards and panels sitting on the background. Default: `#F4F2EE`.
- **Surface elevated.** Third surface tier, for hover states and large dividers. Default: `#EDEAE3`.

### Text

- **Text dark.** The primary text color. Default: `#1A1815`.
- **Text soft.** Secondary text: captions, supporting copy. Default: `#6B655E`.
- **Text muted.** Metadata, microcopy, low-emphasis labels. Default: `#9C968D`.
- **Text light.** Text placed on dark surfaces and over images. Default: `#FAFAF7`.

### Interactive

- **Accent.** The theme's accent color, used for highlights and active states. Default: `#7A8F75`.
- **Button fill.** Primary button background. Default: `#1A1815`.
- **Button text.** Primary button label. Default: `#FAFAF7`.
- **Outline button text.** The label on secondary, outlined buttons. Default: `#1A1815`.

### Feedback states

- **Success.** Confirmations, in-stock messages. Default: `#5A7855`.
- **Warning.** Low stock and cautions. Default: `#A66016`.
- **Danger.** Errors, sold out, destructive actions. Default: `#8A2F2F`.

## Contrast is your responsibility

The defaults are chosen to clear the WCAG AA contrast ratio of 4.5:1 for body text. Once you change them, that is no longer guaranteed.

The pairs that matter most:

| Foreground | Background | Needs |
|---|---|---|
| Text dark | Background | 4.5:1 |
| Text dark | Surface | 4.5:1 |
| Text soft | Background | 4.5:1 |
| Text light | any image overlay | 4.5:1 |
| Button text | Button fill | 4.5:1 |

Any contrast checker will tell you the ratio between two hex values. It is worth a minute per pair: low-contrast text is the most common accessibility failure on a storefront, and it costs sales before it costs anything else.

## Tips

- **Two schemes are usually enough.** One light, one dark, alternated down the page, gives rhythm without turning the storefront into a swatch book.
- **Set the schemes before you build pages.** Section colors reference schemes by name, so adding a third scheme later means revisiting every section that should use it.
- **Text muted is easy to overdo.** It is designed for metadata such as a date or a SKU. Body copy set in it will fail contrast.
- **Change Surface, not Background, when a section needs separating.** That is what the surface tiers are for, and it keeps the page background consistent.

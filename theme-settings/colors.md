---
title: Colors
layout: default
parent: Theme settings
nav_order: 1
permalink: /theme-settings/colors/
---

# Colors

Pave uses Shopify's **color schemes**. A scheme is a complete named palette; every section then chooses which scheme it uses, through its own **Color scheme** setting. Change a color once here and it updates everywhere that scheme is in use.

The theme ships with three schemes:

| Scheme | What it is |
|---|---|
| scheme-1 | The light scheme the whole storefront uses by default. |
| scheme-2 | A dark scheme, for sections you want to set apart. |
| scheme-3 | A second dark scheme, tuned for dark mode. It is the default **Dark mode color scheme**. |

You can add more, rename them and delete them from the theme editor.

## Settings in a scheme

### Backgrounds

- **Background.** The page and section fill. Default: `#FAFAF7`.
- **Background gradient.** An optional gradient that replaces the flat background.
- **Surface.** Sits behind card surfaces such as the product card media and the collection list cards. Default: `#F4F2EE`.
- **Surface elevated.** Third surface tier, for hover states and large dividers. Default: `#EDEAE3`.

### Text

- **Text dark.** The primary text color. Default: `#1A1815`.
- **Text soft.** Secondary text, for captions and supporting copy. Default: `#6B655E`.
- **Text muted.** Metadata, microcopy, low-emphasis labels. Default: `#9C968D`.
- **Text light.** Text placed on dark surfaces and over images. Default: `#FAFAF7`.

### Interactive

- **Accent.** The theme's accent color, used for highlights and active states. Default: `#7A8F75`.
- **Button fill.** Primary button background. Default: `#1A1815`.
- **Button text.** Primary button label. Default: `#FAFAF7`.
- **Outline button text.** The label on secondary, outlined buttons. Default: `#1A1815`.

### Feedback states

- **Success.** Confirmation text and fills, such as the cart savings amount and the added-to-cart button. Default: `#5A7855`.
- **Warning.** The low-stock notice on the product page. Default: `#A66016`.
- **Danger.** Errors and destructive actions. Default: `#8A2F2F`.

### Form fields

- **Field background.** Sits behind the value typed into a field. Default: `#FAFAF7`.
- **Field text.** The value typed into a field. Default: `#1A1815`.
- **Field border.** The outline of text fields, selects and text areas. Default: `#6B655E`.

The thickness and corner radius of fields are set under [Input fields](../input-fields/).

## Dark mode

Below the schemes, two settings let the storefront follow a visitor's device.

- **Follow the visitor's dark mode.** Default: off. When the visitor's device is in dark mode, the page and every section on the first color scheme use the dark mode scheme instead.
- **Dark mode color scheme.** Shown when the setting above is on. Default: scheme-3.

Only the first scheme in your list switches. A section you have deliberately set to another scheme, such as a dark band on scheme-2, keeps its colors in both modes, so the contrast you designed between sections survives. If you pick the first scheme itself as the dark mode scheme, nothing changes.

## Contrast is your responsibility

The defaults are chosen to clear the WCAG AA contrast ratio of 4.5:1 for body text. Once you change them, that is no longer guaranteed. The help text under each color in the editor names the ratio it needs.

The pairs that matter most:

| Foreground | Background | Needs |
|---|---|---|
| Text dark | Background | 4.5:1 |
| Text dark | Surface | 4.5:1 |
| Text soft | Background | 4.5:1 |
| Text muted | Background | 4.5:1 |
| Text light | Any image overlay or dark surface | 4.5:1 |
| Button text | Button fill | 4.5:1 |
| Field text | Field background | 4.5:1 |
| Field border | Background | 3:1 |

Text larger than 18 pt, borders and icons need 3:1 rather than 4.5:1. Any contrast checker will tell you the ratio between two hex values. It is worth a minute per pair: low-contrast text is the most common accessibility failure on a storefront, and it costs sales before it costs anything else.

If you turn on dark mode, check the dark mode scheme's pairs too. It is a whole second set of colors that visitors will read.

## Tips

- **Two or three schemes are usually enough.** One light, one dark, alternated down the page, gives rhythm without turning the storefront into a swatch book.
- **Set the schemes before you build pages.** Section colors reference schemes by name, so adding a scheme later means revisiting every section that should use it.
- **Text muted is easy to overdo.** It is designed for metadata such as a date or a SKU. Body copy set in it strains the eye even when it passes.
- **Change Surface, not Background, when a section needs separating.** That is what the surface tiers are for, and it keeps the page background consistent.
- **Preview dark mode before you turn it on.** Switch your own device to dark mode and walk the home page, a product and the cart. Images with white backgrounds stand out much more against a dark page.

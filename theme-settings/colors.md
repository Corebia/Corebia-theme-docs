---
title: Colors
layout: default
parent: Theme settings
nav_order: 1
permalink: /theme-settings/colors/
---

# Colors

The **Colors** category in **Theme settings** controls every color used across the storefront. Pave organizes colors into reusable **color schemes**, so the same scheme can be applied to multiple sections, and editing a scheme updates every section that uses it.

## How color schemes work

A color scheme is a named bundle of colors (for example, "scheme-1", "scheme-2", "scheme-3"). Pave ships with three schemes by default:

- **scheme-1** — Light background, dark text. The default scheme.
- **scheme-2** — Surface background (cream), dark text.
- **scheme-3** — Dark background, light text.

In every section that has a **Color scheme** setting, you pick which scheme that section should use. Editing a scheme in **Theme settings** propagates the change everywhere it is used.

To add a new scheme, click **Add color scheme** at the top of the Colors panel. To duplicate, edit, or delete a scheme, click the scheme name.

## Settings inside each color scheme

When you open a color scheme, you'll see the following settings, grouped under three headers.

### Backgrounds

- **Background** — The base background color of the scheme. Default: `#FFFFFF` (white).
- **Background gradient** — Optional gradient layered on top of the background color. When set, takes priority over the solid background. Leave empty to use the solid background.
- **Surface** — The secondary background color used for cards, dropdowns, and surfaces that need to stand out from the main background. Default: `#F5F5F0` (warm off-white).

### Text

- **Text dark** — The primary text color, used for body copy and headings. Default: `#1A1A1A`.
- **Text light** — The text color used on top of dark or image backgrounds (for example, the hero banner brand name). Default: `#FFFFFF`.

### Interactive

- **Accent** — Used for links and inline highlights. Default: `#A66016` (warm bronze).
- **Button fill** — The background color of primary buttons. Default: `#1A1A1A`.
- **Button text** — The label color on primary buttons. Default: `#FFFFFF`.
- **Outline button text** — The label color on secondary (outline) buttons. Default: `#1A1A1A`.

## Recommendations

- Keep the **Text dark** color at high contrast against **Background** for accessibility. Aim for a contrast ratio of at least 4.5:1 against body text.
- Use **Accent** sparingly. It is meant for emphasis, not as a primary surface color.
- Pick **Outline button text** so it works against both **Background** and **Surface** — outline buttons appear on either depending on context.
- When adding a custom scheme, copy an existing one as a starting point and tweak only the colors that need to change.

## Where color schemes are used

Every Pave section that displays colored content has a **Color scheme** setting that points to one of these schemes. Examples:

- Header — sets the side navigation panel scheme.
- Footer — sets the footer scheme.
- Announcement bar — sets the bar's scheme.
- Hero banner, Brand message, New arrivals, and most other home page sections.
- Main product, Main collection, Main cart, and other template-level sections.

If you want a section to look different, change its **Color scheme** setting; you should rarely need to override individual colors.

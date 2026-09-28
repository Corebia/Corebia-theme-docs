---
title: Collection list
layout: default
parent: Sections
nav_order: 21
permalink: /sections/collection-list/
---

# Collection list

**Collection list** shows up to five collections as image tiles, either as an editorial mosaic or as a uniform grid. Each tile uses the collection's own image and title.

Every tile shows its collection's name, description and a button over a gradient at the foot of the image, at rest and on every device. On a mouse, hovering a tile zooms its image and dims the others. A tile narrower than 320 px, such as a half-width tile on a phone, shows the name alone, since the whole tile is the link.

It can't be placed in the header or footer groups. It is added with five Collection blocks, ready to fill.

## Settings

- **Heading.** Default: `Collections`.
- **Layout.** **Editorial mosaic** (default) arranges the collections in tiles of different sizes for a magazine feel; tiles side by side share their rows, so no empty space opens beside a tile. **Uniform grid** gives every collection the same size, with its own column and image ratio settings.
- **Image ratio.** **Portrait (4:5)** (default), **Square (1:1)** or **Landscape (3:2)**. Shown when **Layout** is set to Uniform grid; the mosaic sizes its own tiles.
- **Number of columns on desktop.** Range: 2 to 4. Default: 3. Shown when **Layout** is set to Uniform grid.
- **Color scheme.** Default: scheme-1.
- **Image overlay intensity.** **Soft**, **Medium** (default) or **Strong**. Sets the strength of the gradient behind each tile's name and description, so they stay readable on bright or busy imagery.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 80 px each.

## Blocks

Up to **five** Collection blocks.

- **Collections.** The collection this tile points to.
- **Image crop focal point.** Where to anchor the image when it's cropped for this tile. **Auto** (default) uses the image's own focal point from Shopify admin; **Top left**, **Top**, **Top right**, **Left**, **Center**, **Right**, **Bottom left**, **Bottom** and **Bottom right** pin it to that point instead.

## Tips

- **Set the collection image in Shopify.** The tile takes its picture from the collection itself, under `Shopify admin > Products > Collections`. A collection with no image falls back to its first product, which is rarely the crop you want.
- **Use Auto focal point first.** Setting the focal point on the image in your Files area fixes the crop everywhere at once. Only override it here when one tile needs a different crop from the same image.
- **Raise the overlay for bright photography.** Soft looks better on dark images; light or high-key imagery usually needs Medium or Strong for the title to hold.
- **Three or four tiles is the comfortable range.** Five is the maximum and it does fill a wide screen, but the row stops looking like a selection and starts looking like a menu.

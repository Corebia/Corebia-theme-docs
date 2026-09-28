---
title: Lookbook collection page
layout: default
parent: Templates
nav_order: 6
permalink: /templates/lookbook-collection/
---

# Lookbook collection page

The **lookbook** collection template, `collection.lookbook.json`, presents a collection as a campaign rather than a catalog: a tall hero, a grid of cards in varied sizes, and two promotional tiles set between the products.

It uses the same **Main collection** section as the standard [Collection page](../collection-page/), so every setting is documented there. What makes it a lookbook is how those settings are preset.

## What it ships with

| Setting | Lookbook | Standard collection |
|---|---|---|
| Hero height | Large (65% of screen height) | Medium (50% of screen height) |
| Image focal point | Use the image's focal point | Center |
| Text position | Bottom left | Bottom center |
| Hero overlay darkness | 30% | 35% |
| Description position | Below the grid | Above the grid |
| Filter layout | Horizontal bar above the grid | Sidebar |
| Grid style | Lookbook spread | Uniform grid |

The **Lookbook spread** grid keeps the normal product cards but varies their proportions and widths on a repeating six-cell pattern, so the page reads like a magazine spread rather than a shelf.

Two of the three **Promotional tile** slots come filled in:

- At position 4, two columns wide: the heading `The edit`, a line of copy and a `Shop the edit` link.
- At position 9, one column wide: the heading `Fabric notes`, a line of copy and an `About our materials` link.

Both links point at `/collections/all` and neither tile has an image. Replace the copy and links with your own, add an image, or clear a tile to remove it. The third slot is empty. How the tiles work is covered under [Promotional tile](../collection-page/#promotional-tile).

## Using it

1. In Shopify admin, open **Products > Collections** and choose the collection.
2. Under **Theme template**, choose **lookbook** and save.
3. In the theme editor, pick **Collections > lookbook** from the template menu at the top to adjust it. Changes apply to every collection assigned to this template.

## Tips

- **Pick collections with strong photography.** The varied card sizes enlarge some product images well beyond a normal grid cell, so soft or inconsistent shots show.
- **Keep it to a curated set.** A lookbook of 200 products loses the point. It suits a season, a capsule or a collaboration of a few dozen pieces.
- **Write the description as the story.** It sits below the grid here, where it reads as a closing note to the campaign rather than an introduction to scan past.
- **Give the tiles real destinations.** A tile that links to the same collection the shopper is already on wastes a cell. Point it at a journal article, a related collection or a page about materials.

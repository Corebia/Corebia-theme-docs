---
title: Product media
layout: default
parent: Features
nav_order: 4
permalink: /features/product-media/
---

# Product media

Pave's product page supports rich media: images, videos, 3D models, and external video embeds (YouTube, Vimeo). Customers see a configurable gallery that can open any image full screen.

## Supported media types

- **Images.** JPG, PNG, WebP. The primary image type for product photography.
- **Videos.** MP4 video files uploaded directly to Shopify.
- **External videos.** YouTube and Vimeo embeds via the product's media URL field.
- **3D models.** GLB / USDZ files uploaded to the product. They render with the model-viewer web component, supporting orbit, zoom, and AR view on mobile.

## How to upload media

1. In `Shopify admin > Products > [product]`, scroll to **Media**.
2. Drag and drop files, or click **Add media** and pick from your library.
3. To embed an external video, click **Add media > Add embed URL** and paste the YouTube or Vimeo URL.
4. To upload a 3D model, drag the `.glb` or `.usdz` file into the same area.
5. Save.

## Gallery settings

The gallery is configured in the **Main product** section. See the [Product page reference](../../templates/product-page/) for every setting; the ones that shape the gallery are:

- **Desktop gallery layout.** **Stacked**, **2 columns**, **Thumbnails** (the default) or **Thumbnail slideshow**.
- **Mobile layout.** **Show thumbnails**, **Hide thumbnails** or **2 columns**. Offered with the two thumbnail layouts.
- **Extend media to screen edge.** Lets the media column run to the edge of the screen instead of stopping at the page margin. On by default.
- **Enable image zoom.** Clicking an image opens it full screen, where it can be magnified. On by default.
- **Hide other variant media after one is selected.** See below. Off by default.
- **Use video looping.** Makes uploaded videos loop. Off by default. External videos follow the provider's own behavior.

## Variant images

When a customer picks a variant that has its own image, the gallery jumps to that image. The variant image is set in `Shopify admin > Products > [product] > Variants > [variant]`.

To set up:

1. In the product editor, open a variant.
2. Click the image placeholder and pick the image that represents this variant.
3. Repeat for each variant.
4. Save.

With **Hide other variant media after one is selected** on, the gallery goes further and shows only the selected variant's images. Pick "Sand" and the other colors' photos step aside. Videos, 3D models and images not attached to any variant always stay visible, and if a variant has no images of its own, nothing is hidden. The filter applies from the first page load, for the variant the customer arrives on.

The variant image also drives the [color swatch](../swatches/) image for color variants.

## Image focal points

Pave respects the focal point set on an image, either in `Shopify admin > Content > Files` or in the theme editor's image picker. It decides how the image is cropped on cards and in sections that crop, such as the hero banner and the collection hero.

Sections that crop images also have their own **Image focal point** setting, with a separate one for mobile where offered. It is used only when the image has no focal point of its own; a focal point on the image takes priority.

## Video on product cards

Under [Product cards](../../theme-settings/product-cards/), **Play a product video on card hover** plays a product's first video, muted and looping, when a mouse rests on its card. Nothing downloads until then, and touch devices and shoppers who have asked for reduced motion see a still frame. Off by default.

## 3D models and AR

3D models render with the model-viewer web component:

- **Orbit and zoom.** Customers can rotate and zoom into the model on desktop and mobile.
- **AR.** On iOS Safari and Android Chrome, the model can be viewed in the customer's environment via AR Quick Look (iOS) or Scene Viewer (Android), provided the GLB/USDZ files are correctly formatted.

## Tips

- **Image size.** Upload at least 2000 px wide for product photography. Pave generates responsive sizes automatically; images uploaded too small look blurry on high-resolution screens and in the zoom view.
- **One video per product is usually enough.** Videos are heavy. Use them where they genuinely help the customer: movement, fit, transformation.
- **Attach images to color variants.** If you have color variants, give each color its own images, even if the only difference is the color. Swatches and the variant media filter both depend on it.
- **3D models are optional but powerful.** They take time to produce but help sell furniture, jewelry and other high-consideration products.

## Troubleshooting

- **My video doesn't play.** Confirm the file is MP4 and under Shopify's upload size limit. For external videos, confirm the YouTube or Vimeo URL is public and embeddable.
- **Variant image doesn't switch.** Confirm the variant has an image set in the variant editor, not just in the product-level media.
- **Another color's photos still show.** Turn on **Hide other variant media after one is selected**, and check each photo is attached to its variant.
- **3D model loads slowly.** GLB files can be large. Reduce file size with a tool like [glTF-Transform](https://gltf-transform.donmccurdy.com/) before uploading.

## Related

- [Product page template reference](../../templates/product-page/)
- [Swatches](../swatches/)

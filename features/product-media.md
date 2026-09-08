---
title: Product media
layout: default
parent: Features
nav_order: 4
permalink: /features/product-media/
---

# Product media

Pave's product page supports rich media: images, videos, 3D models, and external video embeds (YouTube, Vimeo). Customers see a configurable gallery with multiple layout options.

## Supported media types

- **Images.** JPG, PNG, WebP. The primary image type for product photography.
- **Videos.** MP4 video files uploaded directly to Shopify.
- **External videos.** YouTube and Vimeo embeds via the product's media URL field.
- **3D models.** GLB / USDZ files uploaded to the product. Render with the model-viewer web component, supporting orbit, zoom, and AR view on mobile.

## How to upload media

1. In `Shopify admin > Products > [product]`, scroll to **Media**.
2. Drag and drop files, or click **Add media** and pick from your library.
3. To embed an external video, click **Add media > Add embed URL** and paste the YouTube or Vimeo URL.
4. To upload a 3D model, drag the `.glb` or `.usdz` file into the same area.
5. Save.

## Gallery layouts

The product page gallery has multiple layouts, configured in the **Main product** section settings:

- **Stacked.** Media items stack vertically on desktop.
- **2 columns.** A two-column grid.
- **Thumbnails.** A main image with a column of thumbnails alongside. This is the default.
- **Thumbnail slideshow.** A main image with a scrolling thumbnail strip.

Mobile has its own setting: **Show thumbnails**, **Hide thumbnails**, or **2 columns**.

See the [Product page reference](../../templates/product-page/) for details.

## Variant images

When a customer picks a variant that has its own image, the gallery jumps to that image. The variant image is determined by the **Variant image** field in `Shopify admin > Products > [product] > Variants > [variant]`.

To set up:

1. In the product editor, expand a variant.
2. Click on the **Image** field and pick the image that represents this variant.
3. Repeat for each variant. Variants without an explicit image fall back to the product's first image.
4. Save.

The variant image also drives the [color swatch](../swatches/) image for color variants.

## Image focal points

Pave respects the focal point set on each image in `Shopify admin > Files`. Click an image, then click **Edit** and pick the focal point. This determines how the image is cropped on cards and hero placements.

For section-level images (hero banner, brand image, collection hero), the section settings include their own **Image focal point** for desktop and a separate one for mobile.

## Video looping

The **Main product** section setting **Enable video looping** (default: on) makes uploaded videos auto-loop. External videos (YouTube, Vimeo) follow the embed provider's default behavior.

## 3D models and AR

3D models render with the model-viewer web component:

- **Orbit and zoom.** Customers can rotate and zoom into the model on desktop and mobile.
- **AR.** On iOS Safari and Android Chrome, the model can be viewed in the customer's environment via AR Quick Look (iOS) or Scene Viewer (Android), provided the GLB/USDZ files are correctly formatted.

## Tips

- **Image size.** Upload at least 2000 px wide for product photography. Pave generates responsive sizes automatically; uploading too small produces blurry images on high-resolution screens.
- **One video per product, max.** Videos slow down page load. Use them where they materially help the customer (movement, fit, transformation).
- **Variant images for color.** If you have color variants, upload one image per color, even if the only difference is color. This makes the swatch experience work correctly.
- **3D models are optional but powerful.** They take time to produce but lift conversion for furniture, jewelry, and high-consideration products.

## Troubleshooting

- **My video doesn't play.** Confirm the file is MP4 and under Shopify's upload size limit (1 GB). For external videos, confirm the YouTube/Vimeo URL is public and embeddable.
- **Variant image doesn't switch.** Confirm the variant has an image set in the variant editor (not just the product-level images).
- **3D model loads slowly.** GLB files can be large. Reduce file size with a tool like [glTF-Transform](https://gltf-transform.donmccurdy.com/) before uploading.

## Related

- [Product page template reference](../../templates/product-page/)
- [Swatches](../swatches/)

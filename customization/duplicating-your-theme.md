---
title: Duplicate your theme
layout: default
parent: Customization
nav_order: 1
permalink: /customization/duplicating-your-theme/
---

# Duplicate your theme

{: .warning }
> **Always duplicate your theme before making any code edits.** Working directly on the published theme can break the storefront for live customers. A duplicate is a safe sandbox where you can experiment and roll back at no cost.

## Why duplicate

- **Recovery.** If a code change goes wrong, you still have a clean copy to publish from.
- **Testing.** You can preview a duplicate without affecting customers.
- **Versioning.** Save snapshots before major changes by duplicating, naming the duplicate (for example, "Pave – before holiday rebrand"), and keeping it in your library.
- **Updates.** When a new version of Pave is released, you install the new version on a duplicate, port your customizations, and only then publish. See [Updating to a new version](#updating-to-a-new-version).

## How to duplicate

1. In your Shopify admin, go to **Online Store > Themes**.
2. Find Pave in the **Theme library** (or in the published theme slot).
3. Click the **...** menu next to the theme name.
4. Choose **Duplicate**.
5. Wait for the duplicate to appear in the library. By default, Shopify names it "Copy of [theme name]". Click the **...** menu and choose **Rename** to give it a meaningful name (for example, "Pave – staging").

The duplicate is fully independent: changes to one do not affect the other. Theme settings, sections, blocks, and code are all copied.

## Updating to a new version

When Pave releases a new version:

1. From the Theme Store, click **Update** to install the new version. It appears in your library as a fresh, default copy.
2. Open the new version in the editor and reapply your custom theme settings (colors, fonts, social media URLs, etc.) by referencing your current published theme.
3. If you've made code customizations, port them carefully to the new version, because the underlying files may have changed.
4. Test the new version by previewing it.
5. Publish the new version when ready.

This process keeps you on the latest theme without risking your live storefront.

## Related

- [Custom code](../custom-code/): What is and isn't covered when you do edit theme code.
- [Shopify Help: Duplicate a theme](https://help.shopify.com/manual/online-store/themes/managing-themes#duplicate-a-theme)

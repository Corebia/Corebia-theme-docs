---
title: Custom code
layout: default
parent: Customization
nav_order: 2
permalink: /customization/custom-code/
---

# Custom code

{: .warning }
> **Custom code is not covered by our support policy.** When you modify theme code (Liquid, JavaScript, CSS, or section schemas), you take full responsibility for the result. Our team cannot debug, fix, or maintain code we did not write. See [Support policy](../../support/support-policy/).

## What counts as custom code

Anything that involves editing the theme's source files: editing `.liquid`, `.css`, `.js`, or `.json` files in the theme code editor; pasting Liquid into a [Custom Liquid section](../../sections/custom-liquid/) or block; modifying section schemas; or adding code via apps that inject scripts into the storefront.

The following are *not* custom code and **are** covered by support:

- Configuring sections and blocks in the theme editor.
- Changing theme settings.
- Editing the rich text content of pages, products, and articles in your Shopify admin.
- Adding navigation menus.

## Recommended approach: hire a Shopify Partner

If you need a feature, design change, or integration that isn't built into Pave, the safest path is to hire a verified Shopify Partner.

Visit the [Shopify Partner Directory](https://www.shopify.com/partners/directory) and filter by the kind of work you need. Partners can:

- Add new sections or blocks.
- Modify existing layouts.
- Build custom integrations with apps and external systems.
- Adapt Pave to specific brand requirements.

When you brief a partner, give them:

- A copy of your store's URL (and a staff account if needed).
- A description of the goal, not the implementation.
- Any examples or references that show the desired outcome.

## If you do edit code yourself

### 1. Always duplicate first

See [Duplicate your theme](../duplicating-your-theme/). Work only on the duplicate. Publish only after testing.

### 2. Document what you change

Keep a list of every customization (which file, what was changed, why). This is essential for theme updates: when a new version of Pave is released, you'll need to port these changes.

### 3. Test on multiple devices and browsers

Test on desktop and mobile, on Chrome, Safari, Firefox, and Edge. Pave is tested across these browsers; your customizations should be too.

### 4. Test in the theme editor

Most theme customizations work fine in the storefront but break in the theme editor's preview. Open your customized theme in the editor and verify everything still renders correctly.

## What happens on theme update

When Pave releases a new version, the update is shipped as a fresh, default copy of the theme. **Customizations on your current theme are not carried over to the new version.** You must port your customizations manually if you want to keep them.

This is one reason hiring a partner is recommended: a partner can document and re-apply your customizations on each update, and can help you decide whether a new version's improvements are worth the porting effort.

## Custom translations

Editing the locale file (translations) is also a code-level customization. To translate Pave's default content into other languages or to override default English copy, use **Translate & Adapt** (Shopify's free translation app) or a paid tool like Langify or Weglot. These apps overlay translations without modifying the locale file.

If you do edit the locale file directly, the changes count as custom code and are not covered by support.

## Tutorials

Pave does not bundle "how to make this change" tutorials. The reasoning: every tutorial that survives in the docs becomes implicit support — customers expect us to maintain the recipe and fix it when it breaks. We choose to keep the boundary clear: built-in features are fully supported; everything beyond is on you or a partner you hire.

## Related

- [Duplicate your theme](../duplicating-your-theme/)
- [Support policy](../../support/support-policy/)
- [Shopify Partner Directory](https://www.shopify.com/partners/directory)

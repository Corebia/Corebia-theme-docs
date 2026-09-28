---
title: Typography
layout: default
parent: Theme settings
nav_order: 2
permalink: /theme-settings/typography/
---

# Typography

Four fonts, one text scale, and a full set of controls for each heading level, applied across the whole storefront.

The fonts are chosen once, at the top. Each heading level then picks which of them it uses, along with its own size, line height, letter spacing and case. Out of the box every heading level uses the body font, so the storefront reads as one family until you decide otherwise.

## Settings

### Headings

- **Font.** The heading font. Default: Inter Semi Bold. A heading level uses it when its own **Font** is set to **Heading**; some display elements, such as the shop name in the header, use it directly.
- **Subheading font.** Default: Inter Medium. Available to Heading 3 to Heading 6, and to badges.
- **Accent font.** Default: Inter Regular. A third voice for headings, buttons and badges.

### Body

- **Font.** The font used for body copy and interface text. Default: Inter Regular.

### Sizing

- **Text size.** Scales body text and UI proportionally. Range: 80% to 130% in 5% steps. Default: 100%, the design default.

### Heading 1 to Heading 6

Each of the six heading levels has its own group with the same five settings.

- **Font.** Which of the fonts above the level uses: **Heading**, **Accent** or **Body**, plus **Subheading** for Heading 3 to Heading 6. Default: **Body** for every level.
- **Size.** The size on desktop, chosen from 14px, 16px, 17px, 18px, 19px, 20px, 22px, 24px, 26px, 28px, 32px, 36px, 40px, 44px, 48px, 56px, 64px, 72px, 80px, 88px, 104px and 120px. On smaller screens the heading scales down smoothly, keeping its proportion to the other levels.
- **Line height.** **Tight**, **Normal** or **Loose**.
- **Letter spacing.** **Tight**, **Normal** or **Loose**.
- **Case.** **Default** or **Uppercase**. Default: **Default** for every level.

The defaults per level:

| Level | Size | Line height | Letter spacing |
|---|---|---|---|
| Heading 1 | 64px | Tight | Tight |
| Heading 2 | 48px | Tight | Tight |
| Heading 3 | 36px | Normal | Normal |
| Heading 4 | 28px | Normal | Normal |
| Heading 5 | 22px | Normal | Loose |
| Heading 6 | 19px | Normal | Loose |

Heading 6 also sets the case of product card titles, unless **Title case** under [Product cards](../product-cards/) overrides it.

## About the font picker

The picker offers Shopify's font library. Fonts from it are served by Shopify's own CDN, so there is nothing to upload, no third-party request and no licensing to arrange.

Each family exposes the weights and styles Shopify holds for it. A family with only one weight will render bold text by synthesizing it, which looks heavier and rougher than a real bold cut. If headings matter to you, prefer a family that ships several weights.

Custom fonts of your own aren't available through this setting. Adding one means editing the theme code and hosting the font files, which puts it outside what theme support covers.

## Tips

- **Change size before you change font.** Most "this doesn't feel right" reactions are about scale, not typeface. Adjusting **Size** on Heading 1 and Heading 2 changes the character of a page more than swapping families does.
- **Give headings their own font by switching the level, not the picker.** Setting a heading font does nothing visible until a level's **Font** is set to **Heading**. Start with Heading 1 and Heading 2, and leave the smaller levels on **Body** for readability.
- **Use uppercase sparingly.** It works for short, small headings such as Heading 6. On a long Heading 1 it slows reading down.
- **Check the extremes.** At 130% **Text size** a long product title can wrap to three lines on a phone; at 80% metadata gets close to unreadable. Look at a real product page at both ends before settling.
- **Every extra font is a download.** Each font you put to use adds a file the browser fetches. Using one family at different weights is lighter than mixing three.

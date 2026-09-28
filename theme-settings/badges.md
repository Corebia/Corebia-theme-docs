---
title: Badges
layout: default
parent: Theme settings
nav_order: 13
permalink: /theme-settings/badges/
---

# Badges

The look of every badge in the store, and your own badges driven by product tags. Badges appear on product card images (sale, new, promotion and tag badges) and beside a price on product pages.

What a sale badge says is set under [Discount display](../discount-display/); how long a product counts as new is set under [Product cards](../product-cards/).

## Settings

- **Position.** Where the badge sits on a product card image. **Top left** (default), **Top right** or **Bottom left**. Badges shown next to a price are unaffected. A sold-out product's **Sold out** badge takes the same corner, and on a sold-out card it is the only badge shown.
- **Corner radius.** Rounds every badge to the same radius. Range: 0 to 100 px in 2 px steps. Default: 100 px. At 100 the theme keeps its own shapes instead: a pill on card images, a softly rounded chip beside a price.
- **Font.** Applies to every badge, both on product card images and beside a price. **Body** (default), **Subheading**, **Heading** or **Accent**. The fonts themselves are set in [Typography](../typography/).
- **Text case.** **As typed** or **Uppercase** (default). Uppercase matches the other labels in the theme.
- **Tag badges.** Your own badges, one per line. See below.

## Tag badges

Write one rule per line, as the tag, a colon, then the label to show:

```
handmade: Handmade
limited: Limited edition
organic: Organic cotton
```

A product carrying that tag shows that badge. The whole tag has to match, and capitalization is ignored, so `Handmade` and `handmade` are the same tag, but `handmade-in-italy` is not `handmade`.

A card shows one badge at a time. A tag badge shows below a promotion label and above the sale and new badges, so a tagged product on sale shows its tag badge, not its discount. The full order is under [Discount display](../discount-display/#which-badge-wins).

Turning off **Show discount badge**, in Discount display, hides tag badges too.

## Tips

- **Tag badges are for facts, not urgency.** `Handmade`, `Organic`, `Made in Portugal` tell a shopper something true. Several products shouting `Bestseller` stop meaning anything.
- **Keep labels to one or two words.** The badge sits over the product image; a long label covers the photograph.
- **Remember that tags win over sales.** If a product needs to show its discount during a sale, remove its badge tag for the duration, or add the tag badge only to full-price lines.
- **Move the badge if it keeps covering the product.** Look at a full collection page after changing **Position**. The right corner depends on how your photography is framed, not on a rule.

---
title: Multi-currency and language
layout: default
parent: Features
nav_order: 15
permalink: /features/multi-currency-language/
---

# Multi-currency and language

Pave supports multi-currency and multi-language stores through Shopify Markets. When you sell to more than one country or publish more than one language, shoppers get a country/region and language selector, prices in their currency and the theme's own text in their language.

## Where the selectors appear

| Place | When it shows | Setting |
|---|---|---|
| [Footer](../../sections/footer/), at the top beside the wordmark | Always, once there is something to choose | None |
| [Header](../../sections/header/), in the navigation panel | When turned on | **Show country/region selector** and **Show language selector**, both off by default |
| [Announcement bar](../../sections/announcement-bar/) | When turned on | **Show country/region and language selector**, off by default |

Each selector only renders when there is a choice to make: the country selector needs more than one country to sell to, the language selector more than one published language. A store with a single market and a single language shows neither, whatever the settings say.

## Setting up multi-currency

1. In `Shopify admin > Settings > Markets`, add the markets (countries) you want to sell in.
2. For each market, set the currency. Shopify Payments converts prices using current exchange rates.
3. Save.

Customers pick a country, prices update, and checkout proceeds in the local currency.

Several currencies share the `$` symbol, so Pave can print the currency code after prices, as in `$10.00 CAD`. That is controlled under [Currency code](../../theme-settings/currency-code/) in theme settings, separately for product pages, product cards, cart lines and the cart total.

## Setting up multi-language

1. In `Shopify admin > Settings > Languages`, add the languages you want to publish.
2. Translate your store content with the free **Translate & Adapt** app or a paid translation app.
3. Publish the language.

## Languages the theme ships

Pave's own text (buttons, labels, messages, accessibility text) comes translated into ten languages:

- English
- Spanish
- French
- Italian
- German
- Portuguese (Brazil)
- Portuguese (Portugal)
- Dutch
- Swedish
- Polish

When you publish one of these languages, the theme's text appears in it with no further work. Dates, such as an article's publish date, and counts, such as "3 items", follow the shopper's language and its plural rules.

The theme editor is translated into the same ten languages, so setting names follow the language of your Shopify admin.

For any other language, the theme's text is translated through your translation app or under `Online Store > Themes > ... > Edit default theme content`. Your own content (products, collections, pages, text you typed into sections) is translated in `Settings > Languages`, whatever the language.

## Right-to-left languages

When the storefront's language is written right to left, such as Arabic or Hebrew, the layout mirrors: text aligns to the right, drawers slide in from the left, and carousels, sliders and arrows follow the reading direction. Nothing needs configuring. The theme's own text isn't shipped in a right-to-left language, so translate it as described above.

## Color and size options in other languages

Swatches, size buttons and the size guide link depend on the theme recognizing an option as a color or a size. It recognizes the usual option names in 16 languages, among them `Color`, `Colour`, `Couleur`, `Farbe`, `Talla`, `Taille` and `Größe`. An option with an unusual name, such as `Shade`, is treated as a plain option. See [Swatches](../swatches/).

## Tips

- **Markets first, language second.** Customers in a country may speak the same language; configuring markets but not languages still gives them prices in their currency.
- **Test the currency conversion.** Switch the country and check that prices, shipping and taxes calculate correctly.
- **Translate everything you can.** Untranslated content, or a mix of two languages on one page, reads as unfinished.
- **Put the selector where shoppers look.** The footer always has it; turn it on in the header or the announcement bar if a large share of your traffic comes from abroad.
- **Custom translations.** Edits to the theme's locale files are not covered by support. See [Custom code](../../customization/custom-code/).

## Troubleshooting

- **Country selector doesn't appear.** Confirm at least two countries are set up in `Shopify admin > Settings > Markets`.
- **Language selector doesn't appear.** Confirm at least two languages are published in `Shopify admin > Settings > Languages`.
- **Prices don't change when I switch country.** Check that Shopify Payments is enabled and set up for the additional markets. Without Shopify Payments, multi-currency needs a third-party currency conversion app.
- **Some text isn't translated.** Text you typed into a section or a product needs translating in `Settings > Languages`. Theme text in a language Pave doesn't ship needs translating through your translation app or **Edit default theme content**.

## Related

- [Footer section reference](../../sections/footer/)
- [Currency code](../../theme-settings/currency-code/)
- [Shopify Help: Markets](https://help.shopify.com/en/manual/markets)
- [Shopify Help: Languages](https://help.shopify.com/manual/online-store/languages)

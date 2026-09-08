---
title: Multi-currency and language
layout: default
parent: Features
nav_order: 15
permalink: /features/multi-currency-language/
---

# Multi-currency and language

Pave supports multi-currency and multi-language stores via Shopify Markets. When you configure additional countries or languages, Pave automatically renders country and language selectors in the footer.

## Where the selectors appear

- The [Footer](../../sections/footer/) bottom bar, when more than one country and/or more than one language is published.

If only one country is configured, the country selector is hidden. If only one language is published, the language selector is hidden. There is no theme setting to enable or disable these selectors; they appear automatically based on Shopify Markets configuration.

## Setting up multi-currency

1. In `Shopify admin > Settings > Markets`, add the markets (countries) you want to sell in.
2. For each market, configure the currency. Shopify Payments converts prices automatically using current exchange rates.
3. Save.

Once at least two markets are configured, the country selector appears in Pave's footer. Customers pick a country, prices update, and checkout proceeds in the local currency.

## Setting up multi-language

1. In `Shopify admin > Settings > Languages`, add the languages you want to publish.
2. Translate your store content using one of:
   - The free **Translate & Adapt** Shopify app for manual translations.
   - A paid translation app (Langify, Weglot, etc.) for managed translations.
3. Publish the language.

Once at least two languages are published, the language selector appears in Pave's footer. Customers pick a language, the storefront re-renders with the translated content.

## Pave's translation files

Pave ships with English (`en.default.json`) as the default language. UI strings (button labels, accessibility text, error messages) are stored in this locale file. When you add a language to your store, you also need to translate Pave's UI strings. Most translation apps do this automatically.

If you have only configured your store in English, no language selector appears, and all UI strings come from the English locale.

## Tips

- **Markets first, language second.** Customers in a country may speak the same language; configuring markets but not languages still gives them prices in their currency.
- **Test the currency conversion.** Switch the country and verify prices, shipping, and taxes calculate correctly.
- **Translate everything you can.** Untranslated content (or worse, a mix) reads as unfinished.
- **Custom translations.** Customizations to the locale file (translations) are not covered by support. See [Custom code](../../customization/custom-code/).

## Troubleshooting

- **Country selector doesn't appear.** Confirm at least two markets are configured in `Shopify admin > Settings > Markets`.
- **Language selector doesn't appear.** Confirm at least two languages are published in `Shopify admin > Settings > Languages`.
- **Prices don't change when I switch country.** Verify Shopify Payments is enabled and configured for the additional markets. Without Shopify Payments, multi-currency requires a third-party currency conversion app.
- **Some text isn't translated.** Either Pave's locale file doesn't have a translation for that key (in which case translate it via your translation app or in `Shopify admin > Online Store > Themes > Edit default theme content`), or the content comes from the Shopify admin (products, collections) and needs translation in `Shopify admin > Settings > Languages > Translate`.

## Related

- [Footer section reference](../../sections/footer/)
- [Shopify Help: Markets](https://help.shopify.com/en/manual/markets)
- [Shopify Help: Languages](https://help.shopify.com/manual/online-store/languages)

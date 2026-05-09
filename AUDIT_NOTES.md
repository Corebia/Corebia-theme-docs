# Audit notes — findings about the theme code

These are findings discovered while writing the documentation. They are **theme code issues, not documentation issues**, and are listed here so the development team can act on them before submitting Pave to the Shopify Theme Store.

The full theme audit (with severity, file paths, and reproduction steps) lives in `plantilla/THEME_AUDIT.md` and `plantilla/THEME_AUDIT_FIXES.md`. This file is a short summary of the items most relevant to documentation reviewers.

## Confirmed blockers from the theme audit (must fix before Theme Store submission)

The theme's own audit (`plantilla/THEME_AUDIT.md`) lists 11 confirmed blockers. The most important ones from a docs perspective:

1. **B-1** — `theme_documentation_url` and `theme_support_url` in `config/settings_schema.json` need to point to the public docs and a public contact form. `theme_documentation_url` is currently empty; `theme_support_url` is currently `mailto:support@corebia.com` and needs to be a public form URL.
2. **B-5** — Ampersands in setting labels (`Composition & Care`, `Shipping & Returns`, `Filters & toolbar`, `Press & media`) violate Shopify's "no ampersands" rule. Replace with `and`. The documentation already uses the corrected names ("Composition and care", "Shipping and returns", "Filters and toolbar", "Press and media"), so once the theme is fixed the docs match.
3. **B-6** — "homepage" (one word) appears in `locales/en.default.schema.json:153` and `:1134`. Should be "home page" (two words). The docs use the correct two-word form throughout.
4. **B-7 / B-8** — Cart locale uses "promo code" / "Have a promo code?" instead of Shopify's canonical "discount code". The docs use "discount code" throughout.
5. **B-10** — Defaults in Title Case (`Customer Reviews`, `Frequently Asked Questions`, `Recently Viewed`, `Complete the Look`, `Our Story`, `Learn More`, `Shop Now`) need to be sentence case. The docs use the corrected sentence-case form, but if the theme defaults are not fixed the merchant will see Title Case in the editor and sentence case in the docs — a small inconsistency.

## Items the docs document *as if* fixed

To ensure the docs are publishable as-is alongside the corrected theme, the following pages assume the items above are corrected. Verify after fixes land:

- `templates/product-page.md` documents the **Composition and care** and **Shipping and returns** collapsible tab kinds (no ampersand).
- `theme-settings/cart-settings.md` and `features/discounts.md` use "discount code" (no "promo code").
- `templates/home-page.md`, `sections/header.md`, and other pages use "home page" (two words).
- `templates/contact-page.md` documents `Press and media` as a default subject option (no ampersand).

## Other findings (not blockers, but mentioned in docs)

- The theme name in `config/settings_schema.json` is currently `Pave`. Earlier audit notes referenced `Pavé` with an accent. Confirm the final theme name and update `index.md` in the docs if it changes.
- The author in `theme_info` is `Corebian`. The docs use "Corebian" consistently.

## Items resolved in a follow-up pass

- **Support links** — All "Contact support" / "Open a support ticket" buttons in the docs now route internally to `/support/contact/` within `docs.corebia.com`. The contact page itself is informational and lists the support email (`support@corebia.com`) — there is no external contact-form URL anymore.
- **General website link** — Replaced with a "Documentation: https://docs.corebia.com" link on the contact page.

## Items still needing your input

- **EU compliance address and contact methods** — Not included. If Corebian operates in the EU, add a business address and a second direct contact method on `support/contact.md`.
- **Screenshots** — None included. Once the demo store is populated with real content, capture screenshots for the home page, product page, collection page, and cart, and inline them on the relevant pages.
- **Changelog** — `changelog.md` lists the 1.0.0 release. Add subsequent versions chronologically as they ship.

## Theme-side action required

In `plantilla/config/settings_schema.json`, set:

- `theme_documentation_url` → `https://docs.corebia.com`
- `theme_support_url` → `mailto:support@corebia.com` (the existing value is fine)

Note: Shopify Theme Store reviewers may push back on `mailto:` and prefer a public form. If they do, the simplest path is to set up a managed form (Tally, Typeform, Formspree, etc.) and update both the contact page and `theme_support_url`. That is a future decision and not blocking the current docs publish.

## Reference: full theme audit

For severity-ranked issues with file paths and reproduction steps, see:

- `plantilla/THEME_AUDIT.md`
- `plantilla/THEME_AUDIT_FIXES.md`

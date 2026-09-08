# Working notes

Internal notes on the state of this documentation and of the theme it documents. Excluded from the built site by `_config.yml`.

Last reconciled against the theme: **2026-09-08**, theme at `Pave 1.0.0`.

## How this documentation is kept true

Every reference page — [Sections](sections/), [Templates](templates/), [Theme settings](theme-settings/) — documents settings that exist in `plantilla/`, with the labels, options, ranges and defaults the merchant actually sees.

Those labels come from `plantilla/locales/en.default.schema.json`, resolved from the `t:` keys in each section's `{% schema %}`. When the theme changes a label, an option or a default, the corresponding page here is wrong until it is updated. The failure mode is silent: nothing breaks, the page simply lies.

**Before any Theme Store submission, re-check the reference pages against the theme's schemas.** The drift found on 2026-09-08 had accumulated over four months and touched every reference page in the site — one page alone was missing 47 settings.

## Theme metadata this site depends on

From `plantilla/config/settings_schema.json`:

```json
{
  "theme_name": "Pave",
  "theme_version": "1.0.0",
  "theme_author": "Corebia",
  "theme_documentation_url": "https://docs.corebia.com",
  "theme_support_url": "https://docs.corebia.com/support/"
}
```

`theme_support_url` points at the support index, so `support/index.md` is the page a merchant lands on from their Shopify admin. It has to work as a landing page, not just as a section index.

## Known gaps

1. **No contact form.** §21 of the Theme Store requirements asks for a public contact form carrying name, email, store URL (with an example), a description text area, file upload, an auto-responder, the theme name and a subject. `support/contact.md` currently routes to an email address instead. This is a submission blocker and needs a hosted form.
2. **No screenshots.** Every reference page is text. Screenshots of the sections in place would help, and can only be taken once a demo store exists.
3. **English only.** Matches the theme, which ships `en.default` alone.

## Things the theme does that are worth knowing when writing docs

- **Complementary products is not a section.** It is a mode of the Product recommendations section, chosen with its **Recommendation type** setting. A page exists at `sections/complementary-products.md` because merchants search for the term.
- **The theme ships two alternate templates**, `collection.all.json` (catalog) and `page.contact.json` (contact), documented as their own pages.
- **Customer pages are Shopify's**, not the theme's. The theme ships no `templates/customers/*` and the account entry point in the header is Shopify's own component.
- **Product card fragment** is a section with no settings, requested over the network by Recently viewed. It is not merchant-facing.

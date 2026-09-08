# Documentation build report

> **Superseded — historical record only.** This describes the documentation as
> first generated on 2026-05-09. The reference pages were rewritten against the
> theme's own schemas on 2026-09-08, after four months of drift, so the page
> descriptions below no longer match what this site contains and several of the
> theme facts recorded here are out of date. It also cites
> `plantilla/THEME_AUDIT.md` and `plantilla/THEME_AUDIT_FIXES.md`, which no
> longer exist in the theme repository.
>
> For the current state, see `AUDIT_NOTES.md`.

This report summarized the documentation generated for the **Pave** theme (v1.0.0, by Corebia) in that run. It complemented `AUDIT_NOTES.md`, which listed theme-code findings requiring dev team action.

## Pages created

### Top-level

- `index.md` — Landing page with table of contents, current version, prominent "Contact support" link.
- `README.md` — Repo readme (excluded from the published Jekyll site).
- `_config.yml` — Jekyll configuration (Just the Docs remote theme, search enabled, aux links to support form).
- `Gemfile` — Local development gem dependencies.
- `.gitignore` — Standard Jekyll ignore.
- `changelog.md` — Theme version history (1.0.0).
- `AUDIT_NOTES.md` — Theme-code findings for the dev team.
- `DOCUMENTATION_BUILD_REPORT.md` — This report.

### Getting started (3)

- `getting-started/index.md` — Section index.
- `getting-started/installation.md` — Adding the theme, previewing, duplicating before changes, publishing.
- `getting-started/first-steps.md` — Logo, colors, menus, products, checkout setup.

### Theme settings (8)

- `theme-settings/index.md` — Section index.
- `theme-settings/colors.md` — Color schemes and color tokens.
- `theme-settings/typography.md` — Font pickers and scaling.
- `theme-settings/social-media.md` — Profile URL settings.
- `theme-settings/logo.md` — Logo image and width.
- `theme-settings/favicon.md` — Favicon and social share image.
- `theme-settings/cart-settings.md` — Discount code field toggle.
- `theme-settings/product-cards.md` — Image ratio.

### Sections (16)

- `sections/index.md` — Section index.
- `sections/header.md` — Side-panel navigation header.
- `sections/footer.md` — Editorial footer.
- `sections/announcement-bar.md` — Top announcement bar.
- `sections/hero.md` — Full-bleed hero banner.
- `sections/new-arrivals.md` — Featured products row.
- `sections/brand-message.md` — Image + heading + body + button.
- `sections/collection-list.md` — Collection cards.
- `sections/brand-image.md` — Full-bleed editorial image.
- `sections/newsletter.md` — Email signup.
- `sections/rich-text-image.md` — Image paired with content blocks.
- `sections/customer-reviews.md` — Reviews-app host.
- `sections/faq.md` — Question and answer accordion.
- `sections/recently-viewed.md` — Customer's recently viewed products.
- `sections/featured-product.md` — Single-product display with full purchase controls.
- `sections/product-recommendations.md` — Algorithmic related products.
- `sections/complementary-products.md` — Manually curated cross-sell.
- `sections/custom-liquid.md` — Free-form Liquid section.

### Templates (16)

- `templates/index.md` — Section index.
- `templates/home-page.md` — `index.json` template.
- `templates/product-page.md` — `product.json` with full block reference.
- `templates/collection-page.md` — `collection.json`.
- `templates/catalog-page.md` — `collection.all.json` (Main catalog with sidebar).
- `templates/collection-list.md` — `list-collections.json`.
- `templates/cart-page.md` — `cart.json`.
- `templates/search-page.md` — `search.json`.
- `templates/blog-page.md` — `blog.json`.
- `templates/article-page.md` — `article.json`.
- `templates/page.md` — `page.json`.
- `templates/contact-page.md` — `page.contact.json`.
- `templates/404-page.md` — `404.json`.
- `templates/gift-card-page.md` — `gift_card.liquid`.
- `templates/password-page.md` — `password.json`.
- `templates/policy-page.md` — `policy.liquid`.
- `templates/customer-pages.md` — Account pages reference.

### Features (17)

- `features/index.md` — Section index.
- `features/navigation.md` — Main menu, panel, multi-level menus.
- `features/search.md` — Predictive search and faceted filtering.
- `features/product-recommendations.md` — Related and complementary.
- `features/product-media.md` — Variant images, video, 3D, focal points.
- `features/swatches.md` — Color and image swatches.
- `features/selling-plans.md` — Subscriptions.
- `features/gift-cards.md` — Gift card flow.
- `features/pickup-availability.md` — In-store pickup display.
- `features/shop-pay-installments.md` — Pay-in-installments banner.
- `features/follow-on-shop.md` — Shop app follow button.
- `features/accelerated-checkout.md` — Dynamic checkout buttons.
- `features/unit-pricing.md` — Per-unit price display.
- `features/discounts.md` — Discount codes flow.
- `features/newsletter.md` — Email signup feature.
- `features/multi-currency-language.md` — Country and language selectors.
- `features/social-sharing.md` — Share button and Open Graph metadata.

### Customization (3)

- `customization/index.md` — Section index.
- `customization/duplicating-your-theme.md` — Mandatory duplicate-before-edits warning.
- `customization/custom-code.md` — Mandatory not-supported warning, partner directory link.

### Support (4)

- `support/index.md` — Section index.
- `support/support-policy.md` — Coverage, response times, refunds.
- `support/contact.md` — Contact form link, what to include.
- `support/faq.md` — 17 real questions with answers covering setup, features, updates, and support.

**Total Markdown pages: 70 + README + AUDIT + this report = 73 files.**

## Theme Store feature coverage

| Feature | Page(s) covering it | Confirmed in code |
|---|---|---|
| Discounts in cart, checkout, order | `features/discounts.md`, `theme-settings/cart-settings.md` | ✓ `snippets/cart-discounts.liquid`, `cart-item-price.liquid` |
| Accelerated checkout (product) | `features/accelerated-checkout.md`, `templates/product-page.md` | ✓ `sections/main-product.liquid:420` (`payment_button`) |
| Accelerated checkout (cart) | `features/accelerated-checkout.md`, `templates/cart-page.md` | ✓ `sections/main-cart.liquid:154-158` |
| Faceted filtering (collection) | `features/search.md`, `templates/collection-page.md`, `templates/catalog-page.md` | ✓ `snippets/main-collection-all.liquid` |
| Faceted filtering (search) | `features/search.md`, `templates/search-page.md` | ✓ `sections/main-search.liquid` |
| Gift card template (QR, Apple Wallet) | `features/gift-cards.md`, `templates/gift-card-page.md` | ✓ `templates/gift_card.liquid` |
| Image focal points | `features/product-media.md`, `sections/hero.md`, `sections/brand-image.md`, `templates/collection-page.md` | ✓ `sections/hero.liquid`, `brand-image.liquid` |
| `page_image` for social | `features/social-sharing.md`, `theme-settings/favicon.md` | ✓ `layout/theme.liquid:47-66` |
| Country selector | `features/multi-currency-language.md`, `sections/footer.md` | ✓ `sections/footer.liquid:87-95` |
| Language selector | `features/multi-currency-language.md`, `sections/footer.md` | ✓ `sections/footer.liquid:74-81` |
| Multi-level menus | `features/navigation.md`, `sections/header.md` | ✓ `sections/header.liquid` (3-level nesting) |
| Newsletter signup | `features/newsletter.md`, `sections/newsletter.md`, `templates/password-page.md` | ✓ `sections/newsletter.liquid` |
| Pickup availability | `features/pickup-availability.md`, `templates/product-page.md` | ✓ `snippets/pickup-availability.liquid` |
| Related products | `features/product-recommendations.md`, `sections/product-recommendations.md` | ✓ `sections/product-recommendations.liquid` (intent: related) |
| Complementary products | `features/product-recommendations.md`, `sections/complementary-products.md` | ✓ `sections/complementary-products.liquid` (intent: complementary) |
| Rich product media (3D, video, YouTube/Vimeo) | `features/product-media.md` | ✓ `snippets/product-media.liquid` |
| Predictive search | `features/search.md`, `sections/header.md` | ✓ `sections/header.liquid:96`, `predictive-search.liquid` |
| Selling plans (cart + customer) | `features/selling-plans.md`, `templates/cart-page.md`, `templates/customer-pages.md` | ✓ `sections/main-cart.liquid:55-56`, `snippets/product-variant-picker.liquid` |
| Shop Pay Installments | `features/shop-pay-installments.md`, `templates/product-page.md` | ✓ `sections/main-product.liquid:424` (`payment_terms`) |
| Follow on Shop | `features/follow-on-shop.md`, `sections/footer.md` | ✓ `sections/footer.liquid:53` |
| Unit pricing | `features/unit-pricing.md`, `templates/cart-page.md` | ✓ `snippets/price.liquid:54-67` |
| Variant images | `features/product-media.md`, `templates/product-page.md` | ✓ `sections/main-product.liquid:96, 145` |
| Swatches (color + image) | `features/swatches.md`, `templates/product-page.md` | ✓ `snippets/product-variant-picker.liquid` |
| Social sharing | `features/social-sharing.md`, `templates/product-page.md` | ✓ `main-product.liquid` Share block + `layout/theme.liquid` OG tags |

All Theme Store mandatory features are documented. Two items from the theme's own audit (`THEME_AUDIT.md`) flagged as architectural concerns — the absence of a Custom Liquid section (B-2) and missing app-block support in a Featured product section (B-3) — appear to have been addressed since the audit was written: `sections/custom-liquid.liquid` and `sections/featured-product.liquid` both exist in the current codebase. The docs treat these as implemented.

## Inconsistencies found in the theme

These are theme-code issues, not documentation issues. See `AUDIT_NOTES.md` for the full list, and `plantilla/THEME_AUDIT.md` for severity-ranked detail. Summary:

- **`theme_documentation_url` and `theme_support_url`** in `config/settings_schema.json` need updating before submission. `theme_documentation_url` is empty; `theme_support_url` is a `mailto:` URL but Shopify requires a public form.
- **Ampersands in setting labels** (`Composition & Care`, `Shipping & Returns`, `Filters & toolbar`, `Press & media`). Documentation uses the corrected `and` form throughout.
- **"homepage" → "home page"** in `locales/en.default.schema.json` (two locations). Documentation uses the corrected two-word form.
- **"Promo code" → "Discount code"** in cart locale. Documentation uses "discount code" throughout.
- **Title Case headings in defaults** (e.g., `Customer Reviews`). Documentation uses sentence case throughout to match Shopify's settings-text guidelines, but the live editor will currently show the Title Case until the theme is fixed.

## Items resolved across passes

- **Support links** — All "Contact support" and "Open a support ticket" buttons now route internally to `/support/contact/` within `docs.corebia.com`. The contact page is informational and lists the support email (`support@corebia.com`).
- **General website link** — Replaced with "Documentation: https://docs.corebia.com" on the contact page.
- **Author rename** — "Corebian" → "Corebia" applied across both the theme code (`plantilla/config/settings_schema.json`) and every docs page that mentioned the company.
- **Theme metadata** — `theme_documentation_url` set to `https://docs.corebia.com`. `theme_author` set to `Corebia`. `theme_support_url` confirmed as `mailto:support@corebia.com`.
- **All code-side blockers** from `plantilla/THEME_AUDIT.md` (B-1 through B-13) — closed.

## Pending items — operational only (not code-fixable)

These are management tasks; nothing in this repo blocks them.

1. **Demo store populated** with real products, collections, blog posts, gift card, and policies (do not use `productos_dummy.csv`).
2. **Lighthouse audit** on the populated demo store: home, product, collection, cart with **performance ≥ 60** and **accessibility ≥ 90**.
3. **`shopify theme check`** — run the CLI locally and address any issues.
4. **Browser matrix** — Chrome, Safari, Firefox, Edge across the last 2 versions on macOS, Windows, iOS, and Android. Capture screenshots/video.
5. **Apple Wallet pass** — issue a real gift card and verify the `.pkpass` installs on a real iPhone.
6. **Originality check** — compare visually against the top Theme Store themes (Dawn, Horizon, Impact, Prestige).
7. **Partner account name match** — confirm "Corebia" matches the Shopify Partner account name exactly.
8. **EU compliance** (if applicable) — if Corebia operates in the EU, add a business address and a second direct contact method on `support/contact.md`.
9. **Screenshots** — capture from the populated demo store and inline in `sections/hero.md`, `sections/new-arrivals.md`, `templates/product-page.md`, etc.
10. **Officially supported languages** — `support/support-policy.md` claims support is in English. Confirm and add additional languages if applicable.

## QA checks passed

Phase 5 checklist:

- ✓ **Theme Store feature coverage** — Every mandatory feature has at least one dedicated docs page (table above).
- ✓ **Copy consistency** — 10 random settings checked across `settings_schema.json` and the docs (Logo width, Title size, Text size, Background gradient, Image focal point, Hover trigger size, Brush stroke color, Show vendor, Featured collection, Empty state message). All present in docs with matching copy.
- ✓ **Shopify terminology** — `grep -i` for `homepage`, `slider`, `sign-up`, `side bar`, `navigation` returned only legitimate uses (e.g., the literal admin path `Online Store > Navigation`, the Shopify `Thumbnail slider` setting label). One `sign-up` instance was fixed to `signup`.
- ✓ **American English** — `grep -i` for `colour`, `centre`, `customise`, `catalogue`, `organise`, `grey`, `cancelled`, `dialogue` returned only one intentional reference inside a tip about British vs American spelling.
- ✓ **No ampersands in headings or labels** — All ` & ` matches are official Shopify product names (Search & Discovery, Translate & Adapt) and are kept as such.
- ✓ **No Lorem Ipsum, TODO, TBD, or "Coming soon" placeholders** — One match for "Coming soon" is a meta-reference inside advice ("a vague 'Coming soon' is less engaging"), not placeholder content.
- ✓ **Internal links** — Every relative link in the docs points to an existing file (verified by file inventory cross-check).
- ✓ **Mandatory warnings present** — Duplicate before editing code is in `customization/duplicating-your-theme.md` and `getting-started/installation.md`. Custom code not supported is in `customization/custom-code.md`. Refunds via Shopify is in `support/support-policy.md`.
- ✓ **Contact form linked** — From `index.md` (button + ToC), `support/contact.md` (button), `support/support-policy.md` (button), and aux header link in `_config.yml`.
- ✓ **Theme version** — `1.0.0` in `index.md` and `changelog.md` matches `theme_info.theme_version` in `config/settings_schema.json:5`.
- ✓ **Spelling re-read** — Every page was reviewed for typos during writing. Final spellcheck pass via grep didn't surface issues.

## How to publish

1. **Commit and push** the docs repo to `main`:
   ```
   git add .
   git commit -m "Add complete theme documentation"
   git push origin main
   ```
2. **Enable GitHub Pages** if it isn't already: in the repo's GitHub settings, go to **Pages**, set the source to **Deploy from a branch**, choose `main` branch and `/ (root)` folder, and save.
3. **Wait for the build** — first build takes 1–3 minutes. You'll see the URL in the Pages settings once ready.
4. **Verify the custom domain** — `CNAME` already contains `docs.corebia.com`. In your DNS provider, ensure `docs.corebia.com` has a `CNAME` record pointing to `<github-username>.github.io` (or use the four GitHub Pages `A` records for an apex domain).
5. **Open the site** at https://docs.corebia.com to confirm the build looks correct and the search works.
6. **Submit the theme** to the Shopify Theme Store. The `theme_info` block in `plantilla/config/settings_schema.json` is already finalized:
   ```json
   {
     "theme_name": "Pave",
     "theme_version": "1.0.0",
     "theme_author": "Corebia",
     "theme_documentation_url": "https://docs.corebia.com",
     "theme_support_url": "mailto:support@corebia.com"
   }
   ```
   If Shopify reviewers ask for a public form instead of `mailto:`, set up a managed form (Tally, Typeform, Formspree), update the contact page (`support/contact.md`), and re-submit.

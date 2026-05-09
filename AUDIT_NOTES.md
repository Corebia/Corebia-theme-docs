# Audit notes — final state

These are the findings discovered while writing the documentation, as of the final pass on 2026-05-09. The full theme audit (with severity, file paths, and reproduction steps) lives in `plantilla/THEME_AUDIT.md` and `plantilla/THEME_AUDIT_FIXES.md`.

## Code-side blockers — all resolved

Every Theme Store code-side blocker tracked in the original `plantilla/THEME_AUDIT.md` (B-1 through B-13) is now resolved in the theme code.

| ID | Item | Status |
|---|---|---|
| B-1 | `theme_info` URLs apuntaban al repo del autor | ✅ `theme_documentation_url=https://docs.corebia.com`, `theme_support_url=mailto:support@corebia.com` |
| B-2 | Custom Liquid SECTION ausente | ✅ `sections/custom-liquid.liquid` añadida |
| B-3 | Featured product section ausente | ✅ `sections/featured-product.liquid` añadida con `@app` blocks |
| B-4 | Swatches API `option_value.swatch.image/.color` | ✅ Implementado en `snippets/product-variant-picker.liquid` |
| B-5 | Ampersands en setting labels | ✅ "and" en lugar de "&" en `locales/` |
| B-6 | "homepage" → "home page" | ✅ Corregido en `locales/en.default.schema.json` |
| B-7+B-8 | "Promo code" → "Discount code" + label declarativo | ✅ Corregido en cart locale |
| B-10 | Defaults en Title Case → sentence case | ✅ 7 cambios en `locales/en.default.schema.json` |
| B-11 | Social media info con username "shopify" | ✅ Reemplazado por descripciones genéricas |
| B-13 | Theme name "Pavé" (no-ASCII) → "Pave" | ✅ Corregido |
| A-7 | "X (Twitter)" → "X" | ✅ |
| A-8 | "1200 x 628" → "1200 by 628" | ✅ |

## Theme metadata — finalized

`plantilla/config/settings_schema.json` `theme_info` block:

```json
{
  "name": "theme_info",
  "theme_name": "Pave",
  "theme_version": "1.0.0",
  "theme_author": "Corebia",
  "theme_documentation_url": "https://docs.corebia.com",
  "theme_support_url": "mailto:support@corebia.com"
}
```

Note: Shopify Theme Store reviewers occasionally prefer a public form over `mailto:`. If they push back, set up a managed form (Tally, Typeform, Formspree) and update both `theme_support_url` and the docs `support/contact.md`. Not a current blocker.

## Items still pending — operational only

These are management tasks; they cannot be fixed in code from this pass.

1. **Demo store populated** with real products, collections, blog posts, gift card, and policies (do not use `productos_dummy.csv` from the repo).
2. **Lighthouse audit** on the populated demo store: home / product / collection / cart with **performance ≥ 60** and **accessibility ≥ 90**.
3. **`shopify theme check`** — run the CLI locally and address anything reported.
4. **Browser matrix** — Chrome, Safari, Firefox, Edge on the last 2 versions across macOS, Windows, iOS, and Android. Capture screenshots or video evidence.
5. **Apple Wallet pass** — issue a real gift card, scan the QR / use the wallet button on a real iPhone, and confirm the `.pkpass` installs.
6. **Originality check** — compare Pave with the top Theme Store themes (Dawn, Horizon, Impact, Prestige) to confirm it doesn't read as a clone.
7. **Partner account name match** — confirm that "Corebia" exactly matches the name on the Shopify Partner account.
8. **EU compliance** (if applicable) — if Corebia operates in the EU, add a geographical business address and a second direct contact method on `support/contact.md`.
9. **Screenshots** — capture key flows from the demo store (home, product page, collection, cart) and inline them in the relevant docs pages (`sections/hero.md`, `templates/product-page.md`, etc.).
10. **(Optional) `templates/customers/*`** — only if a Shopify reviewer specifically requests customer-page templates with selling plans.

## Fully-resolved items in earlier passes

For history:

- All "Contact support" / "Open a support ticket" buttons in the docs route to `/support/contact/` within `docs.corebia.com`. The contact page is informational and lists the support email; there is no external contact-form URL.
- The author rename "Corebian" → "Corebia" landed in this pass across both theme code and docs.

## Reference

- `plantilla/THEME_AUDIT.md` — original code audit with severity-ranked issues.
- `plantilla/THEME_AUDIT_FIXES.md` — record of which audit items were fixed and how.

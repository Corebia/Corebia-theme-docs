# Working notes

Internal notes on the state of this documentation and of the theme it documents. Excluded from the built site by `_config.yml`.

Last reconciled against the theme: **2026-09-28**, theme at `Pave 1.0.0`, branch `feature/f19-submission` (commit `505f32db`).

## How this documentation is kept true

Every reference page under [Sections](sections/), [Templates](templates/) and [Theme settings](theme-settings/) documents settings that exist in `plantilla/`, with the labels, options, ranges and defaults the merchant actually sees.

Those labels come from `plantilla/locales/en.default.schema.json`, resolved from the `t:` keys in each section's `{% schema %}`. When the theme changes a label, an option or a default, the corresponding page here is wrong until it is updated. The failure mode is silent: nothing breaks, the page simply lies.

**Before any Theme Store submission, re-check the reference pages against the theme's schemas.** The drift found on 2026-09-08 had accumulated over four months and touched every reference page in the site. One page alone was missing 47 settings.

The 2026-09-28 pass came after F1 to F19 (theme blocks, languages and RTL, B2B, accessibility, motion, editorial sections): three weeks of feature work that again touched every reference page, and added 17 merchant-facing sections (21 new section files in all), 9 theme settings groups, 12 theme blocks and 12 templates the site did not document.

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

## The GitHub Pages build is the only gate

There is no CI on this repository and no local Jekyll toolchain, so a template
error is not caught until Pages tries to build. **After every push, check that
the build actually succeeded**, and check the Actions run rather than the Pages API:

```bash
gh run list --repo Corebia/Corebia-theme-docs --limit 3
gh run view <id> --repo Corebia/Corebia-theme-docs --log-failed
```

A failed build leaves the **previous** version serving, so `docs.corebia.com`
answering 200 proves nothing about the commit you just pushed. Confirm by
fetching a string that only exists in the new content.

The Pages API is not a reliable signal on its own: a run that fails leaves
`repos/.../pages/builds/latest` reporting `building` indefinitely.

One failure has already happened this way, and it is worth knowing the shape
of it: a literal Liquid tag written **inside** a `comment` block closes that
block early, and the build dies on the orphaned closing tag. Instructions
written inside a comment must not contain Liquid tags.

## Known gaps

1. **The contact form is not live yet.** The page is built for it; the form itself has to be created. See below.
2. **No screenshots.** Every reference page is text. Screenshots of the sections in place would help, and can only be taken once a demo store exists.
3. **English only.** The theme now ships storefront and editor translations in ten languages (en, es, fr, it, de, pt-BR, pt-PT, nl, sv, pl), but this site documents the English editor labels only. A merchant working in another admin language sees translated labels.

## Building the contact form

The embed is already written. `support/contact.md` includes `_includes/contact-form.html`, which renders the Tally iframe as soon as `tally_form_id` is set in `_config.yml`, and an email fallback until then. **A contact email on its own does not satisfy §21.** The requirement is a form.

So going live is one line of YAML: take the id out of the form's share link, `https://tally.so/r/<id>`, and set `tally_form_id` to just that id.

The embed URL is built from Tally's own contract rather than copied from their UI, so the options are fixed in the include: `alignLeft=1`, `hideTitle=1`, `transparentBackground=1`, `dynamicHeight=1`. The last two are the ones that matter. `tally.so/widgets/embed.js` looks for `dynamicHeight=1` before attaching its resizer, without which the form scrolls inside a fixed box, and for `transparentBackground=1` before letting the page's own background show through. To change the options, edit the query string in the include.

If Tally ever changes that contract, their **Share > Embed > Standard embed > Get the code** output is the authority: paste it over the whole `if` branch of the include.

### Fields §21 requires

| Field | Requirement |
|---|---|
| Name | First and last |
| Email address | n/a |
| Store URL | Must show an example, such as `http://www.storename.myshopify.com`. Put it in the field's placeholder or help text |
| Description of problem | Must be a **text area**, not a single-line input |
| File upload | So merchants can attach screenshots |
| Auto-responder | Fires on submit. It exists so merchants don't write again asking whether the message arrived, which Shopify names as the reason |
| Theme name | *"if you offer multiple themes"*. Corebia ships one, so this is **not required** |
| Subject | Conditional: if included, it must populate the email subject line |

So six required fields, and two that don't apply while Pave is the only theme.

Do **not** ask for budget, phone number or project type. §21 names those as the fields to avoid. That is an agency enquiry form, not a support form.

### Tally setup

1. Build the form with the six fields, and put the example URL in the store URL field's placeholder. §21 asks for the example, not just the field.
2. Use Tally's **File upload** question type for the attachment field.
3. Under **Integrations > Email**, set an auto-reply to the respondent. **This is the auto-responder requirement, and it is the step most likely to be missed**: it is an integration, not a question, so a form that looks complete can still fail this one.
4. Set `tally_form_id` in `_config.yml` to the id from the form's share link. Nothing else needs pasting, because the embed is already written.
5. Push, watch the Pages build, then open `/support/contact/` and submit a test message. Confirm the auto-reply arrives and that the attachment came through.
6. Check it on a phone. The embed asks Tally for dynamic height, so the form should grow rather than scroll inside its own box.

### Where the URL goes afterwards

- **Theme Store listing**, under *Merchant support > Contact and documentation*: the form URL, and `https://docs.corebia.com` for the documentation. This is the link a reviewer checks.
- **`theme_support_url`** in `plantilla/config/settings_schema.json` currently points at `https://docs.corebia.com/support/`, the support hub, which carries a contact button and the FAQ above it. That deflects tickets, and is the reason it is not pointed straight at the form. Either target conforms, since `shopify.dev` only says "a URL where merchants can find support for the theme", so this is a choice rather than a requirement.
- Note that `theme_support_email` and `theme_support_url` are mutually exclusive. Setting both is an error.

## Things the theme does that are worth knowing when writing docs

- **Complementary products is not a section.** It is a mode of the Product recommendations section, chosen with its **Recommendation type** setting. A page exists at `sections/complementary-products.md` because merchants search for the term; the Sections index lists it as a mode, not a section.
- **Collection list is `sections/collections-list.liquid`.** The docs page is `sections/collection-list.md` because the editor calls the section "Collection list". Keep the docs name and URL; the theme file name is not something a merchant sees.
- **The theme ships fourteen alternate templates**: three product (`editorial`, `gift-card`, `quick-order`), two collection (`all`, `lookbook`) and nine page (`contact` plus `about`, `accessibility`, `contact-stores`, `drop`, `editorial`, `faq`, `lookbook`, `size-guide`). Catalog, contact and lookbook collection have their own pages; the rest are grouped in `templates/product-templates.md` and `templates/page-templates.md`.
- **Customer pages are Shopify's**, not the theme's. The theme ships no `templates/customers/*` and the account entry point in the header is Shopify's own component.
- **Sections with no editor presence.** Product card fragment, Product quick view, Search empty state, Cart drawer and Cart suggestions have no settings and no presets; they are rendered by the layout or fetched over the network. Cart drawer and suggestions are configured under Theme settings > Cart. **Predictive search** does have six settings in its schema, but the section sits in no template or group, so a merchant can never reach them and they always run at their defaults. The docs page describes the results panel instead of the settings.
- **Newsletter popup** is rendered from `layout/theme.liquid` and is **off by default** since F19.
- **Theme labels are not all American English.** "Shop by colour", "Personalisation" and "centre" in some help texts. The docs quote labels verbatim and write prose in American English.
- **Some theme help texts contain em dashes** (`badge_tag_pairs`, `card_swatch_radius`). Rephrase them, never copy them.

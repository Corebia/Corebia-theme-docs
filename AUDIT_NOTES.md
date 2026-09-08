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

## The GitHub Pages build is the only gate

There is no CI on this repository and no local Jekyll toolchain, so a template
error is not caught until Pages tries to build. **After every push, check that
the build actually succeeded** — and check the Actions run, not the Pages API:

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
3. **English only.** Matches the theme, which ships `en.default` alone.

## Building the contact form

`support/contact.md` includes `_includes/contact-form.html`, which currently renders an email fallback. Replacing that file's contents with Tally's generated embed code puts the form live. **A contact email on its own does not satisfy §21** — the requirement is a form.

### Fields §21 requires

| Field | Requirement |
|---|---|
| Name | First and last |
| Email address | — |
| Store URL | Must show an example, such as `http://www.storename.myshopify.com`. Put it in the field's placeholder or help text |
| Description of problem | Must be a **text area**, not a single-line input |
| File upload | So merchants can attach screenshots |
| Auto-responder | Fires on submit. It exists so merchants don't write again asking whether the message arrived — Shopify names that as the reason |
| Theme name | *"if you offer multiple themes"*. Corebia ships one, so this is **not required** |
| Subject | Conditional: if included, it must populate the email subject line |

So six required fields, and two that don't apply while Pave is the only theme.

Do **not** ask for budget, phone number or project type. §21 names those as the fields to avoid — that is an agency enquiry form, not a support form.

### Tally setup

1. Build the form with the six fields, and put the example URL in the store URL field's placeholder.
2. Turn on the file upload question type.
3. Under **Integrations > Email**, set an auto-reply to the respondent. This is the auto-responder requirement; without it the form does not conform.
4. **Share > Embed > Standard embed**: turn on *Dynamic height* and *Align content to the left*, then **Get the code** and paste it into `_includes/contact-form.html`, replacing the whole fallback block.
5. If you use a popup rather than an inline embed, §21 adds that it must be mobile friendly and linkable from the Theme Store.

### Where the URL goes afterwards

- **Theme Store listing**, under *Merchant support > Contact and documentation*: the form URL, and `https://docs.corebia.com` for the documentation. This is the link a reviewer checks.
- **`theme_support_url`** in `plantilla/config/settings_schema.json` currently points at `https://docs.corebia.com/support/`, the support hub, which carries a contact button and the FAQ above it. That deflects tickets, and is the reason it is not pointed straight at the form. Either target conforms — `shopify.dev` only says "a URL where merchants can find support for the theme" — so this is a choice, not a requirement.
- Note that `theme_support_email` and `theme_support_url` are mutually exclusive. Setting both is an error.

## Things the theme does that are worth knowing when writing docs

- **Complementary products is not a section.** It is a mode of the Product recommendations section, chosen with its **Recommendation type** setting. A page exists at `sections/complementary-products.md` because merchants search for the term.
- **The theme ships two alternate templates**, `collection.all.json` (catalog) and `page.contact.json` (contact), documented as their own pages.
- **Customer pages are Shopify's**, not the theme's. The theme ships no `templates/customers/*` and the account entry point in the header is Shopify's own component.
- **Product card fragment** is a section with no settings, requested over the network by Recently viewed. It is not merchant-facing.

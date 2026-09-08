# Pave theme documentation

This repository hosts the public documentation for the **Pave** Shopify theme by Corebia. The site is built with [Jekyll](https://jekyllrb.com/) and the [Just the Docs](https://just-the-docs.com/) remote theme, and is served via GitHub Pages at [docs.corebia.com](https://docs.corebia.com).

## What this is

The site you see at `docs.corebia.com` is the URL referenced from the Pave theme's `theme_documentation_url` in the Shopify Theme Store. Merchants who install Pave land here to learn how to configure the theme, customize sections, and contact support.

## How it is served

1. Commits to the `main` branch trigger a GitHub Pages build.
2. GitHub Pages renders the Markdown files in this repo using the `_config.yml` configuration.
3. The built site is published at [docs.corebia.com](https://docs.corebia.com) (custom domain configured via `CNAME`).

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

The site is then available at `http://localhost:4000`.

## Repository layout

- `index.md`: Landing page.
- `getting-started/`: Installation and first-steps guides.
- `theme-settings/`: Documentation for every category in the theme settings.
- `sections/`: One page per storefront section.
- `templates/`: One page per page template.
- `features/`: Documentation for Shopify Theme Store mandatory features.
- `customization/`: Guidance for code edits and custom modifications.
- `support/`: Support policy, contact instructions, FAQ.
- `changelog.md`: Theme version history.

## Editing

Content lives in plain Markdown with [Just the Docs front matter](https://just-the-docs.com/docs/navigation-structure/). Each page declares its position in the navigation tree via `nav_order` and `parent`.

## Reporting issues with the docs

For issues with the documentation itself (typos, broken links, unclear instructions), open an issue on this repository. For issues with the theme, see [Contact support](https://docs.corebia.com/support/contact/).

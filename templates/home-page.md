---
title: Home page
layout: default
parent: Templates
nav_order: 1
permalink: /templates/home-page/
---

# Home page

The storefront entry point, at `/`. It uses `index.json`, so the entire section list is yours to arrange from the theme editor.

## Sections it ships with

A fresh install of Pave opens the home page with these six, in this order:

1. [Hero banner](../../sections/hero/): a full-height photograph carrying the brand name.
2. [New arrivals](../../sections/new-arrivals/): a row of hand-picked products, four to start with.
3. [Brand message](../../sections/brand-message/): copy beside an image, with a button.
4. [Collection list](../../sections/collection-list/): collections as image tiles, two to start with.
5. [Journal](../../sections/journal/): three articles from your `News` blog.
6. [Brand image](../../sections/brand-image/): a full-width photograph.

Around them sit the two section groups every page shares:

- **Header group**: the [Announcement bar](../../sections/announcement-bar/) and the [Header](../../sections/header/).
- **Footer group**: the [Newsletter](../../sections/newsletter/) signup and the [Footer](../../sections/footer/). Because the newsletter lives in the footer group, it appears at the foot of every page, not only the home page.

Select any section in the editor to change its settings, or use **Add section** to insert others.

### The newsletter popup is off

The [Newsletter popup](../../sections/newsletter-popup/) ships turned off. It is listed in the editor on every page, and nothing shows until you select it and turn on **Show popup**. It never shows to signed-in customers.

## Sections you can add

Almost every section in the theme can go on the home page. The exceptions are the ones tied to a group or a template: the header and footer sections, [Quick order list](../../sections/quick-order-list/) (product templates only) and [Related articles](../../sections/related-articles/) (article templates only). [Sections](../../sections/) lists them all.

## What the home page does differently

- **The header sits over the hero.** On the home page the header is transparent and its icons adapt to the image beneath them.
- **The top-left brand mark waits for the scroll.** It is hidden while the header sits over the hero, because the hero already carries the name, and appears once the shopper scrolls and the header takes a solid background. To show a mark over the hero too, upload a light version of your logo as **Inverse logo** under [Logo](../../theme-settings/logo/). When the header's **Desktop menu style** is the inline bar, the desktop bar keeps your regular logo either way.
- **The menu panel opens on hover.** On a desktop with a mouse, pointing at the top-right corner of the page opens the navigation panel (top-left in right-to-left languages). The size of that corner is the header's **Hover trigger size** setting. Everywhere else the panel opens on click.

## Tips

- **Lead with brand, then product.** Pave is designed for a hero-first home page. Move products higher only if your traffic already knows what it wants.
- **Four to seven sections.** Fewer feels unfinished; more turns the home page into a scroll nobody reaches the end of.
- **Replace every default string before publishing.** The headings and sample paragraphs that ship with the sections read as sample text to a shopper.
- **Don't put Recently viewed here.** A first-time visitor has no history, so the section renders nothing; a returning one is shown their own past before anything new.
- **Set the Journal articles when you publish.** They are chosen by hand and stay chosen until you change them.
- **Turn the popup on deliberately.** A popup that covers the hero seconds into a first visit costs attention. If you use it, give shoppers a real reason to sign up, such as a first-order discount.

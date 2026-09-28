---
title: Newsletter popup
layout: default
parent: Sections
nav_order: 5
permalink: /sections/newsletter-popup/
---

# Newsletter popup

**Newsletter popup** is the overlay version of the email signup. Once switched on, it opens once per visitor, after a delay or a scroll, whichever happens first, and never on page load.

**It is off by default.** A popup that covers the page a few seconds into a first visit costs as much attention as it earns, so the theme leaves the decision to you.

The popup is part of the theme's layout rather than of any one template, so its settings are the same on every page. You select it from the section list in the theme editor sidebar; it is never offered under **Add section**, and it can't be removed or moved. Addresses collected land in `Shopify admin > Customers`, marked as accepting marketing.

It shows only to visitors who are **logged out** and who **haven't dismissed it in this browser**. Signed-in customers never see it.

## Settings

- **Show popup.** The master switch. Default: off. Every other setting appears once it is on.

### Content

- **Image.** Shown at the top of the popup. Alt text is read from the image asset itself.
- **Black and white image.** Renders the image in grayscale. Default: on.
- **Heading.** Default: `Sign up`.
- **Subheading.** Default: `Be the first to know about new arrivals and store news.`
- **Email field placeholder.** Default: `Email`.
- **Button text.** Default: `Subscribe`.
- **Decline link text.** Default: `No thanks`.

### Behavior

- **Open after delay.** Seconds before the popup opens. Range: 0 to 60 s. Default: 5 s.
- **Open after scroll.** Percentage of the page scrolled before it opens. Range: 0% to 100% in 5% steps. Default: 50%. Set to 0 to use the delay only.

Whichever of the two happens first opens the popup. It also waits while the shopper is busy: it won't open over the cart drawer, the navigation panel or the filters, or while the shopper is typing in a field.

### Consent

- **Show consent checkbox.** Default: off. Recommended for EU markets under GDPR. Without the checkbox, consent is recorded when the form is submitted.
- **Consent text.** Inline rich text, and it may contain links. Ships pointing at `/policies/privacy-policy`. Shown when the consent checkbox is on.

The popup takes its colors from [Popovers and drawers](../../theme-settings/popovers/) in theme settings, like the theme's other overlays.

## Tips

- **Decide whether you want it at all.** A popup suits a store with a real reason to sign up, such as early access or a restock list. Without one, the in-page [Newsletter](../newsletter/) section collects addresses without interrupting anyone.
- **Don't set the delay too low.** Under about three seconds the popup lands before the shopper has seen anything worth signing up for.
- **Scroll is the better trigger of the two.** A shopper who has scrolled halfway down has shown interest; one who has waited five seconds has only been slow.
- **Turn the consent checkbox on for EU markets.** It is off by default because it isn't required everywhere; if you sell into the EU, treat it as required.
- **Dismissal is per browser.** Testing it repeatedly means clearing site data, or using a private window, each time.

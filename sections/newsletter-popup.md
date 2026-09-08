---
title: Newsletter popup
layout: default
parent: Sections
nav_order: 11
permalink: /sections/newsletter-popup/
---

# Newsletter popup

**Newsletter popup** is the overlay version of the email signup. It opens once per visitor, after a delay or a scroll, whichever happens first, and never on page load.

It shows only to visitors who are **logged out** and who **haven't dismissed it in this browser**. Signed-in customers never see it.

## Settings

- **Show popup.** The master switch. Default: on.

### Content

- **Image.** Shown at the top of the popup. Alt text is read from the image asset itself.
- **Black and white image.** Renders the image in greyscale. Default: on.
- **Heading.** Default: `Sign up`.
- **Subheading.** Default: `Be the first to know about new arrivals and store news.`
- **Email field placeholder.** Default: `Email`.
- **Button text.** Default: `Subscribe`.
- **Decline link text.** Default: `No thanks`.

### Behavior

- **Open after delay.** Seconds before the popup opens. Range: 0 to 60 s. Default: 5 s.
- **Open after scroll.** Percentage of the page scrolled before it opens. Range: 0% to 100% in 5% steps. Default: 50%. Set to 0 to use the delay only.

Whichever of the two happens first opens the popup.

### Consent

- **Show consent checkbox.** Default: off. Recommended for EU markets under GDPR. Without the checkbox, consent is recorded when the form is submitted.
- **Consent text.** Inline rich text, and it may contain links. Ships pointing at `/policies/privacy-policy`.

### Colors

- **Color scheme.** Default: scheme-1.

## Tips

- **Don't set the delay too low.** Under about three seconds the popup lands before the shopper has seen anything worth signing up for.
- **Scroll is the better trigger of the two.** A shopper who has scrolled halfway down has shown interest; one who has waited five seconds has only been slow.
- **Turn the consent checkbox on for EU markets.** It is off by default because it isn't required everywhere; if you sell into the EU, treat it as required.
- **Dismissal is per browser.** Testing it repeatedly means clearing site data, or using a private window, each time.
- **You can run both signups.** The popup catches the visitor who was going to leave; the [Newsletter](../newsletter/) section catches the one who read to the end of the page.

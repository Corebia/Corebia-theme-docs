---
title: Contact page
layout: default
parent: Templates
nav_order: 11
permalink: /templates/contact-page/
---

# Contact page

An alternate page template, `page.contact.json`, using the **Contact form** section: a form on one side, your contact details on the other.

To use it, create a page in `Shopify admin > Content > Pages` and set its **Theme template** to `contact`.

## Section settings

### Header

- **Show subheading** — Default: on.
- **Subheading** — Default: `Get in touch`.
- **Show description** — Default: on.
- **Description** — Default: `We'd love to hear from you. Send us a message and we'll respond as soon as possible.`

### Contact details

The panel beside the form. Each line can be hidden.

- **Show email** — Default: on.
- **Email address** — Default: `hello@yourstore.com`. **Change this before launch.**
- **Email label** — Default: `Email`.
- **Show location** — Default: on.
- **Location** — Default: `City, Country`. **Change this before launch.**
- **Location label** — Default: `Location`.
- **Phone number (display)** — A clickable phone number in the info panel. Leave blank to hide.
- **Show response time** — Default: on.
- **Response time** — Empty by default. For example, `Within 2 business days`.
- **Response time label** — Default: `Response time`.
- **Show trust message** — Default: on.
- **Trust message** — Shown below the contact details. Leave blank to hide.

### Form

- **Show phone field** — Default: on.
- **Phone field label** — Default: `Phone`.
- **Subject options** — One option per line. The form shows a Subject dropdown built from these. Leave blank to hide the dropdown. Defaults: General inquiry, Order support, Press and media, Wholesale, Careers.
- **Privacy reassurance** — Small text below the submit button. Leave blank to hide.

### Colors

- **Color scheme** — Default: scheme-1.

## Where messages go

Submissions arrive by email at the address in `Shopify admin > Settings > Store details > Sender email`, not at the address shown on the page. Those are two different things, and it is worth checking the first one actually reaches someone.

The form is protected by Shopify's own spam check, which can ask a shopper to confirm they're human before the message sends.

## Tips

- **Replace the placeholder details.** `hello@yourstore.com` and `City, Country` ship as examples and will go live if you leave them.
- **Only promise a response time you can keep.** An unanswered promise on the contact page generates more mail, not less.
- **Trim the subject options** to the ones you actually route differently. Five choices where two would do makes the form feel longer than it is.
- **Some markets require a business address** on the storefront. If yours does, the location line here and a Contact block in the [Footer](../../sections/footer/) are the two conventional places for it.

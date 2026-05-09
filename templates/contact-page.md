---
title: Contact page
layout: default
parent: Templates
nav_order: 11
permalink: /templates/contact-page/
---

# Contact page

The **Contact page** is a dedicated template for a contact form. It uses the `page.contact.json` template, an alternate page template that combines a form with brand contact details.

## URL

Whichever page you create with the contact template assigned. The conventional URL is `/pages/contact`.

## Sections included by default

1. **Contact form** — The contact form section with form fields and brand details.

## Contact form section

### Header

- **Show subtitle** — Toggle the small uppercase text above the heading.
- **Subtitle** — Default: `GET IN TOUCH`.
- **Show description** — Toggle the description paragraph.
- **Description** — Default: `We'd love to hear from you. Send us a message and we'll respond as soon as possible.`

### Contact details

A side panel with brand contact information.

- **Show email** — Toggle.
- **Email address** — Default: `hello@yourstore.com`.
- **Email label** — Default: `Email`.
- **Show location** — Toggle.
- **Location** — Default: `New York, NY`.
- **Location label** — Default: `Location`.
- **Phone number (display)** — Clickable phone number shown in the info panel. Leave blank to hide.
- **Show response time** — Toggle.
- **Response time** — Default: `Within 24 hours`.
- **Response time label** — Default: `Response time`.
- **Show trust message** — Toggle.
- **Trust message** — Shown below the contact details to build trust. Default: `Every message is read and responded to personally — we value your time.`

### Form

- **Show phone field** — Adds a phone field to the form. Toggle.
- **Phone field label** — Default: `Phone`.
- **Subject options** — One option per line. The form will show a Subject dropdown using these. Leave blank to hide the dropdown. Default:
  ```
  General inquiry
  Order support
  Press and media
  Wholesale
  Careers
  ```
- **Privacy reassurance** — Shown as small text below the submit button. Leave blank to hide. Default: `We respect your privacy. Your information will not be shared.`

### Colors

- **Color scheme** — Default: scheme-2.

## How submissions work

The form posts to Shopify's built-in contact endpoint. Submissions are sent as emails to the **Sender email** configured in `Shopify admin > Settings > Notifications > Sender email`.

If you want submissions to go to a different inbox, change the **Customer email** in your store settings, or install a third-party form app.

## Setting up the contact page

1. In `Shopify admin > Online Store > Pages`, create a new page titled "Contact".
2. Under **Theme template**, choose **page.contact**.
3. Save.
4. Open the theme editor and customize the contact form section's settings.
5. Add a link to the contact page from your main menu and footer menu.

## Sections that can be added

In addition to **Contact form**, you can add any of these sections:

- [FAQ](../../sections/faq/)
- [Brand image](../../sections/brand-image/)
- [Brand message](../../sections/brand-message/)
- [Rich text with image](../../sections/rich-text-image/)
- [Newsletter](../../sections/newsletter/)
- [Custom Liquid](../../sections/custom-liquid/)

## Tips

- **Update the placeholder details** — `hello@yourstore.com` and `New York, NY` are placeholders; customers will not trust contact details that look like demo content.
- **Set realistic response times.** A "Within 24 hours" promise that you don't keep is worse than no promise.
- **Phone number** — Only show if you actually answer it. A phone number that goes to voicemail erodes trust.
- **Subject options** — Cap at 4–6 options. Long lists feel overwhelming.

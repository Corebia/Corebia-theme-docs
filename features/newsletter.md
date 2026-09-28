---
title: Newsletter
layout: default
parent: Features
nav_order: 14
permalink: /features/newsletter/
---

# Newsletter

Pave's newsletter signup is a simple email form that creates a customer record in your Shopify admin, marked as accepting email marketing.

## Where it appears

Pave offers several ways to collect an address, and they can all run at once:

- The [Newsletter section](../../sections/newsletter/), in the page flow. Out of the box it sits in the footer group, just above the footer, so it appears once on every page. It can also be added to any template.
- The **Email signup** block in the [Footer](../../sections/footer/), a compact field inside one of the footer columns.
- The [Newsletter popup](../../sections/newsletter-popup/), an overlay that opens once per visitor after a delay or a scroll. It is **off by default**: turn on **Show popup** in the popup's settings to use it. It never shows to a signed-in customer, and never to someone who has dismissed it in that browser.
- The [Password page](../../templates/password-page/), when **Show email signup form** is on. A pre-launch list is often the most valuable one a store builds.
- The [Drop](../../sections/drop/) section, which collects a waitlist before a launch date.

All of them write to the same place.

## Why the popup starts off

A popup that opens a few seconds into every first visit covers the page before the visitor has seen it. Pave leaves it off so a new store doesn't greet everyone with an overlay. If you want one, turn it on, and consider a longer delay or a scroll trigger so it opens once the visitor is already reading.

## Consent

The section and the popup both offer a **Show consent checkbox** setting, with editable consent text that can carry a link to your privacy policy. It is on by default in the section and off in the popup. The footer's Email signup block has no checkbox.

If you sell into the EU, turn it on in both, and consider whether the footer block suits your consent policy. Without the checkbox, consent is recorded on submission rather than given explicitly.

## Where signups go

Submissions create a customer record in `Shopify admin > Customers`. Each form adds a tag so you can tell the lists apart: `newsletter` for the section, the footer block and the popup, `password-page` for the password page, and the tag you choose for a drop's waitlist. From there, you can:

- Send campaigns from `Shopify admin > Marketing` using the **Shopify Email** app.
- Sync to a third-party tool. Apps like **Klaviyo**, **Mailchimp**, **Drip** or **Omnisend** read the customer list from Shopify and handle the email sending. Install the app from the Shopify App Store and follow its setup.

## What the form captures

- Email address (required).
- The customer's marketing consent.

The form does not capture a name, phone number or other fields. If you need richer signup data, use a third-party form app (Klaviyo, Mailchimp and so on) instead.

## Tips

- **Honor your offer.** If your subtext promises a 10% discount on a first order, send a welcome email with the code. Customers who don't get the promised discount unsubscribe at high rates.
- **Confirm subscriptions.** Many email tools support double opt-in, where the customer clicks a link in a welcome email to confirm. It helps deliverability and GDPR compliance.
- **One signup per screen is enough.** The section above the footer and a footer Email signup block show two forms a few inches apart. Pick one.
- **GDPR and privacy.** In the EU, make sure your form copy and privacy policy meet GDPR consent requirements. Customer and marketing email settings live in `Shopify admin > Settings > Customer accounts` and `Settings > Notifications`.

## Troubleshooting

- **The popup never opens.** Check **Show popup** is on in the Newsletter popup settings, then test in a private window while signed out. Once dismissed, it stays closed in that browser.
- **Submitting the form does nothing.** Confirm the email is valid (some browsers' autofill inserts non-email values). Check the browser console for errors and confirm Shopify customer creation isn't blocked.
- **Customer doesn't appear in admin.** Submissions take a moment to show up. Refresh the admin customer list.
- **Welcome email doesn't go out.** Welcome emails are configured by your email tool (Shopify Email, Klaviyo and so on). Configure the welcome flow in that tool, not the theme.

## Related

- [Newsletter section reference](../../sections/newsletter/)
- [Newsletter popup reference](../../sections/newsletter-popup/)
- [Password page template reference](../../templates/password-page/)

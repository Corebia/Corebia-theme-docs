---
title: Newsletter
layout: default
parent: Features
nav_order: 14
permalink: /features/newsletter/
---

# Newsletter

Pave's newsletter signup is a simple email form that creates a customer record in your Shopify admin tagged as accepting marketing.

## Where it appears

Pave offers three ways to collect an address, and they can all run at once:

- The [Newsletter section](../../sections/newsletter/), in the page flow, on the home page by default. Add it to any template except the header group.
- The [Newsletter popup](../../sections/newsletter-popup/), an overlay that opens once per visitor after a delay or a scroll. It never shows to a signed-in customer, and never to someone who has dismissed it in that browser.
- The [Password page](../../templates/password-page/), when **Show email signup form** is on. A pre-launch list is often the most valuable one a store builds.

All three write to the same place.

## Consent

Both the section and the popup offer a **Show consent checkbox** setting, with editable consent text that can carry a link to your privacy policy. It is on by default in the section and off in the popup.

If you sell into the EU, turn it on in both. Without the checkbox, consent is recorded on submission rather than given explicitly.

## Where signups go

Submissions create a customer record in `Shopify admin > Customers` tagged as accepting email marketing. From there, you can:

- Send campaigns from `Shopify admin > Marketing` using the **Shopify Email** app.
- Sync to a third-party tool. Apps like **Klaviyo**, **Mailchimp**, **Drip**, or **Omnisend** read the customer list from Shopify and handle the email sending. Install the relevant app from the Shopify App Store and follow its setup.

## What the form captures

- Email address (required).
- The customer's marketing consent (when they submit, they are tagged as accepting marketing).

The form does not capture name, phone, or other fields. If you need richer signup data, replace the section with a third-party form app (Klaviyo, Mailchimp, etc.).

## Tips

- **Honor your offer.** If your subtext promises a 10% discount on first order, send a welcome email with the discount code. Customers who don't get the promised discount unsubscribe at high rates.
- **Confirm subscriptions.** Many email tools support double opt-in (customer must click a confirmation link in their welcome email). Recommended for deliverability and GDPR compliance.
- **GDPR / privacy.** In the EU, ensure your form copy and privacy policy meet GDPR consent requirements. Configure customer accounts and email marketing settings in `Shopify admin > Settings > Customer accounts` and `Settings > Notifications`.

## Troubleshooting

- **Submitting the form does nothing.** Confirm the email is valid (some browsers' autofill inserts non-email values). Check the browser console for errors and confirm Shopify customer-creation isn't blocked.
- **Customer doesn't appear in admin.** Submissions take a moment to show up. Refresh the admin customer list. If still missing, confirm the section's form posts are reaching Shopify (check the network panel in dev tools).
- **Welcome email doesn't go out.** Welcome emails are configured by your email tool (Shopify Email, Klaviyo, etc.). Configure the welcome flow in that tool, not the theme.

## Related

- [Newsletter section reference](../../sections/newsletter/)
- [Password page template reference](../../templates/password-page/)

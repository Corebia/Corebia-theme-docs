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

- The [Newsletter section](../../sections/newsletter/) — placed by default on the home page, page template, and several other places.
- The [Password page](../../templates/password-page/) — when **Show email signup form** is enabled.

## Where signups go

Submissions create a customer record in `Shopify admin > Customers` tagged as accepting email marketing. From there, you can:

- Send campaigns from `Shopify admin > Marketing` using the **Shopify Email** app.
- Sync to a third-party tool. Apps like **Klaviyo**, **Mailchimp**, **Drip**, or **Omnisend** read the customer list from Shopify and handle the email sending. Install the relevant app from the Shopify App Store and follow its setup.

## What the form captures

- Email address (required).
- The customer's marketing consent (when they submit, they are tagged as accepting marketing).

The form does not capture name, phone, or other fields. If you need richer signup data, replace the section with a third-party form app (Klaviyo, Mailchimp, etc.).

## Tips

- **Honor your offer** — If your subtext promises a 10% discount on first order, send a welcome email with the discount code. Customers who don't get the promised discount unsubscribe at high rates.
- **Confirm subscriptions** — Many email tools support double opt-in (customer must click a confirmation link in their welcome email). Recommended for deliverability and GDPR compliance.
- **GDPR / privacy** — In the EU, ensure your form copy and privacy policy meet GDPR consent requirements. Configure customer accounts and email marketing settings in `Shopify admin > Settings > Customer accounts` and `Settings > Notifications`.

## Troubleshooting

- **Submitting the form does nothing** — Confirm the email is valid (some browsers' autofill inserts non-email values). Check the browser console for errors and confirm Shopify customer-creation isn't blocked.
- **Customer doesn't appear in admin** — Submissions take a moment to show up. Refresh the admin customer list. If still missing, confirm the section's form posts are reaching Shopify (check the network panel in dev tools).
- **Welcome email doesn't go out** — Welcome emails are configured by your email tool (Shopify Email, Klaviyo, etc.). Configure the welcome flow in that tool, not the theme.

## Related

- [Newsletter section reference](../../sections/newsletter/)
- [Password page template reference](../../templates/password-page/)

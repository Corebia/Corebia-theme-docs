---
title: Newsletter
layout: default
parent: Sections
nav_order: 9
permalink: /sections/newsletter/
---

# Newsletter

The **Newsletter** section displays an email signup form. Submissions create a customer record in your Shopify admin tagged as accepting marketing.

## Settings

- **Heading** — The section heading. Default: `Subscribe to the newsletter`.
- **Subtext** — Supporting text shown below the heading. Default: `Subscribe for exclusive offers and 10% off your first order.`
- **Social proof text** — Small text shown below the form. Leave blank to hide. Default: `Join our community`.
- **Color scheme** — The color scheme applied to the section. Default: scheme-2.

## Where signups go

Newsletter signups are stored as customers in `Shopify admin > Customers`. They are automatically tagged as accepting email marketing. From there, you can:

- Send campaigns from `Shopify admin > Marketing` using the **Shopify Email** app.
- Sync to a third-party marketing platform (Klaviyo, Mailchimp, etc.) by installing the appropriate Shopify app, which will pull the same customer list.

Pave does not integrate directly with third-party email tools. The form posts to Shopify, and apps that subscribe to customer events handle the rest.

## Tips

- **Be honest in the offer.** If your subtext promises 10% off, send the discount code in the welcome email. Customers who don't receive the promised discount unsubscribe at high rates.
- **Keep the subtext short.** Two short sentences work; long marketing copy hurts conversion.
- **Social proof text** is optional. Use it for a follower count (`Join 12,000+ subscribers`) only if the number is real and impressive.
- **GDPR / privacy compliance** — If you operate in the EU, configure customer accounts and email marketing settings in `Shopify admin > Settings > Customer accounts` and `Settings > Notifications` to ensure the signup language is compliant.

## Related

- For the dedicated [Newsletter feature](../../features/newsletter/) overview.

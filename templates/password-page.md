---
title: Password page
layout: default
parent: Templates
nav_order: 14
permalink: /templates/password-page/
---

# Password page

The **Password page** is shown to visitors when your store is password-protected (in `Shopify admin > Online Store > Preferences > Password protection`). It uses the `password.json` template.

The password page is its own self-contained layout — it does not show the storefront header, footer, or navigation. Customers who enter the correct password are redirected to your store.

## URL

When password protection is enabled, every URL on the storefront redirects to the password page until the password is entered. After entering the correct password, the customer accesses the storefront normally.

## Sections included by default

1. **Password page** — The full password page with branding, message, optional countdown, and email signup.

## Password page section

### Branding

- **Show logo** — Display your shop logo above the headline. Reads from **Theme settings > Logo**.

### Content

- **Headline** — The main heading. Default: `Opening Soon`.
- **Message** — The supporting message. Default: `We're putting the finishing touches on something new. Enter the password below for early access.`

### Countdown

A live countdown to your launch date. Leave the date blank to hide the countdown.

- **Launch date** — Format: `YYYY-MM-DD` (e.g. `2026-06-01`). Leave blank to hide the countdown.
- **Launch time** — Format: `HH:MM` in 24-hour time (e.g. `09:00`). Used together with the date and timezone.
- **Timezone** — The timezone in which the launch date and time are interpreted.

### Email signup

- **Show email signup form** — Toggle.
- **Signup prompt text** — Default: `Be the first to know when we launch`.

### Background

- **Background image** — Recommended: `1920 by 1080 px` or larger. A gradient overlay is applied automatically.

### Other

- **Color scheme** — Default: scheme-3.

## Special behaviors

- **Password input** — Always present at the bottom of the page; this is the access mechanism. The password itself is configured in `Shopify admin > Online Store > Preferences > Password protection`.
- **Email signups** — When enabled, captured emails go to your customer database tagged as accepting marketing, just like the normal newsletter signup.
- **Auto-launch** — When the countdown reaches zero, nothing technically happens — you must still toggle off password protection in your admin to make the store live. The countdown is informational.

## Setting up password protection

1. In `Shopify admin > Online Store > Preferences`, scroll to **Password protection**.
2. Enable **Restrict access to visitors with the password**.
3. Set the password and the message that appears on the password page (this Shopify-level message is separate from the **Message** in this section, which has priority).
4. Save.

## Tips

- **Use a striking background image.** This is a brand moment — every visitor sees this page until you go live.
- **Set a real launch date.** A countdown to a credible date builds anticipation. A vague "Coming soon" is less engaging.
- **Capture emails.** A pre-launch email list is the highest-value marketing asset for a soft-launch. Enable the email signup.
- **Test the page** at the password URL before going live to make sure all settings render correctly.

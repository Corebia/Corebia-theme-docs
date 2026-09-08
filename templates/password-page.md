---
title: Password page
layout: default
parent: Templates
nav_order: 14
permalink: /templates/password-page/
---

# Password page

What visitors see while the store is password-protected. It uses the **Password page** section, which can carry a countdown to launch and an email signup — so the wait can collect an audience rather than just block one.

Turn password protection on and off under `Shopify admin > Online Store > Preferences`, at the bottom.

## Section settings

- **Color scheme** — Default: scheme-1.

### Branding

- **Show logo** — Uses the logo from [Logo](../../theme-settings/logo/). Default: on. With no logo uploaded it falls back to the shop name.

### Content

- **Heading** — Default: `Opening soon`.
- **Message** — Default: `We're putting the finishing touches on something new. Enter the password below for early access.`

### Countdown

- **Launch date** — Format: `YYYY-MM-DD`, for example `2026-06-01`. Leave blank to hide the countdown.
- **Launch time** — Format: `HH:MM` in 24-hour time, for example `09:00`. Used together with the date and timezone. Default: `00:00`.
- **Timezone** — The timezone the launch date and time are read in. Default: UTC. The list covers major zones from Auckland to Los Angeles.

### Email signup

- **Show email signup form** — Default: off.
- **Signup prompt text** — Default: `Be the first to know when we launch`.

### Background

- **Background image** — 1920 x 1080px recommended. A gradient overlay is applied automatically.

## The password itself

Set under `Shopify admin > Online Store > Preferences`, not in the theme. The page always shows the entry field; these settings control everything around it.

## Where signups go

Addresses collected here land in `Shopify admin > Customers`, tagged as accepting marketing — the same place the [Newsletter](../../sections/newsletter/) section sends them. A pre-launch list is usually the most valuable one a store ever builds, so it is worth turning the form on even for a short closed period.

## Tips

- **Set the timezone.** It defaults to UTC, which is the wrong local hour almost everywhere. A countdown that hits zero at the wrong time is worse than none.
- **Turn the countdown off unless the date is firm.** A countdown that expires with the store still closed reads badly.
- **Use one strong image.** This page is one screen with no scrolling; it is the whole first impression.
- **Preview it while logged out.** Signed in to your admin you bypass the password, so use a private window to see what visitors see.

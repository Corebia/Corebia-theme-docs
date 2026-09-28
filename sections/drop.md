---
title: Drop
layout: default
parent: Sections
nav_order: 33
permalink: /sections/drop/
---

# Drop

**Drop** runs a product launch on a date and time you set. Before the launch it shows a countdown and a waitlist signup; at the launch moment it switches by itself to what you want shoppers to see once the drop is live, with links to the product and the collection. No one has to be at a keyboard when it happens.

The theme ships a page template built around it, `page.drop`. See [Alternate page templates](../../templates/page-templates/#drop).

It can't be placed in the header or footer groups.

## Settings

### Drop date

- **Date.** Written as `YYYY-MM-DD`, for example `2026-12-31`. Left blank, the section shows the live content.
- **Time.** Written as `HH:MM` in 24-hour time, for example `18:00`. Blank is midnight. Default: `00:00`.
- **Timezone.** The timezone the date and time are in. **UTC** (default), or one of 28 cities: **London (GMT/BST)**, **Paris (CET/CEST)**, **Berlin (CET/CEST)**, **Madrid (CET/CEST)**, **Athens (EET/EEST)**, **Moscow (MSK)**, **Cairo (EET)**, **Johannesburg (SAST)**, **Dubai (GST)**, **Mumbai (IST)**, **Singapore (SGT)**, **Hong Kong (HKT)**, **Shanghai (CST)**, **Tokyo (JST)**, **Seoul (KST)**, **Perth (AWST)**, **Sydney (AEST/AEDT)**, **Auckland (NZST/NZDT)**, **Anchorage (AKST/AKDT)**, **Los Angeles (PST/PDT)**, **Denver (MST/MDT)**, **Chicago (CST/CDT)**, **New York (EST/EDT)**, **Toronto (EST/EDT)**, **Mexico City (CST/CDT)**, **Bogotá (COT)**, **São Paulo (BRT)** or **Buenos Aires (ART)**.

### Before the drop

- **Heading.** Default: `Coming soon`.
- **Text.** Rich text under the heading.
- **Waitlist tag.** Added to each customer who joins the waitlist. Default: `drop`.

### Once live

- **Heading.** Default: `Out now`.
- **Text.** Rich text under the heading.
- **Product.** Adds a button to this product, labeled `Shop` and the product's title.
- **Collection.** Adds a second button, to this collection, labeled the same way.
- **Image.** Shown beside the content, both before and after the launch.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 60 px each.

## Before and after the launch

**Before**, the section shows the before heading and text, a countdown in days, hours, minutes and seconds with a pause button, and an email field with a **Join the waitlist** button.

**At the launch moment**, the page switches to the live heading, text and buttons without a reload, even for a shopper who has had it open all along.

**After**, anyone arriving sees the live content straight away. If you left every live setting empty, the section disappears at the launch moment instead.

## The waitlist

The signup creates a customer in Shopify admin, subscribed to email marketing and tagged with the **Waitlist tag**. To email them when the drop goes live, filter customers by that tag in `Shopify admin > Customers`, or build a segment on it in Shopify Email or your email app.

Use a different tag for each drop, such as `drop-autumn`, so each launch has its own list.

## A note on daylight saving time

Liquid can't read a timezone's current offset, so the page served from Shopify decides "before" or "live" using each zone's standard time. Where daylight saving time is in effect, a page loaded in the hour after the launch can still arrive showing the countdown. The shopper's browser then switches it to live at once, so nobody waits. It is never early.

## Tips

- **Check the date format.** A date that isn't a real `YYYY-MM-DD` (and `HH:MM`) is treated as no date, and the section shows the live content straight away.
- **Fill in the live settings before launch day.** The switch is automatic, so what you set in **Once live** is what shoppers see the moment the countdown ends.
- **Keep the product unavailable until launch.** The section changes what the page says, not whether the product can be bought. Publish the product to your online store at the launch time, or keep it hidden until then.
- **Use the same image before and after.** It carries the launch across the switch, so the page doesn't feel like it changed under the shopper.

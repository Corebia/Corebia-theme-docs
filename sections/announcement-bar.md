---
title: Announcement bar
layout: default
parent: Sections
nav_order: 3
permalink: /sections/announcement-bar/
---

# Announcement bar

The **Announcement bar** is the slim strip above the header. It carries up to five messages, each of which can optionally run a countdown or hand the shopper a discount code to copy.

It belongs to the `header` section group, so it can only be placed above or below the header — not in the middle of a page.

## Settings

- **Color scheme** — Default: scheme-2, so the bar reads as a band against the page rather than blending into it.
- **Motion** — How messages animate. Default: **Rotate**.
  - **Rotate (cross-fade between messages)** — One message at a time, cross-fading to the next.
  - **Marquee (continuous horizontal scroll)** — All messages scrolling horizontally in a continuous loop.
- **Rotation interval** — How long each message shows before the next rotates in. Range: 3000 to 9500 ms in 500 ms steps. Default: 5000 ms. Only used when there are two or more messages, and only in Rotate mode.
- **Marquee speed** — **Slow**, **Medium** or **Fast**. Default: Slow. Slow keeps the bar editorial; fast competes with the page below.
- **Marquee gap** — Spacing between messages, and between the end of the sequence and its repeat. **Compact**, **Standard** or **Spacious**. Default: Standard.
- **Pause on hover** — Halts motion while the shopper's pointer or keyboard focus is inside the bar. Default: on.

## Blocks

Up to **five** Message blocks. Every field below the first two is optional, and a message that uses none of them is just a line of text.

### Message

- **Text** — Inline rich text. Default: `Free shipping on all orders over $50`.
- **Link** — Optional. Wraps the text in an anchor.

#### Countdown

- **Countdown end date and time** — When the countdown ends, written as `2026-12-31T23:59:59-08:00`, where the last part is your timezone's offset from Greenwich Mean Time. Without an offset the time is read as Greenwich Mean Time. Leave blank to hide the countdown.
- **Countdown format** — **Days : Hours : Minutes : Seconds** (default), **Hours : Minutes : Seconds**, **Minutes : Seconds**, or **Days only**.
- **Countdown prefix label** — Optional text before the digits. Defaults to `Sale ends in` when blank.
- **When the countdown reaches zero** — **Remove this block from the bar** (default) or **Show an expired message in this block**.
- **Expired message** — Defaults to `This offer has ended.` when blank.

#### Discount code

- **Promo code** — The code shoppers will copy, for example `SAVE20`. Leave blank to omit the promo.
- **Promo label prefix** — Optional. Defaults to `Use code` when blank.
- **Copy confirmation text** — The toast shown after a successful copy. Defaults to `Copied` when blank.

## Tips

- **Keep each message short.** The bar is one line on mobile, and a long message either truncates or forces the marquee to do the reading for you.
- **Pick motion to match the number of messages.** One message doesn't need motion at all. Two or three suit Rotate. Five short messages are what Marquee is for.
- **Set the timezone offset on countdowns.** Without the offset the deadline is read as Greenwich Mean Time, which will end your sale at the wrong local hour.
- **Decide what happens at zero before you launch.** Removing the block is the safe default; showing an expired message only makes sense if the message itself is worth reading afterwards.
- **The discount code still has to exist in Shopify.** Copying the code doesn't create it — set it up under `Shopify admin > Discounts` first, and see [Discount codes](../../features/discounts/).

---
title: Theme blocks
layout: default
parent: Sections
nav_order: 51
permalink: /sections/theme-blocks/
---

# Theme blocks

Theme blocks are the small building pieces, such as a heading, a button or an image, that several sections share. They work the same wherever they appear, so what you learn about a Button block in one section holds in every other.

## Where they can be used

- **[Section](../section/)** and **[Media with content](../media-with-content/)** accept every theme block below, plus app blocks.
- **[Group](#group)**, itself a theme block, accepts every theme block and app blocks, so groups can be nested inside groups.
- **[Slideshow](../slideshow/)** slides take Heading, Text and Button.
- **[Rich text with image](../rich-text-image/)** takes Heading, Text and Button.
- **[Hero banner](../hero/)** takes Button.
- **Custom Liquid** is also available as a block in [Customer reviews](../customer-reviews/), [Featured product](../featured-product/) and the main section of most [templates](../../templates/).

The [Divider](#divider) is only offered inside Section and Group.

## Button

A link styled as one of the theme's buttons. A button with no label is not shown.

- **Label.** The button text. A new button starts with `Learn more`.
- **Link.** Where it goes.
- **Style.** **Primary** (default), the filled button, or **Secondary**, the outlined one. Both follow **Theme settings > Buttons**.

## Comparison slider

Two images in one frame, split by a handle the shopper drags to compare them: before and after, two colors, day and night. The handle also works with the arrow, Home and End keys.

- **Before image** / **After image.** Without an image, a placeholder shows in its place.
- **Before label** / **After label.** Short captions on each side. Defaults: `Before` and `After`. Leave one empty to hide it.
- **Starting position.** Where the handle sits when the page loads, measured from the left edge. At 0% the after image shows in full. Range: 0% to 100% in 1% steps. Default: 50%.
- **Aspect ratio.** **Adapt to before image** (default), **Landscape (16:9)**, **Standard (4:3)**, **Square (1:1)** or **Portrait (4:5)**.

Use two images of the same size and framing. Anything that moves between them other than the change you are showing makes the comparison hard to read.

## Countdown

A timer counting down to a date and time you set, in days, hours, minutes and seconds. Shoppers can pause the ticking digits.

- **End date.** Written as YYYY-MM-DD, for example `2026-12-31`. Leave blank to hide the countdown. A date that doesn't exist or isn't written in that form also hides it, and the theme editor shows a hint.
- **End time.** Written as HH:MM in 24-hour time, for example `18:00`. Default: `00:00`. Blank is midnight.
- **Timezone.** The timezone of the end date and time. Default: **UTC**. The other options are 28 cities across the world's timezones, such as **London (GMT/BST)**, **New York (EST/EDT)** and **Tokyo (JST)**.

### Labels

- **Days** / **Hours** / **Minutes** / **Seconds.** The words under each number. When blank, they read Days, Hours, Minutes and Seconds in the store's language.

### When the countdown ends

- **At the end.** **Hide the countdown** (default) or **Show a message**.
- **Message.** Shown when At the end is set to Show a message. Defaults to "This offer has ended." when blank.

## Custom Liquid

- **Liquid code.** Add app snippets or custom code. Invalid Liquid can break the page, so test it on a [duplicate theme](../../customization/duplicating-your-theme/) first. See [Custom Liquid](../custom-liquid/) for what it can and can't do; the same guidance applies to the block.

## Divider

A horizontal rule between blocks. Only available inside Section and Group.

- **Thickness.** Range: 1 to 8 px in 1 px steps. Default: 1 px.
- **Color.** Leave empty to use the color scheme's border color.
- **Width.** How much of the available width the line spans. Range: 10% to 100% in 5% steps. Default: 100%.

## Group

A container that arranges the blocks inside it in a column or a row. Groups are how Section builds columns, rows of logos and side-by-side content.

- **Direction.** **Vertical** (default) stacks the blocks; **Horizontal** puts them side by side.
- **Alignment.** Shown for a vertical group. **Full width** (default), **Left**, **Center** or **Right**.
- **Horizontal alignment.** Shown for a horizontal group. **Left** (default), **Center**, **Right** or **Space between**.
- **Vertical alignment.** Shown for a horizontal group. **Top**, **Middle** (default) or **Bottom**.
- **Gap.** Space between the blocks inside. Range: 0 to 100 px in 4 px steps. Default: 16 px.
- **Width.** **Fit content** (default) or **Fill**. In a horizontal group, groups set to Fill share the width equally and stack on narrow screens.

## Heading

- **Heading.** Default: `Our story`. It is marked up as a second-level heading, and the section it sits in sets its size.

## Icon

A small decorative icon, usually placed above a heading and text. It is hidden from screen readers, so the text beside it should say what it means.

- **Icon.** **Truck (shipping)** (default), **Shield (security)**, **Lock (secure payment)**, **Leaf (sustainability)**, **Package**, **Refresh (returns)**, **Heart**, **Star**, **Check (guarantee)**, **Clock (fast)** or **Credit card**.
- **Image.** Replaces the icon when set, for a mark of your own.
- **Width.** Range: 16 to 96 px in 4 px steps. Default: 32 px.

## Image

- **Image.** Without one, a placeholder illustration shows. The crop follows the focal point set on the image in the image picker. Set the image's alt text in **Content > Files** so screen readers can describe it.

## Jumbo text

Text sized to fill the full width of its container, however long it is. A short word becomes very large; a long line stays within the width.

- **Text.** Default: `Made to last`.
- **Alignment.** **Left** (default), **Center** or **Right**.
- **Case.** **As typed** (default) or **Uppercase**.

## Spacer

Empty space between blocks, for when the group's gap isn't enough.

- **Size.** **Pixels** (default) or **Percentage**. Percentage sizes take effect in horizontal groups.
- **Size.** The amount of space, in the unit chosen above. Pixels: 0 to 200 px in 4 px steps, default 32 px. Percentage: 0% to 100% in 1% steps, default 10%.
- **Use a different size on mobile.** Default: off.
- **Mobile size.** Shown when the option above is on, and used below 750 px wide. Pixels: 0 to 200 px in 4 px steps, default 16 px. Percentage: 0% to 100% in 1% steps, default 10%.

## Text

- **Text.** Rich text. It ships with sample copy that is shown to customers on the storefront, so replace it with your own.

## Video

A video with a poster image and a play button. Nothing is loaded from the video host until the video plays.

- **Source.** **Uploaded video** (default) or **YouTube or Vimeo URL**.
- **Video.** Shown for an uploaded video.
- **URL.** Shown for YouTube or Vimeo. Paste the video's page address.
- **Poster image.** Shown until the video plays. Without one, an uploaded video shows its preview image.
- **Play automatically.** Default: off. Plays muted once the page has loaded, with a pause button. Shoppers who ask their device for reduced motion see the poster and a play button instead.
- **Loop.** Default: on.
- **Aspect ratio.** **Landscape (16:9)** (default), **Standard (4:3)**, **Square (1:1)** or **Portrait (9:16)**.

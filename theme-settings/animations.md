---
title: Animations
layout: default
parent: Theme settings
nav_order: 18
permalink: /theme-settings/animations/
---

# Animations

The motion in the storefront: how one page gives way to the next, how product cards respond to the pointer, and how sections arrive as the shopper scrolls.

Every animation here is skipped for shoppers who ask their device for reduced motion. They get the same content, without the movement.

## Settings

- **Page transitions.** Pages fade into each other when a shopper follows a link. Skipped in browsers without support. Default: on.
- **Transition to product page.** The product card image morphs into the product page image when a shopper opens a product. Skipped in browsers without support. Default: on.
- **Card hover effect.** Moves the product card when a shopper points at it or tabs into it. Cards already fade to their second image; this adds to it. Skipped on touch screens. **None** (default), **Lift**, **Scale** or **Subtle zoom**.
- **Reveal on scroll.** Brings the sections below the first into view as the shopper scrolls. **None**, **On enter** (default) or **Scroll-linked**. Scroll-linked ties the motion to the scroll position where the browser supports it, and works like On enter elsewhere.

## Browser support

Page transitions and the transition to the product page use a browser feature that isn't available everywhere yet. In a browser without it, links simply load the next page as usual. Nothing breaks and nothing needs setting up; the effect appears for shoppers whose browser supports it.

## Tips

- **Keep one kind of motion in charge.** Page transitions, the product morph and reveal on scroll are designed to work together, but a strong card hover on top of all three makes the store feel busy. If you add a hover effect, **Subtle zoom** is the quietest.
- **Choose None for reveal on scroll if your pages are long lists.** Sections arriving one by one reads well on an editorial home page; on a page of many short sections it can feel slow.
- **Test on a real phone.** Motion that looks smooth on a desktop monitor can feel sluggish on an older phone.

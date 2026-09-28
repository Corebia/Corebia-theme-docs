---
title: Store locations
layout: default
parent: Sections
nav_order: 46
permalink: /sections/store-locations/
---

# Store locations

**Store locations** lists your physical stores, each with an optional photo, its address, opening hours, a phone number and a link for directions. There is no embedded map: the directions link opens Google Maps with the address filled in, which needs no API key and loads nothing until it is clicked.

It can't be placed in the header or footer groups. The preset starts with two example stores; replace their names, addresses and phone numbers before publishing.

## Settings

- **Heading.** Default: `Visit us`.
- **Text.** Optional rich text under the heading.
- **Columns on desktop.** Range: 1 to 3. Default: 2. Tablets show at most two columns, and phones one.
- **Color scheme.** Default: scheme-1.

### Spacing

- **Top padding** / **Bottom padding.** Range: 0 to 300 px in 5 px steps. Default: 60 px each.

## Blocks

A section with no stores shows nothing on the storefront.

### Store

- **Image.** Optional photo of the store.
- **Name.** The store's name.
- **Address.** One line per line of the address, as you would write it on an envelope.
- **Opening hours.** Rich text, so each day or range of days can go on its own line.
- **Phone.** Shown as a link that dials the number on a phone.
- **Show directions link.** Adds a "Get directions" link that opens the address in Google Maps, in a new tab. Default: on.

## Tips

- **Write the address the way Google knows it.** The directions link searches for exactly what you type, so a street, town and postcode find the right place; a building nickname may not.
- **Include the country code in the phone number** if you have shoppers abroad, for example `+44 20 7946 0000`.
- **Match the column count to your stores.** Two stores sit best in two columns, three in three; one store reads best in a single column.
- **Pair it with a contact form.** The **page.contact-stores** template puts this section and a [Contact form](../contact-form/) on one page. See [Alternate page templates](../../templates/page-templates/#contact-and-stores).

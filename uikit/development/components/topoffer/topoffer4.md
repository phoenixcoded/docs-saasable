---
description: >-
  The TopOffer4 component renders a collapsible alert card with a customizable
  message and optional secondary label and link, featuring central alignment and
  responsive styling.
---

# TopOffer4

{% hint style="info" %}
All available props for the TopOffer4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the TopOffer section.
{% endhint %}

**Component path**: `src/blocks/top-offer/TopOffer4.tsx`

**Component usage path:**  `src/app/blocks/top-offer/top-offer4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/top-offer/top-offer4**](https://www.saasable.io/blocks/top-offer/top-offer4)

## Props Details

| Prop            | Type                                                            | Description                                                                                                                                                      | Displayed as                                                                                                      |
| --------------- | --------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **offer**       | `{ label: string; secondaryLabel?: string; link?: LinkProps; }` | Contains details about the offer. It includes a `label` for the primary message, optionally a `secondaryLabel` for additional text, and a `link` for navigation. | `{ label: 'Special Discount!', secondaryLabel: 'Save More', link: { href: '/discounts', title: 'See Details' } }` |
| **handleClick** | `function` (Optional)                                           | A function to handle the click event for closing the alert. If not provided, the alert can be closed by internal state management.                               | `() => console.log('Alert closed')`                                                                               |

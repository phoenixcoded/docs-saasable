---
description: >-
  The TopOffer3 component displays a collapsible alert card with a central
  message and optional link, including customizable styling and focus-visible
  enhancements.
---

# TopOffer3

{% hint style="info" %}
All available props for the TopOffer3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the TopOffer section.
{% endhint %}

**Component path**: `src/blocks/top-offer/TopOffer3.tsx`

**Component usage path:**  `src/app/blocks/top-offer/top-offer3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/top-offer/top-offer3**](https://www.saasable.io/blocks/top-offer/top-offer3)

## Props Details

| Prop            | Type                                                            | Description                                                                                                                                   | Displayed as                                                                        |
| --------------- | --------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| **offer**       | `{ label: string; secondaryLabel?: string; link?: LinkProps; }` | An object representing the offer details. It typically includes a `label` for the message and optionally a `link` for additional information. | `{ label: 'Limited Time Offer!', link: { href: '/special', title: 'Learn More' } }` |
| **handleClick** | `function` (Optional)                                           | A function to handle the click event for closing the alert. If not provided, the alert can be closed by internal state management.            | `() => console.log('Alert closed')`                                                 |

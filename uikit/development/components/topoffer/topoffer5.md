---
description: >-
  The TopOffer5 component displays a collapsible alert card with a background
  image, featuring a customizable message, email input with a button, and
  responsive styling for different screen sizes.
---

# TopOffer5

{% hint style="info" %}
All available props for the TopOffer5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the TopOffer section.
{% endhint %}

**Component path**: `src/blocks/top-offer/TopOffer5.tsx`

**Component usage path:**  `src/app/blocks/top-offer/top-offer5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/top-offer/top-offer5**](https://www.saasable.io/blocks/top-offer/top-offer5)

## Props Details

| Prop            | Type                  | Description                                                                                                                      | Displayed as                                                       |
| --------------- | --------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **heading**     | `string`              | The main heading text of the alert.                                                                                              | `"Exclusive Offer"`                                                |
| **caption**     | `string` (Optional)   | The caption or additional description for the offer.                                                                             | `"Sign up now to receive updates and special offers!"`             |
| **bgImage**     | `BgImageProps`        | Contains the background image configuration for the `GraphicsCard`.                                                              | `{ src: '/images/offer-bg.jpg', alt: 'Background Image' }`         |
| **primaryBtn**  | `ButtonProps`         | Props for the primary button used in the subscription input field.                                                               | `{ label: 'Subscribe', onClick: () => console.log('Subscribed') }` |
| **icon**        | `SpriteIconProps`     | The icon to be displayed within the alert. Can be a string (icon name) or `SvgIconProps`.                                        | It will display an icon on the left side of the top offer.         |
| **handleClick** | `function` (Optional) | Function to handle the click event for closing the alert. If not provided, the alert can be closed by internal state management. | `() => console.log('Alert closed')`                                |

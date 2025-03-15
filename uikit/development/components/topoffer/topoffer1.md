---
description: >-
  The TopOffer1 component renders a collapsible alert card with customizable
  heading, caption, and buttons, and includes an icon with responsive styling
  and conditional layout adjustments.
---

# TopOffer1

{% hint style="info" %}
All available props for the TopOffer1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the TopOffer section.
{% endhint %}

**Component path**: `src/blocks/top-offer/TopOffer1.tsx`

**Component usage path:**  `src/app/blocks/top-offer/top-offer1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/top-offer/top-offer1**](https://www.saasable.io/blocks/top-offer/top-offer1)

## Props Details

| Prop             | Type                     | Description                                                                                                                                                                      | Displayed as                                                             |
| ---------------- | ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| **heading**      | `string`                 | The main heading or title for the offer. This will be displayed prominently at the top of the alert.                                                                             | `"Limited Time Offer"`                                                   |
| **caption**      | `string` (Optional)      | A subheading or description that provides additional context or details about the offer.                                                                                         | `"Get 20% off on your next purchase"`                                    |
| **primaryBtn**   | `ButtonProps`            | An optional object defining the primary button's properties, such as `text`, `onClick` handler, and `variant`. It is displayed on the right side of the alert on larger screens. | `{ text: 'Shop Now', onClick: handleShopNow, variant: 'outlined' }`      |
| **secondaryBtn** | `ButtonProps` (Optional) | An optional object defining the secondary button's properties, similar to `primaryBtn`. It is also displayed on the right side of the alert on larger screens.                   | `{ text: 'Learn More', onClick: handleLearnMore, variant: 'contained' }` |
| **icon**         | `SpriteIconProps`        | An icon or image to be displayed within the alert.                                                                                                                               | It will display an icon on the left side of the top offer.               |
| **handleClick**  | `function` (Optional)    | A function to handle the click event for closing the alert. If not provided, the alert can be closed by the internal state toggle.                                               | `() => console.log('Alert closed')`                                      |

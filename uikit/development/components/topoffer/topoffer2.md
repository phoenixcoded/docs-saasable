# TopOffer2

The `TopOffer2` component renders a collapsible alert card with customizable heading, caption, and an email input field with a button, featuring responsive layout adjustments and conditional styling based on screen size.

{% hint style="info" %}
All available props for the TopOffer2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the TopOffer section.
{% endhint %}

**Component path**: `src/blocks/top-offer/TopOffer2.tsx`

**Component usage path:**  `src/app/blocks/top-offer/top-offer2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/top-offer/top-offer2**](https://www.saasable.io/blocks/top-offer/top-offer2)

## Props Details

| Prop            | Type                  | Description                                                                                                                                                          | Displayed as                                                            |
| --------------- | --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| **heading**     | `string`              | The main heading or title for the offer, displayed prominently within the alert.                                                                                     | `"Join Our Newsletter"`                                                 |
| **caption**     | `string` (Optional)   | A subheading or additional information that provides context or details about the offer.                                                                             | `"Stay updated with the latest news and offers."`                       |
| **primaryBtn**  | `ButtonProps`         | An optional object defining the primary button's properties, such as `text`, `onClick` handler, and `variant`. This button appears within the `OutlinedInput` field. | `{ text: 'Subscribe', onClick: handleSubscribe, variant: 'contained' }` |
| **icon**        | `SpriteIconProps`     | An icon or image to be displayed within the alert.                                                                                                                   | It will display an icon on the left side of the top offer.              |
| **handleClick** | `function` (Optional) | A function to handle the click event for closing the alert. If not provided, the alert can be closed by internal state management.                                   | `() => console.log('Alert closed')`                                     |

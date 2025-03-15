---
description: >-
  The Cta2 renders a call-to-action section featuring a background image with a
  gradient overlay, a heading, and a primary button, all within a responsive
  layout provided by Material-UI components.
---

# Cta2

{% hint style="info" %}
All available props for the Cta2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta2.tsx`

**Component usage path:**  `src/app/blocks/cta/cta2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta2**](https://www.saasable.io/blocks/cta/cta2)

## Props Details

| Prop           | Type                      | Description                                                                           | Displayed as                                     |
| -------------- | ------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------ |
| **bgImage**    | `BgImageProps` (Optional) | URL of the background image for the `GraphicsCard`. Optional.                         | Sets the background image of the card.           |
| **heading**    | `string`                  | Main heading text displayed in the card. Required.                                    | Displays the primary heading in the card.        |
| **primaryBtn** | `ButtonProps`             | Properties for the primary button, such as text, style, and click handlers. Required. | Renders a prominent button for user interaction. |

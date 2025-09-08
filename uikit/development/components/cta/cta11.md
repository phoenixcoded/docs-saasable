---
description: >-
  The Cta11 component displays a call-to-action section with an image on one
  side, a list of features with icons and text on the other, and primary and
  secondary buttons for user interaction.
---

# Cta11

{% hint style="info" %}
All available props for the Cta11 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta11.tsx`

**Component usage path:**  `src/app/blocks/cta/cta11/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta11**](https://www.saasable.io/blocks/cta/cta11)

## Props Details

| Prop             | Type                     | Description                                                                                       | Displayed as                                   |
| ---------------- | ------------------------ | ------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| **heading**      | `string`                 | Main heading text displayed prominently.                                                          | Positioned at the top of the section.          |
| **caption**      | `string`                 | Additional text providing context or details related to the heading.                              | Positioned below the heading.                  |
| **primaryBtn**   | `ButtonProps`            | Properties for the primary call-to-action button, including text, color, size, and variant.       | Main action button, styled prominently.        |
| **secondaryBtn** | `ButtonProps` (Optional) | Properties for the secondary button, offering an alternative action with a different style.       | Alternative action button, typically outlined. |
| **list**         | `ListProps[]` (Optional) | Array of items each containing primary text. Can include icons to represent features or benefits. | Rendered as a list with optional icons.        |
| **image**        | `ImageCommonProps`       | Properties for the image, including source, alt text, and styling options.                        | Displayed as a visual element or background.   |

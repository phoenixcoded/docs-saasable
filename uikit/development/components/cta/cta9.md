---
description: >-
  Cta9 component creates a call-to-action section with a responsive layout,
  heading and caption alongside a prominent button, and an image with a gradient
  overlay that adjusts based on text direction
---

# Cta9

{% hint style="info" %}
All available props for the Cta9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta9.tsx`

**Component usage path:**  `src/app/blocks/cta/cta9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta9**](https://www.saasable.io/blocks/cta/cta9)

## Props Details

| Prop           | Type               | Description                                                                          | Displayed as                                   |
| -------------- | ------------------ | ------------------------------------------------------------------------------------ | ---------------------------------------------- |
| **heading**    | `string`           | The main headline text for the call-to-action section.                               | Displayed prominently at the top.              |
| **caption**    | `string`           | Secondary text providing additional context or details below the heading.            | Positioned below the heading.                  |
| **primaryBtn** | `ButtonProps`      | Properties for the primary button, including text, color, size, and variant.         | Rendered below the caption as a CTA.           |
| **image**      | `ImageCommonProps` | Properties related to the background image, including source, alt text, and styling. | Used for displaying a styled background image. |

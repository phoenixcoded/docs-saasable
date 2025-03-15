---
description: >-
  Cta8 component creates a visually engaging call-to-action section with a
  centered heading, caption,  primary button, complemented by an image that
  features a gradient overlay and responsive scaling
---

# Cta8

{% hint style="info" %}
All available props for the Cta8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta8.tsx`

**Component usage path:**  `src/app/blocks/cta/cta8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta8**](https://www.saasable.io/blocks/cta/cta8)

## Props Details

| Prop           | Type               | Description                                                               | Displayed as                                   |
| -------------- | ------------------ | ------------------------------------------------------------------------- | ---------------------------------------------- |
| **heading**    | `string`           | The main headline text of the call-to-action section.                     | Displayed prominently at the top.              |
| **caption**    | `string`           | Secondary text providing additional context or details below the heading. | Positioned below the heading.                  |
| **primaryBtn** | `ButtonProps`      | Properties for the primary button, including text, color, and variant.    | Rendered below the caption as a CTA.           |
| **image**      | `ImageCommonProps` | Properties related to the background image, including source and styling. | Used for displaying a styled background image. |

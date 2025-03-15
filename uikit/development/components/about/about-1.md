---
description: >-
  The About1 component is designed to display a section with a heading, two
  descriptions, and an image.
---

# About 1



{% hint style="success" %}
All available props for the `About1` component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the about section.
{% endhint %}

**Component path**: `src/blocks/about/About1.tsx`

**Component usage path:**  `src/app/blocks/about/about1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/about/about1](https://www.saasable.io/blocks/about/about1)

## Props Details

| Prop             | Type               | Description                                                                                           | Displayed as                                    |
| ---------------- | ------------------ | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| **heading**      | `string`           | The main title of the section.                                                                        | Large centered text (`Typography` variant="h2") |
| **description1** | `string`           | The first description paragraph, displayed on the left side of the section.                           | Left-aligned paragraph in `Grid`                |
| **description2** | `string`           | The second description paragraph, displayed on the right side of the section.                         | Right-aligned paragraph in `Grid`               |
| **image**        | `ImageCommonProps` | The image to be displayed, with additional styling for scaling, positioning, and background gradient. | Image with styling applied (`GraphicsImage`)    |


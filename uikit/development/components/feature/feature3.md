---
description: >-
  The Feature3 component renders a section with a heading and optional caption,
  featuring three blocks of content: one prominent block with an image and
  optional action button, and two additional image
---

# Feature3

{% hint style="info" %}
All available props for the Feature3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature3.tsx`

**Component usage path:**  `src/app/blocks/feature/feature3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature3**](https://www.saasable.io/blocks/feature/feature3)

## Props Details

| Prop           | Type                | Description                                                     | Displayed as                                                                                            |
| -------------- | ------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`            | Main title of the section.                                      | `"Our Key Features"`                                                                                    |
| **caption**    | `string` (Optional) | Optional subtitle or description.                               | `"Discover the highlights of our product."`                                                             |
| **blockData1** | `BlockProps`        | Content block with image, title, and description.               | `{ image: { src: 'path/to/image1.jpg' }, title: 'Feature 1', description: 'Description of feature 1' }` |
| **blockData2** | `BlockProps`        | Second content block.                                           | `{ image: { src: 'path/to/image2.jpg' }, title: 'Feature 2', description: 'Description of feature 2' }` |
| **blockData3** | `BlockProps`        | Third content block.                                            | `{ image: { src: 'path/to/image3.jpg' }, title: 'Feature 3', description: 'Description of feature 3' }` |
| **actionBtn**  | `ButtonProps`       | Optional button with properties like label, color, and variant. | `{ variant: 'contained', color: 'primary', children: 'Learn More' }`                                    |

---
description: >-
  The Benefit7 component renders a section with a responsive layout featuring
  background images, a heading, caption, and multiple counter and card
  components with custom styling and overlay effects.
---

# Benefit7

{% hint style="info" %}
All available props for the Benefit7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Benefit section.
{% endhint %}

**Component path**: `src/blocks/benefit/Benefit7.tsx`

**Component usage path:**  `src/app/blocks/benefit/benefit7/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/benefit/benefit7](https://www.saasable.io/blocks/benefit/benefit7)

## Props Details

| Prop            | Type           | Description                                           | Displayed as                                        |                                                       |
| --------------- | -------------- | ----------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------- |
| **bgImage1**    | `BgImageProps` | Background image for the first `GraphicsCard`.        | Applied as background in the top-left card section. | Background image in the first section of the layout.  |
| **bgImage2**    | `BgImageProps` | Background image for the second `GraphicsCard`.       | Applied conditionally in the bottom-right card.     | Background image in the second section of the layout. |
| **heading**     | `string`       | Main heading text for the section.                    | Rendered at the top of the section.                 | Displays the section title.                           |
| **caption**     | `string`       | Subtitle or description text.                         | Rendered below the heading.                         | Provides additional context below the heading.        |
| **blockDetail** | `BlockProps[]` | Array of counter card details (count, caption, unit). | Rendered as multiple `CounterCard` and `CardText`.  | Displays numerical data and descriptions in cards.    |

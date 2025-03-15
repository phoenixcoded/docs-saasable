---
description: >-
  The About2 component is structured to display a section with a heading,
  caption, image, description, title, and a button.
---

# About 2

{% hint style="info" %}
All available props for the `About2` component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the about section.
{% endhint %}

**Component path**: `src/blocks/about/About2.tsx`

**Component usage path:**  `src/app/blocks/about/about2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/about/about2](https://www.saasable.io/blocks/about/about2)

## Props Details

| Prop            | Type               | Description                                                                            | Displayed as                                 |
| --------------- | ------------------ | -------------------------------------------------------------------------------------- | -------------------------------------------- |
| **heading**     | `string`           | The main title of the section, displayed at the top.                                   | Large centered text within `Typeset`         |
| **caption**     | `string`           | A subtitle or brief explanation, displayed under the heading.                          | Centered subtitle text within `Typeset`      |
| **title**       | `string`           | The title within the left-side card, providing context or focus.                       | `Typography` within a `GraphicsCard`         |
| **description** | `string`           | A description or body text within the left-side card.                                  | `Typography` within a `GraphicsCard`         |
| **image**       | `ImageCommonProps` | The image to be displayed, with scaling and positioning applied.                       | `GraphicsImage` within a `GraphicsCard`      |
| **primaryBtn**  | `ButtonProps`      | A button at the bottom of the left-side card, customizable with MUI Button properties. | `Button` wrapped in `ButtonAnimationWrapper` |


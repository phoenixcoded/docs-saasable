---
description: >-
  The SmallHero7 component features a hero section with a heading and caption on
  a graphics card, a primary button, and an image section with a gradient
  overlay, arranged in a responsive grid layout.
---

# SmallHero7

{% hint style="info" %}
All available props for the SmallHero7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero7.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero7**](https://www.saasable.io/blocks/small-hero/small-hero7)

## Props Details

| Prop           | Type               | Description                                                         | Displayed as                                                                                                                         |
| -------------- | ------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**    | `string`           | Main heading or title of the hero section.                          | `"Discover Our Latest Collection"`                                                                                                   |
| **caption**    | `string`           | Optional brief description or subtitle displayed below the heading. | `"Exclusive designs and styles just for you"`                                                                                        |
| **primaryBtn** | `ButtonProps`      | Properties for the primary action button.                           | `{ onClick: handleClick, children: "Explore Now" }`                                                                                  |
| **image**      | `ImageCommonProps` | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |

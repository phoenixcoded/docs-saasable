---
description: >-
  Hero13 is a hero section featuring a centered heading and caption, a
  call-to-action button, and a responsive image carousel created with
  react-slick, all styled with MUI components and custom styling.
---

# Hero13

{% hint style="info" %}
All available props for the Hero13 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero13.tsx`

**Component usage path:**  `src/app/blocks/hero/hero13/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero13**](https://www.saasable.io/blocks/hero/hero13)

## Props Details

| Prop           | Type                 | Description                                                                                                 | Displayed as                                                                                                                             |
| -------------- | -------------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`             | Main heading text of the section.                                                                           | `"Discover Our Latest Collection"`                                                                                                       |
| **caption**    | `string`             | Secondary line of text for additional context.                                                              | `"Explore a curated selection of our finest products."`                                                                                  |
| **exploreBtn** | `ButtonProps`        | Properties for the "Explore" button.                                                                        | `{ variant: "contained", color: "primary", children: "Explore Now" }`                                                                    |
| **images**     | `ImageCommonProps[]` | <p>Array of<br>Image path or Array  of object with <code>light</code> and <code>dark</code> image path.</p> | <p><code>["path-to-image.svg"]</code><br> or <br><code>[{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }]</code></p> |

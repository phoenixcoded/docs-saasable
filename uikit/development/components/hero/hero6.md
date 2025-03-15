---
description: >-
  The Hero6 component is a responsive hero section featuring an optional chip, a
  centered heading with caption, primary and secondary buttons, and a carousel
  of images displayed using react-slick.
---

# Hero6

{% hint style="info" %}
All available props for the Hero6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero6.tsx`

**Component usage path:**  `src/app/blocks/hero/hero6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero6**](https://www.saasable.io/blocks/hero/hero6)

## Props Details

| Prop             | Type                                                          | Description                                                                                                 | Displayed as                                                                                                                             |
| ---------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **chip**         | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip component with text and an optional link.                                                     | `{ label: "Featured", link: { href: "/featured" } }`                                                                                     |
| **heading**      | `string`                                                      | Main heading text                                                                                           | `"Explore Our New Collection"`                                                                                                           |
| **caption**      | `string`                                                      | Secondary caption text                                                                                      | `"Discover the latest trends and styles in our newest collection."`                                                                      |
| **primaryBtn**   | `ButtonProps`                                                 | Properties for the primary button                                                                           | `{ variant: "contained", color: "primary", children: "Shop Now" }`                                                                       |
| **secondaryBtn** | `ButtonProps`                                                 | Properties for the secondary button                                                                         | `{ variant: "outlined", color: "primary", children: "Learn More" }`                                                                      |
| **images**       | `ImageCommonProps[]`                                          | <p>Array of<br>Image path or Array  of object with <code>light</code> and <code>dark</code> image path.</p> | <p><code>["path-to-image.svg"]</code><br> or <br><code>[{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }]</code></p> |

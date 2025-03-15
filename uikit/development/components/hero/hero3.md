---
description: >-
  Hero3 React component that renders a hero section layout with customizable
  elements including images, text, a list, and a button, styled using
  Material-UI and Next.js components.
---

# Hero3

{% hint style="info" %}
All available props for the Hero3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero3.tsx`

**Component usage path:**  `src/app/blocks/hero/hero3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero3**](https://www.saasable.io/blocks/hero/hero3)

## Props Details

| Prop Name       | Type                                                          | Description                                                         | Displayed as                                                                                                                                 |
| --------------- | ------------------------------------------------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip with text and optional link.                          | `{ label: "New Feature", link: { href: "/features", passHref: true } }`                                                                      |
| **headLine**    | `string \| ReactElement`                                      | Main headline for the hero section. Can be text or a React element. | `"Effortless CRM Management, Seamless BusinessGrowth"`                                                                                       |
| **boxImage1**   | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image1.svg"</code><br> or <br><code>{ light: 'path-to-image1-light.svg', dark: 'path-to-image1-dark.svg' }</code></p>      |
| **boxImage2**   | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image2.svg"</code><br> or <br><code>{ light: 'path-to-image2-light.svg', dark: 'path-to-image2-dark.svg' }</code></p>      |
| **boxImage3**   | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image3.svg"</code><br> or <br><code>{ light: 'path-to-image3-light.svg', dark: 'path-to-image3-dark.svg' }</code></p>      |
| **listData**    | `ListDataProps[]` (Optional)                                  | Array of list items with titles and optional links.                 | `[{ title: "Feature 1", link: { href: "/feature1", passHref: true } }, { title: "Feature 2", link: { href: "/feature2", passHref: true } }]` |
| **description** | `string` (Optional)                                           | Optional description text.                                          | `"Discover the amazing features of our new product range."`                                                                                  |
| **exploreBtn**  | `ButtonProps` (Optional)                                      | Optional properties for an "Explore" button.                        | `{ children: "Explore Now", href: "/explore", variant: "outlined", size: "small" }`                                                          |

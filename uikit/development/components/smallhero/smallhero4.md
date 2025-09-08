---
description: >-
  The SmallHero4 React component that renders a responsive section with a
  heading, caption, optional chip, and an optional image, using Material-UI for
  styling and layout.
---

# SmallHero4

{% hint style="info" %}
All available props for the SmallHero4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero4.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero4**](https://www.saasable.io/blocks/small-hero/small-hero4)

## Props Details

| Prop           | Type                                                          | Description                                                                                                | Displayed as                                                                                                                         |
| -------------- | ------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **chip**       | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Displays a badge or label with optional hyperlink.                                                         | `{ label: 'Featured', link: { href: '/featured', passHref: true } }`                                                                 |
| **heading**    | `string`                                                      | The main title or heading of the hero section.                                                             | `"Discover Our New Collection"`                                                                                                      |
| **caption**    | `string`                                                      | A subheading or additional description text below the heading.                                             | `"Explore the latest trends in our new arrivals."`                                                                                   |
| **exploreBtn** | `ButtonProps` (Optional)                                      | Configuration for an optional button, which can include properties like `href`, `onClick`, and `children`. | `{ href: '/explore', children: 'Explore Now' }`                                                                                      |
| **image**      | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.                                                   | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| isCoverImage   | boolean                                                       | Image data (e.g. src, alt) used for display in the right panel                                             | Rendered using `GraphicsImage`inside `GraphicsCard`on the right                                                                      |

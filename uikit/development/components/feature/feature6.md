---
description: >-
  The Feature6 component displays a responsive feature section with animated
  headings, optional images, and a grid of feature cards, utilizing Framer
  Motion for smooth transitions.
---

# Feature6

{% hint style="info" %}
All available props for the Feature6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature6.tsx`

**Component usage path:**  `src/app/blocks/feature/feature6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature6**](https://www.saasable.io/blocks/feature/feature6)

## Props Details

| Prop         | Type                          | Description                                              | Displayed as                                                                                                                         |
| ------------ | ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**  | `string`                      | Main title of the feature section.                       | `"Our Key Features"`                                                                                                                 |
| **caption**  | `string` (Optional)           | Additional subtitle or description.                      | `"Discover the unique aspects of our product"`                                                                                       |
| **image**    | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **features** | `IconCardProps[]`             | Array of feature objects with icon, title, and content.  | `[ { icon: 'icon-name-1', title: 'Feature 1', content: 'Description of feature 1', animationDelay: 0.2 }, ... ]`                     |

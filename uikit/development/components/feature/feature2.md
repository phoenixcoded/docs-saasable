---
description: >-
  The Feature2 component displays a section with a heading, optional caption, an
  optional image, and a list of feature cards, each with an icon and
  description, all within a responsive grid layout.
---

# Feature2

{% hint style="info" %}
All available props for the Feature2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature2.tsx`

**Component usage path:**  `src/app/blocks/feature/feature2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature2**](https://www.saasable.io/blocks/feature/feature2)

## Props Details

| Prop         | Type                          | Description                                               | Displayed as                                                                                                                                                                                                                                                                                                                                                         |
| ------------ | ----------------------------- | --------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**  | `string`                      | Main heading or title of the feature section.             | `"Our Innovative Features"`                                                                                                                                                                                                                                                                                                                                          |
| **caption**  | `string` (Optional)           | Additional context or description under the heading.      | `"Discover the cutting-edge technologies and benefits that set our product apart from the rest."`                                                                                                                                                                                                                                                                    |
| **image**    | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path.  | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p>                                                                                                                                                                                                                                 |
| **features** | `IconCardProps[]` (Optional)  | Array of feature objects with icons, titles, and content. | `[ { "icon": "star", "title": "High Performance", "content": "Our product offers unparalleled speed and efficiency." }, { "icon": "security", "title": "Enhanced Security", "content": "State-of-the-art security features protect your data." }, { "icon": "support", "title": "24/7 Support", "content": "Dedicated support team available around the clock." } ]` |

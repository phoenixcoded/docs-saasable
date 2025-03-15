---
description: >-
  The Feature4 component displays a section with a heading and caption, a list
  of feature cards, and an optional image, all styled responsively using
  Material-UI.
---

# Feature4

{% hint style="info" %}
All available props for the Feature4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature4.tsx`

**Component usage path:**  `src/app/blocks/feature/feature4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature4**](https://www.saasable.io/blocks/feature/feature4)

## Props Details

| Prop        | Type                 | Description                                                                                | Displayed as                                                                                                                                                                                                                                                                        |
| ----------- | -------------------- | ------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`             | The main title or heading of the section.                                                  | `"Innovative Solutions"`                                                                                                                                                                                                                                                            |
| **caption** | `string`             | A brief description or subtitle for additional context.                                    | `"Explore the groundbreaking solutions that are reshaping the industry."`                                                                                                                                                                                                           |
| **cards**   | `ProcessCardProps[]` | An array of objects where each object represents a card with title, description, and icon. | `[{ "title": "High Performance", "description": "Maximize your system's performance with cutting-edge technology.", "icon": "performance_icon" }, { "title": "Energy Efficient", "description": "Reduce energy consumption while achieving high output.", "icon": "energy_icon" }]` |
| **image**   | `ImageCommonProps`   | Image path or object with `light` and `dark` image path.                                   | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p>                                                                                                                                                |

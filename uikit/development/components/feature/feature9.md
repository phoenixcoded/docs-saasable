---
description: >-
  The Feature9 component renders a section with a heading and caption at the
  top, followed by a grid of animated icon cards that display features with
  custom icons and content.
---

# Feature9

{% hint style="info" %}
All available props for the Feature9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature9.tsx`

**Component usage path:**  `src/app/blocks/feature/feature9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature9**](https://www.saasable.io/blocks/feature/feature9)

## Props Details

| Prop         | Type                | Description                                                                 | Displayed as                                                                                                                                                       |
| ------------ | ------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**  | `string`            | Main title of the feature section.                                          | `"Our Key Features"`                                                                                                                                               |
| **caption**  | `string` (Optional) | Additional description or subtitle under the heading.                       | `"Discover the innovative features that make our product stand out"`                                                                                               |
| **features** | `IconCardProps[]`   | List of feature cards, each with icon, title, content, and animation delay. | `[{ icon: 'star', title: 'High Quality', content: '...', animationDelay: 0.2 }, { icon: 'bolt', title: 'Fast Performance', content: '...', animationDelay: 0.4 }]` |

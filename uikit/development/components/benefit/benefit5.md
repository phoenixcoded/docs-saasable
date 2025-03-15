---
description: >-
  The Benefit5 component renders a section with a heading, caption, and a grid
  of animated statistic cards, each displaying a counter, unit, and description.
---

# Benefit5

{% hint style="info" %}
All available props for the Benefit5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Benefit section.
{% endhint %}

**Component path**: `src/blocks/benefit/Benefit5.tsx`

**Component usage path:**  `src/app/blocks/benefit/benefit5/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/benefit/benefit5](https://www.saasable.io/blocks/benefit/benefit5)

## Props Details&#x20;

| Prop            | Type               | Description                                                             | Displayed as                                                                           |
| --------------- | ------------------ | ----------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| **heading**     | `string`           | Main title of the section.                                              | `"Our Key Advantages"`                                                                 |
| **caption**     | `string`           | Additional descriptive text for the section.                            | `"Discover the unique features and benefits that set us apart..."`                     |
| **blockDetail** | `Array of objects` | Array of blocks, each with counter, unit, caption, and animation delay. | `[ { counter: '500', defaultUnit: 'k', caption: 'Users', animationDelay: 0.1 }, ... ]` |


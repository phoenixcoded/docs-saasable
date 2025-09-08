---
description: >-
  The Metrics8 component displays a section with a heading and caption in one
  column, and a list of progress indicators and counters in another column, all
  within a responsive grid layout.
---

# Metrics8

{% hint style="info" %}
All available props for the Metrics8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Metrics section.
{% endhint %}

**Component path**: `src/blocks/metrics/Metrics8.tsx`

**Component usage path:**  `src/app/blocks/metrics/metrics8/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/metrics/metrics8](https://www.saasable.io/blocks/metrics/metrics8)

## Props Details

| Prop            | Type             | Description                                                      | Displayed as                                                 |
| --------------- | ---------------- | ---------------------------------------------------------------- | ------------------------------------------------------------ |
| **heading**     | `string`         | Main title for the section                                       | Displayed in the left column in a `GraphicsCard`             |
| **caption**     | `string`         | Subtitle or description text                                     | Displayed under the `heading` in the left column             |
| **blockDetail** | Array of Objects | List of progress items with caption, progress, counter, and unit | Rendered in the right column with progress bars and counters |


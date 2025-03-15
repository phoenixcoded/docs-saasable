---
description: >-
  The Benefit4 component displays a section with a title and description, an
  optional button, and a grid of counters and captions within a GraphicsCard
  layout.
---

# Benefit4

{% hint style="info" %}
All available props for the Benefit4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Benefit section.
{% endhint %}

**Component path**: `src/blocks/benefit/Benefit4.tsx`

**Component usage path:**  `src/app/blocks/benefit/benefit4/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/benefit/benefit4)[https://www.saasable.io/blocks/benefit/benefit4](https://www.saasable.io/blocks/benefit/benefit4)

## Props Details

| Prop            | Type                                                                | Description                                                                           | Displayed as                                                                                       |
| --------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **heading**     | `string`                                                            | Main title text for the section.                                                      | `"Our Achievements"`                                                                               |
| **caption**     | `string`                                                            | Subtitle or additional description text below the heading.                            | `"Key metrics and milestones"`                                                                     |
| **exploreBtn**  | `object` (optional)                                                 | Button configuration, e.g., text, color, size, and onClick handler.                   | `{ text: "Learn More", onClick: () => { ... }}`                                                    |
| **blockDetail** | `Array<{ counter: number; caption: string; defaultUnit?: string }>` | Array of objects containing counter values, captions, and optional units for display. | `[ { counter: 120, caption: "Projects", defaultUnit: "K" }, { counter: 50, caption: "Clients" } ]` |

---
description: >-
  The Benefit3 component displays a layout with a GraphicsCard containing a
  heading, optional button, and CounterCard components arranged in a responsive
  grid layout.
---

# Benefit3

{% hint style="info" %}
All available props for the Benefit3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Benefit section.
{% endhint %}

**Component path**: `src/blocks/benefit/Benefit3.tsx`

**Component usage path:**  `src/app/blocks/benefit/benefit3/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/benefit/benefit3](https://www.saasable.io/blocks/benefit/benefit3)

## Props Details

| Prop            | Type                                                                | Description                                                                           | Displayed as                                                                                       |
| --------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **heading**     | `string`                                                            | Main title of the benefit section.                                                    | `"Tailored for Your Process"`                                                                      |
| **caption**     | `string` (optional)                                                 | Subtitle or additional description text below the heading.                            | `"Key metrics and milestones"`                                                                     |
| **bgImage**     | `BgImageProps`(optional)                                            | URL or path for the background image of the card.                                     | `"/images/background.jpg"`                                                                         |
| **exploreBtn**  | `object` (optional)                                                 | Button configuration, e.g., text, color, size, and onClick handler.                   | `{ text: "Learn More", onClick: () => { ... }}`                                                    |
| **blockDetail** | `Array<{ counter: number; caption: string; defaultUnit?: string }>` | Array of objects containing counter values, captions, and optional units for display. | `[ { counter: 120, caption: "Projects", defaultUnit: "K" }, { counter: 50, caption: "Clients" } ]` |

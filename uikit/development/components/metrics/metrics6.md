---
description: >-
  The Metrics6 component displays a section with a background image, heading,
  caption, and a grid of CounterCard components showing statistics with dynamic
  layouts and dividers.
---

# Metrics6

{% hint style="info" %}
All available props for the Metrics6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Metrics section.
{% endhint %}

**Component path**: `src/blocks/metrics/Metrics6.tsx`

**Component usage path:**  `src/app/blocks/metrics/metrics6/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/metrics/metrics6](https://www.saasable.io/blocks/metrics/metrics6)

## Props Details

| Prop            | Type                | Description                                        | Displayed as                                                                                                                                                                                    | Visual Example                                       |
| --------------- | ------------------- | -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| **bgImage**     | `string`            | URL of the background image for the `GraphicsCard` | `"https://example.com/background.jpg"`                                                                                                                                                          | Background image of the card                         |
| **heading**     | `string`            | Main heading text                                  | `"Innovative Solutions"`                                                                                                                                                                        | Large, bold text at the top of the section           |
| **caption**     | `string`            | Supporting subtitle text                           | `"Discover our cutting-edge technology and features.`"                                                                                                                                          | Smaller text below the heading                       |
| **blockDetail** | `Array<BlockProps>` | Array of objects containing counter details        | `[ { counter: 120, caption: "Projects Completed", defaultUnit: "K" }, { counter: 35, caption: "Awards Won", defaultUnit: "T" }, { counter: 200, caption: "Happy Clients", defaultUnit: "+" } ]` | Counter cards displaying numeric values and captions |


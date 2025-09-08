---
description: >-
  The Metrics1 component displays a section with a background image, a heading
  caption and multiple counter blocks with numerical values and descriptions,
  adjusting layout based on screen size.
---

# Metrics1

{% hint style="info" %}
All available props for the Metrics1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Metrics section.
{% endhint %}

**Component path**: `src/blocks/metrics/Metrics1.tsx`

**Component usage path:**  `src/app/blocks/metrics/metrics1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/metrics/metrics1](https://www.saasable.io/blocks/metrics/metrics1)



## Props Details

| Prop Name	      | Type                | Description                                                                                                                                                                                                              | Displayed as                                                                                     |
| --------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| **heading**     | `string`            | Main title of the section.                                                                                                                                                                                               | `"Our Key Metrics"`                                                                              |
| **caption**     | `string` (optional) | Additional descriptive text below the heading.                                                                                                                                                                           | `"Here are some of our key achievements."`                                                       |
| **bgImage**     | `string` (optional) | URL or path for the background image.                                                                                                                                                                                    | `"/images/background.jpg"`                                                                       |
| **blockDetail** | Array of objects    | <p>Details for each counter block. Each object includes:<br>- <code>counter</code>: <code>number</code><br>- <code>caption</code>: <code>string</code><br>- <code>defaultUnit</code>: <code>string</code> (optional)</p> | `[ { counter: 120, caption: "Users", defaultUnit: "k" }, { counter: 80, caption: "Projects" } ]` |

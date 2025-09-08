---
description: >-
  The Metrics9 component uses several props to render a styled layout with
  headings, details, and an action button. Here's a detailed explanation of each
  prop along with its usage in the component.
---

# Metrics9

{% hint style="info" %}
All available props for the Metrics9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Metrics section.
{% endhint %}

**Component path**: `src/blocks/metrics/Metrics9.tsx`

**Component usage path:**  `src/app/blocks/metrics/metrics9/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/metrics/metrics9](https://www.saasable.io/blocks/metrics/metrics9)

## Props Details

| Prop            | Type                   | Description                                       | Displayed as                                           |
| --------------- | ---------------------- | ------------------------------------------------- | ------------------------------------------------------ |
| **heading**     | `string`               | Main title for the section                        | Displayed at the top of the card                       |
| **caption**     | `string`               | Subtitle or description text                      | Displayed below the heading                            |
| **blockDetail** | Array of Objects       | List of items with counter, unit, and description | Rendered in a grid layout with counter and description |
| **exploreBtn**  | `ButtonProps` (object) | Props for customizing the "Explore" button        | Rendered as a button at the bottom of the card         |

---
description: >-
  The Process4 component renders an interactive timeline with a changing image
  carousel, updating every 5 seconds and allowing manual step selection.
---

# Process4

{% hint style="info" %}
All available props for the Process4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process4.tsx`

**Component usage path:**  `src/app/blocks/process/process4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process4**](https://www.saasable.io/blocks/process/process4)

## Props Details

| Prop        | Type                 | Description                                                                      | Displayed as                                         |
| ----------- | -------------------- | -------------------------------------------------------------------------------- | ---------------------------------------------------- |
| **heading** | `string`             | Main title for the component                                                     | `"Our Process"`                                      |
| **caption** | `string`             | Additional description or context                                                | `"Here’s a step-by-step guide through our process."` |
| **cards**   | `ProcessCardProps[]` | Array of cards for the timeline, each with a title, description, icon, and image | See example data above                               |

---
description: >-
  The Feature8 component displays a vertical stepper with icons and titles on
  the left and a dynamic graphic image on the right, allowing users to navigate
  through different steps with updated content.
---

# Feature8

{% hint style="info" %}
All available props for the Feature8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature8.tsx`

**Component usage path:**  `src/app/blocks/feature/feature8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature8**](https://www.saasable.io/blocks/feature/feature8)

## Props Details

| Prop        | Type                 | Description                                    | Displayed as                                                                                               |
| ----------- | -------------------- | ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **heading** | `string`             | Main title of the feature section.             | `"How It Works"`                                                                                           |
| **caption** | `string`             | Additional description or subtitle.            | `"Follow these steps to understand our process"`                                                           |
| **cards**   | `ProcessCardProps[]` | List of step cards with details for each step. | `[ { title: "Step 1", description: "Learn...", icon: "icon-name-1", image: "path-to-image-1.jpg" }, ... ]` |

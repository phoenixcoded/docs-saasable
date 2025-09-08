---
description: >-
  SmallHero8 is a responsive hero section component that displays a heading,
  caption, and a clickable video thumbnail that opens a modal with video
  playback.
---

# SmallHero8

{% hint style="info" %}
All available props for the SmallHero8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero8.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero8**](https://www.saasable.io/blocks/small-hero/small-hero8)

## Props Details

| Prop        | Type          | Description                                                         | Displayed as                                                                                                        |
| ----------- | ------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`      | Main heading or title of the hero section.                          | Displayed as a bold, centered heading inside the component.                                                         |
| **caption** | `string`      | Optional brief description or subtitle displayed below the heading. | Displayed as a sub-caption or paragraph under the heading, centered.                                                |
| **video**   | `ButtonProps` | Properties for the primary action button.                           | `thumbnail`is shown as a background image with a play icon. Clicking it opens a modal playing the video from `src`. |

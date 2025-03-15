---
description: >-
  Integration7 that displays a headline, a primary button, and a series of tags
  with icons and labels that scroll horizontally in a marquee, using Material-UI
  for styling and layout.
---

# Integration7

{% hint style="info" %}
All available props for the Integration7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration7.tsx`

**Component usage path:**  `src/app/blocks/integration/integration7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration7**](https://www.saasable.io/blocks/integration/integration7)

## Props Details

| Prop           | Type                  | Description                              | Displayed as                                                          |
| -------------- | --------------------- | ---------------------------------------- | --------------------------------------------------------------------- |
| **marquees**   | `MarqueesDataProps[]` | Array of marquee configurations and data | Renders multiple scrolling marquees                                   |
| **headLine**   | `string`              | Main heading or title of the section     | `"Connect with top-tier tools available Interface"`                   |
| **primaryBtn** | `ButtonProps`         | Properties for the primary action button | `{ variant: "contained", color: "primary", children: "Get Started" }` |

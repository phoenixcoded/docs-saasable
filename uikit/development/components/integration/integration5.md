---
description: >-
  Integration5 will display a headline, a caption, and a button, alongside a
  grid of icons and curved elements.
---

# Integration5

{% hint style="info" %}
All available props for the Integration5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration5.tsx`

**Component usage path:**  `src/app/blocks/integration/integration5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration5**](https://www.saasable.io/blocks/integration/integration5)

## Props Details

| Prop            | Type          | Description                              | Displayed as                                                          |
| --------------- | ------------- | ---------------------------------------- | --------------------------------------------------------------------- |
| **headLine**    | `string`      | Main heading or title of the section     | `"Innovative Solutions"`                                              |
| **captionLine** | `string`      | Additional descriptive text or subtitle  | `"Discover cutting-edge technologies..."`                             |
| **primaryBtn**  | `ButtonProps` | Properties for the primary action button | `{ variant: "contained", color: "primary", children: "Get Started" }` |

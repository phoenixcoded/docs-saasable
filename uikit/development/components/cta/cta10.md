---
description: >-
  The Cta10 component is a call-to-action section featuring a profile group with
  review highlights, a list of features with icons and text, and two buttons,
  alongside a prominent image on the other side
---

# Cta10

{% hint style="info" %}
All available props for the Cta10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta10.tsx`

**Component usage path:**  `src/app/blocks/cta/cta10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta10**](https://www.saasable.io/blocks/cta/cta10)

## Props Details

| Prop              | Type                                                   | Description                                                                              | Displayed as                        |
| ----------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------- | ----------------------------------- |
| **heading**       | `string`                                               | Main heading text for the call-to-action section.                                        | Displayed prominently at the top.   |
| **caption**       | `string`                                               | Supplementary text providing additional context below the heading.                       | Positioned below the heading.       |
| **primaryBtn**    | `ButtonProps`                                          | Properties for the primary button, including text, color, size, and variant.             | Main call-to-action button.         |
| **secondaryBtn**  | `ButtonProps`                                          | Properties for the secondary button, usually styled differently from the primary button. | Alternative call-to-action button.  |
| **profileGroups** | `{ avatarGroups: AvatarGroupProps[]; review: string }` | Contains avatar groups and review text.                                                  | Displays user profiles and reviews. |
| **list**          | `ListProps[]` (Optional)                               | Array of list items with optional icons and primary text.                                | Displays features or benefits.      |
| **image**         | `ImageCommonProps`                                     | Properties related to the background image, including source and styling.                | Decorative or main visual element.  |

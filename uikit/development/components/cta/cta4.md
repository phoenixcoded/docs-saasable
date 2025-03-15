---
description: >-
  Cta4 displays a call-to-action section featuring a headline, a button, profile
  avatars, a list of items, and client content, all presented within a
  responsive grid layout and enhanced with animation
---

# Cta4

{% hint style="info" %}
All available props for the Cta4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta4.tsx`

**Component usage path:**  `src/app/blocks/cta/cta4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta4**](https://www.saasable.io/blocks/cta/cta4)

## Props Details

| Prop              | Type                                                   | Description                                                                   | Displayed as                                                                                        |
| ----------------- | ------------------------------------------------------ | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **headLine**      | `string \| ReactElement`                               | `string` or `ReactElement` that represent section headline                    | Main heading or content to be displayed at the top of the card. Can be a string or a React element. |
| **primaryBtn**    | `ButtonProps`                                          | Properties for the primary button, including text, style, and handlers.       | Renders a prominent action button.                                                                  |
| **profileGroups** | `{ avatarGroups: AvatarGroupProps[]; review: string }` | Data for user avatars and review text.                                        | Renders user profiles and a testimonial.                                                            |
| **list**          | `ListProps[]`                                          | Array of items with text and icons.                                           | Renders a list of features or benefits.                                                             |
| **clientContent** | `string`                                               | Additional content or callout, displayed in the top-right corner of the card. | Provides extra information or emphasis.                                                             |

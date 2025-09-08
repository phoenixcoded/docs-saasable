---
description: >-
  This code defines a React functional component Cta13 that renders a
  call-to-action section with animated elements, utilizing Material-UI
  components and Framer Motion for transitions.
---

# Cta13

{% hint style="info" %}
All available props for the Cta13 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta13.tsx`

**Component usage path:**  `src/app/blocks/cta/cta13/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta13**](https://www.saasable.io/blocks/cta/cta13)

## Props Details

| Prop        | Type               | Description                                                                                          | Displayed as                                                                                      |
| ----------- | ------------------ | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **heading** | `string`           | Main heading text displayed prominently.                                                             | Positioned at the top of the section.                                                             |
| **caption** | `string`           | Additional text providing context or details related to the heading.                                 | Positioned below the heading                                                                      |
| listdata    | `ListDataProps[];` | An array of objects, each containing a title, description, chips, and button — used to render cards. | Displayed as a vertical stack of cards, each showing title, chip tags, description, and a button. |


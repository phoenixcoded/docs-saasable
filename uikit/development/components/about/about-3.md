---
description: >-
  The About3 component is designed to display content in two main columns: one
  with text (including the heading, description, and list) and one with an
  image.
---

# About 3

{% hint style="info" %}
All available props for the `About3` component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the about section.
{% endhint %}

**Component path**: `src/blocks/about/About3.tsx`

**Component usage path:**  `src/app/blocks/about/about3/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/about/about3](https://www.saasable.io/blocks/about/about3)

## Props Details

| Prop            | Type               | Description                                                                           | Displayed as                              |
| --------------- | ------------------ | ------------------------------------------------------------------------------------- | ----------------------------------------- |
| **heading**     | `string`           | The main title of the section, displayed at the top of the left column.               | Large text within `Typeset`               |
| **description** | `string`           | A description or introductory text, displayed below the heading.                      | `Typography` below the heading            |
| **list**        | `ListItem[]`       | A list of items, each with a title, displayed below the description in a grid format. | `Typography` with `SvgIcon` for each item |
| **image**       | `ImageCommonProps` | The image to be displayed, with scaling and positioning applied.                      | `GraphicsImage` within a `GraphicsCard`   |

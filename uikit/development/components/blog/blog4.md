---
description: >-
  The Blog4 component renders a blog section with a title, a caption, a
  responsive slider of blog cards, and an optional "explore more" button.
---

# Blog4

{% hint style="info" %}
All available props for the Blog4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog4.tsx`

**Component usage path:**  `src/app/blocks/blog/blog4/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog4](https://www.saasable.io/blocks/blog/blog4)

## Props Details

| Prop            | Type                | Description                                       | Displayed as                                                   |
| --------------- | ------------------- | ------------------------------------------------- | -------------------------------------------------------------- |
| **heading**     | `string` (optional) | Main heading of the blog section                  | `<Typography variant="h2">{heading}</Typography>`              |
| **caption**     | `string` (optional) | Secondary description or subtitle for the section | `<Typography variant="h6">{caption}</Typography>`              |
| **blogs**       | `BlogListProps[]`   | Array of blog items to display in the slider      | Mapped over in the `Slider` component to render each blog card |
| **exploreMore** | `ButtonProps`       | Customizable call-to-action button                | Rendered as a `Button` if `exploreMore` is provided            |

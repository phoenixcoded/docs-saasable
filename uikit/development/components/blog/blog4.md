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

| Prop            | Type                                              | Description                                                                                                                                                         | Displayed as                                                   |
| --------------- | ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| **heading**     | Main heading of the blog section                  | `"Latest Blog Updates"`                                                                                                                                             | `<Typography variant="h2">{heading}</Typography>`              |
| **caption**     | Secondary description or subtitle for the section | `"Discover the latest trends and insights from our blog"`                                                                                                           | `<Typography variant="h6">{caption}</Typography>`              |
| **blogs**       | Array of blog items to display in the slider      | `[ { image: "path/to/image1.jpg", chips: ["Tech"], date: "August 27, 2024", caption: "Exploring the future of technology", link: { href: "/blog/future-tech" } } ]` | Mapped over in the `Slider` component to render each blog card |
| **exploreMore** | Customizable call-to-action button                | `{ href: "/blog", variant: "outlined", size: "large" }`                                                                                                             | Rendered as a `Button` if `exploreMore` is provided            |

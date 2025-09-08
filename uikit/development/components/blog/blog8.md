---
description: >-
  Blog8 renders a categorized blog section with a main heading, optional
  caption, and an "Explore More" button.
---

# Blog8

{% hint style="info" %}
All available props for the Blog8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog8.tsx`

**Component usage path:**  `src/app/blocks/blog/blog8/page.tsx`

**Preview link:** [https://stage.saasable.io/blocks/blog/blog8](https://stage.saasable.io/blocks/blog/blog8)

## Props Details

| Prop        | Type                | Description                                                     | Displayed as                                                       |
| ----------- | ------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------ |
| **heading** | `string` (optional) | Main title of the blog section.                                 | Top of the section in large font (via `Typeset` component).        |
| caption     | `string` (optional) | Short subheading or explanation below the heading.              | Below the heading (via `Typeset`).                                 |
| exploreMore | `ButtonProps`       | Optional button to explore more content (with href or action).  | Top-right corner as a "Explore More" button.                       |
| categories  | `CategoryProps[]`   | List of blog categories used to filter blogs.                   | Rendered as slider buttons (`CategoryButton`) for category filter. |
| blogs       | `BlogListProps[]`   | Array of blog posts with metadata (title, image, avatar, etc.). | Displayed in a card layout with title, image, author, etc.         |

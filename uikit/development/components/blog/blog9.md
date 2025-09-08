---
description: >-
  Blog9 is a responsive animated blog section component in MUI React that
  displays a list of blog cards with headings, captions, and optional "Explore
  More" button.
---

# Blog9

{% hint style="info" %}
All available props for the Blog9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog9.tsx`

**Component usage path:**  `src/app/blocks/blog/blog9/page.tsx`

**Preview link:** [https://stage.saasable.io/blocks/blog/blog9](https://stage.saasable.io/blocks/blog/blog9)

## Props Details

| Prop        | Type                                       | Description                                                     | Displayed as                                                |
| ----------- | ------------------------------------------ | --------------------------------------------------------------- | ----------------------------------------------------------- |
| **heading** | `string` (optional)                        | Main title of the blog section.                                 | Top of the section in large font (via `Typeset` component). |
| caption     | `string` (optional)                        | Short subheading or explanation below the heading.              | Below the heading (via `Typeset`).                          |
| exploreMore | `ButtonProps`                              | Optional button to explore more content (with href or action).  | Top-right corner as a "Explore More" button.                |
| blogs       | <p><code>BlogListProps[]</code></p><p></p> | Array of blog posts with metadata (title, image, avatar, etc.). | Displayed in a card layout with title, image, author, etc.  |

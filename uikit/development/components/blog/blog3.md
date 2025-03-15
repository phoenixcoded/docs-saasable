---
description: >-
  The Blog3 component displays a grid of blog posts with animated transitions,
  including a heading, caption, and optional profile details, using Material UI
  and framer-motion for styling and animations.
---

# Blog3

{% hint style="info" %}
All available props for the Blog3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog3.tsx`

**Component usage path:**  `src/app/blocks/blog/blog3/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog3](https://www.saasable.io/blocks/blog/blog3)

## Props Details

| Prop        | Type          | Description                                   | Displayed as                                                        | Usage in Code                                           |
| ----------- | ------------- | --------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------- |
| **heading** | `string`      | Main heading for the blog section             | `"Featured Articles"`                                               | Displayed as the main heading in `Typeset`              |
| **caption** | `string`      | Subtitle or additional text under the heading | `"Check out our latest posts from industry experts"`                | Displayed below the heading in `Typeset`                |
| **blogs**   | `BlogProps[]` | Array of blog objects with details            | `[ { "caption": "Exploring the Future of Web Development", ... } ]` | Used to render individual blog cards in the grid layout |


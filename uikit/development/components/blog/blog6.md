---
description: >-
  Blog6 component renders a section of blog posts with a main heading, a
  featured blog card, additional blog cards in a grid layout, and  "Explore
  More" button, using Material UI and responsive design
---

# Blog6

{% hint style="info" %}
All available props for the Blog1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog6.tsx`

**Component usage path:**  `src/app/blocks/blog/blog6/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog6](https://www.saasable.io/blocks/blog/blog6)

## Props Details

| Prop            | Type                | Description                                  | Displayed as                                                      |
| --------------- | ------------------- | -------------------------------------------- | ----------------------------------------------------------------- |
| **heading**     | `string` (optional) | Title of the blog section                    | `"Latest Blog Posts"`                                             |
| **caption**     | `string` (optional) | Caption or subtitle for the blog section     | `"Explore our latest articles and insights."`                     |
| **blogs**       | `BlogListProps[]`   | List of individual blog posts                | See the `Example Structure` section above                         |
| **exploreMore** | `ButtonProps`       | Button properties for exploring more content | `{ href: '/explore-more', children: 'Explore More', sx: { ... }}` |

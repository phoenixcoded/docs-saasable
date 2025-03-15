---
description: >-
  The Blog5 component renders a section of blog posts with a main heading, a
  featured blog card, additional blog cards in a grid layout, and a "View More"
  button, using Material UI and responsive design
---

# Blog5

{% hint style="info" %}
All available props for the Blog5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog5.tsx`

**Component usage path:**  `src/app/blocks/blog/blog5/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog5](https://www.saasable.io/blocks/blog/blog5)

## Props Details

| Prop         | Type                      | Description                                   | Displayed as                                        |
| ------------ | ------------------------- | --------------------------------------------- | --------------------------------------------------- |
| **heading**  | `string`                  | Main heading for the blog section             | `"Latest Blog Posts"`                               |
| **caption**  | `string`                  | Subtitle or additional text under the heading | `"Explore our most recent articles and updates"`    |
| **viewMore** | `ButtonProps & LinkProps` | Configuration for the "View More" button/link | `{ href: "/more-blogs", variant: "contained" }`     |
| **blogs**    | `BlogListProps[]`         | Array of blog objects with details            | `[{ "caption": "Understanding React Hooks", ... }]` |

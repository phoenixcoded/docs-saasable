---
description: >-
  Blog6 component renders a section of blog posts with a main heading, a
  featured blog card, additional blog cards in a grid layout, and  "Explore
  More" button, using Material UI and responsive design
---

# Blog7

{% hint style="info" %}
All available props for the Blog1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog7.tsx`

**Component usage path:**  `src/app/blocks/blog/blog7/page.tsx`

**Preview link:** [https://stage.saasable.io/blocks/blog/blog7](https://stage.saasable.io/blocks/blog/blog7)

## Props Details

| Prop        | Type                  | Description                   | Displayed as                              |
| ----------- | --------------------- | ----------------------------- | ----------------------------------------- |
| **heading** | `string`              | Title of the blog section     | `"Latest Blog Posts"`                     |
| **blogs**   | `Array` of `BlogItem` | List of individual blog posts | See the `Example Structure` section above |

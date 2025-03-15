---
description: >-
  The Blog2 component presents a blog section with a central slider that
  displays blog cards featuring images, titles, and links to blog posts, along
  with a heading and caption.
---

# Blog2

{% hint style="info" %}
All available props for the Blog2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog2.tsx`

**Component usage path:**  `src/app/blocks/blog/blog2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog2](https://www.saasable.io/blocks/blog/blog2)



## Props Details

| Prop        | Type          | Description                                                                                           | Displayed as                              |
| ----------- | ------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| **heading** | `string`      | The main title for the blog section.                                                                  | "Latest News"                             |
| **caption** | `string`      | A subtitle or description for the blog section, providing more context to the heading.                | "Stay updated with our latest blog posts" |
| **blogs**   | `Array<Blog>` | An array of blog objects, each representing an individual blog post with an image, caption, and link. | See the JSON example above.               |

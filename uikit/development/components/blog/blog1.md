---
description: >-
  The Blog1 component displays a blog section with a heading, caption, and a
  slider of blog cards featuring images, titles, and clickable links to
  individual blog posts.
---

# Blog1

{% hint style="info" %}
All available props for the Blog1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog1.tsx`

**Component usage path:**  `src/app/blocks/blog/blog1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/blog/blog1](https://www.saasable.io/blocks/blog/blog1)

## Props Details

| Prop        | Type                | Description                                                                                                                      | Displayed as                                                                                                                                                        |
| ----------- | ------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | This is the main title for the blog section, which gives an overview or main topic of the blog posts.                            | The `heading` is prominently displayed at the top of the component inside the `Typeset` component, setting the context for the blog posts.                          |
| **caption** | `string` (optional) | An optional subheading that provides additional context or a brief description related to the blog posts.                        | The `caption` is shown below the `heading` within the `Typeset` component, offering more details about the blog section.                                            |
| **blogs**   | `BlogProps[]`       | An array of blog data objects, where each object includes properties like an image, a caption, and a link to the full blog post. | Each blog post is rendered as a card within a slider, displaying the image as the background, the caption as the blog title, and a clickable link to the full post. |


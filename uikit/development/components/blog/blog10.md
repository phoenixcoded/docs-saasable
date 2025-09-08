---
description: >-
  Blog10 is a responsive MUI React component that displays a featured blog post
  alongside a grid of additional blog cards using GraphicsCard, Typeset, and
  custom layout components.
---

# Blog10

{% hint style="info" %}
All available props for the Blog10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the blog section.
{% endhint %}

**Component path**: `src/blocks/blog/Blog10.tsx`

**Component usage path:**  `src/app/blocks/blog/blog10/page.tsx`

**Preview link:** [https://stage.saasable.io/blocks/blog/blog9](https://stage.saasable.io/blocks/blog/blog9)

## Props Details

| Prop        | Type                                       | Description                                        | Displayed as                                                   |
| ----------- | ------------------------------------------ | -------------------------------------------------- | -------------------------------------------------------------- |
| headLine    | `string`                                   | Main title of the blog section.                    | Top of the section in large font (via `Typeset` component).    |
| captionLine | `string`                                   | Short subheading or explanation below the heading. | Below the heading (via `Typeset`).                             |
| blog        | `BlogListProps`                            | The featured blog (main highlighted blog post)     | Shown at the top with image, chips, title, date, and link      |
| blogs       | <p><code>BlogListProps[]</code></p><p></p> | List of additional blog cards                      | Rendered in a grid, each showing image, chips, title, and date |

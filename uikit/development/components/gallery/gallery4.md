---
description: >-
  The Gallery4 component is a responsive image gallery with tab navigation,
  carousel slider, and lightbox functionality, allowing users to view and
  organize images by topics.
---

# Gallery4

{% hint style="info" %}
All available props for the Gallery4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the gallery section.
{% endhint %}

**Component path**: `src/blocks/gallery/Gallery4.tsx`

**Component usage path:**  `src/app/blocks/gallery/gallery4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/gallery/gallery4**](https://www.saasable.io/blocks/gallery/gallery4)

## Props Details

| Prop        | Type                 | Description                                                                                                                             | Displayed as                                                                             |
| ----------- | -------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| **heading** | `string`             | The main title or heading of the gallery.                                                                                               | `"Our Latest Projects"`                                                                  |
| **caption** | `string` (Optional)  | A caption or description providing context for the gallery.                                                                             | `"Explore the latest designs and innovations we've been working on."`                    |
| **topics**  | `string[]`           | An array of strings representing different topics or categories for filtering the gallery content.                                      | `["Web Design", "Mobile Apps", "Graphic Design"]`                                        |
| **images**  | `GalleryImageList[]` | An array of objects each containing image data. Each object may include properties like `src` (image source) and `index` (image index). | `[{ src: '/images/project1.jpg', index: 0 }, { src: '/images/project2.jpg', index: 1 }]` |

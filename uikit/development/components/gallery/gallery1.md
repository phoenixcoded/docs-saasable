---
description: >-
  This Gallery1 component renders a heading caption and responsive grid of
  images. Clicking on any image opens it in a lightbox for a larger view.
---

# Gallery1

{% hint style="info" %}
All available props for the Gallery1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the gallery section.
{% endhint %}

**Component path**: `src/blocks/gallery/Gallery1.tsx`

**Component usage path:**  `src/app/blocks/gallery/gallery1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/gallery/gallery1**](https://www.saasable.io/blocks/gallery/gallery1)

## Props Details

| Prop        | Type                 | Description                                               | Displayed as                                                       |
| ----------- | -------------------- | --------------------------------------------------------- | ------------------------------------------------------------------ |
| **heading** | `string`             | Main title of the gallery section.                        | `"Nature Photography"`                                             |
| **caption** | `string` (Optional)  | Brief description or caption for the gallery.             | `"A collection of beautiful nature photographs"`                   |
| **images**  | `GalleryImageList[]` | Array containing image objects, each with `src` property. | `[ { src: '/images/photo1.jpg' }, { src: '/images/photo2.jpg' } ]` |

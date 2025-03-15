# Gallery2

The `Gallery2` component displays a gallery of images in a responsive grid layout. Clicking an image opens it in a lightbox for a larger view. The grid layout adjusts based on the number of images provided.



{% hint style="info" %}
All available props for the Gallery2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the gallery section.
{% endhint %}

**Component path**: `src/blocks/gallery/Gallery2.tsx`

**Component usage path:**  `src/app/blocks/gallery/gallery2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/gallery/gallery2**](https://www.saasable.io/blocks/gallery/gallery2)

## Props Details

| Prop        | Type                 | Description                                               | Displayed as                                                       |
| ----------- | -------------------- | --------------------------------------------------------- | ------------------------------------------------------------------ |
| **heading** | `string`             | Main title of the gallery section.                        | `"Nature Photography"`                                             |
| **caption** | `string` (Optional)  | Brief description or caption for the gallery.             | `"A collection of beautiful nature photographs"`                   |
| **images**  | `GalleryImageList[]` | Array containing image objects, each with `src` property. | `[ { src: '/images/photo1.jpg' }, { src: '/images/photo2.jpg' } ]` |

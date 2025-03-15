# Gallery3

The `Gallery3` component in your code is designed to display a gallery with images, including a heading and caption. Here's an explanation of the `heading`, `caption`, and `images` props, along with a table to summarize their content.



{% hint style="info" %}
All available props for the Gallery3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the gallery section.
{% endhint %}

**Component path**: `src/blocks/gallery/Gallery3.tsx`

**Component usage path:**  `src/app/blocks/gallery/gallery3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/gallery/gallery3**](https://www.saasable.io/blocks/gallery/gallery3)

## Props Details

| Prop          | Type                 | Description                                                                                                                                                                        | Displayed as                                                                                  |
| ------------- | -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| **`heading`** | `string`             | The main title for the gallery section                                                                                                                                             | `"Nature Photography"`                                                                        |
| **`caption`** | `string` (Optional)  | A descriptive subtitle for the gallery section                                                                                                                                     | `"A collection of stunning nature shots"`                                                     |
| **`images`**  | `GalleryImageList[]` | <table data-header-hidden><thead><tr><th></th></tr></thead><tbody><tr><td>Array of image objects with <code>src</code> and <code>index</code> properties</td></tr></tbody></table> | `[ { src: '/path/to/image1.jpg', index: 0 }, { src: '/path/to/image2.jpg', index: 1 }, ... ]` |

# Hero8

The `Hero8` component displays a hero section with a headline, caption, optional primary button, and a responsive image. It includes a grid layout for a list of items, each featuring a counter and caption, with responsive adjustments for different screen sizes.

{% hint style="info" %}
All available props for the Hero8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero8.tsx`

**Component usage path:**  `src/app/blocks/hero/hero8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero8**](https://www.saasable.io/blocks/hero/hero8)

## Props Details

| Prop            | Type                     | Description                                              | Displayed as                                                                                                                         |
| --------------- | ------------------------ | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **headLine**    | `ReactElement`           | Main headline text                                       | `<Typography variant="h1">Our Key Features</Typography>`                                                                             |
| **captionLine** | `string`                 | Subtitle or descriptive text                             | `"Discover the key features that make our product unique."`                                                                          |
| **primaryBtn**  | `ButtonProps` (Optional) | Optional properties for the primary button.              | `{ variant: "contained", color: "primary", children: "Learn More" }`                                                                 |
| **image**       | `ImageCommonProps`       | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **listData**    | `ListDataProps[]`        | Array of data objects for the grid                       | `[{ counter: "10", caption: "Years in Business", defaultUnit: "years" }, ...]`                                                       |

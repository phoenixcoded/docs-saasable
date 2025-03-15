# Feature11

The `Feature11` component presents a section with a heading and optional caption, followed by an optional image inside a `GraphicsCard`. Below the image, a grid of animated `IconCard` components displays feature details.



{% hint style="info" %}
All available props for the Feature11 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature11.tsx`

**Component usage path:**  `src/app/blocks/feature/feature11/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature11**](https://www.saasable.io/blocks/feature/feature11)

## Props Details

| Prop           | Type                          | Description                                              | Displayed as                                                                                                                         |
| -------------- | ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**    | `string`                      | Main heading for the feature section                     | `"Our Key Features"`                                                                                                                 |
| **caption**    | `string` (Optional)           | Additional context or description under the heading.     | `"Discover the features that will transform your customer relationships"`                                                            |
| **image**      | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **features**   | `IconCardProps[]`             | Array of feature details to display                      | `[ { icon: 'icon-name1', title: 'Feature 1', content: 'Description of Feature 1', animationDelay: 0.3 }, ... ]`                      |
| **showBorder** | `boolean` (Optional)          | Optional prop for display border around image.           | Default it will show border around image.                                                                                            |

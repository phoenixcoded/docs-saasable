# Feature17

The `Feature17` component renders a section featuring a heading, caption, a series of icon cards, and an optional action button. It displays an image on one side and the icon cards on the other, with responsive layouts adjusting the image's position based on screen size.

{% hint style="info" %}
All available props for the Feature17 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature17.tsx`

**Component usage path:**  `src/app/blocks/feature/feature17/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature17**](https://www.saasable.io/blocks/feature/feature17)

## Props Details

| Prop          | Type                     | Description                                              | Displayed as                                                                                                                         |
| ------------- | ------------------------ | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**   | `string`                 | Main title of the section.                               | `"Our Outstanding Features"`                                                                                                         |
| **caption**   | `string`                 | Brief description under the heading.                     | `"Explore the key features that make our product..."`                                                                                |
| **features**  | `IconCardProps[]`        | Array of feature objects with icon, title, and content.  | `[ { icon: "feature-icon-1", title: "Feature One", content: "This feature provides value..." }, ... ]`                               |
| **image**     | `ImageCommonProps`       | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **actionBtn** | `ButtonProps` (Optional) | Properties for an optional action button.                | Rendered above cards if provided, enabling user interaction.                                                                         |

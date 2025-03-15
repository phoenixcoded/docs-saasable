# Feature13

The `Feature13` component displays a section with a centered heading and caption, a primary action button with an icon, and a list of feature cards with icons and descriptions. It also optionally includes an image in a `GraphicsCard` that is responsive to different screen sizes.

{% hint style="info" %}
All available props for the Feature13 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature13.tsx`

**Component usage path:**  `src/app/blocks/feature/feature13/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature13**](https://www.saasable.io/blocks/feature/feature13)

## Props Details

| Prop          | Type                 | Description                                              | Displayed as                                                                                                                         |
| ------------- | -------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**   | `string`             | Main heading for the feature section                     | `"Discover Our Features"`                                                                                                            |
| **caption**   | `string` (Optional)  | Additional subtitle or description.                      | `"Discover the unique aspects of our product"`                                                                                       |
| **actionBtn** | `ButtonProps`        | Props for the action button                              | `{ variant: 'contained', color: 'primary', children: 'Learn More' }`                                                                 |
| **cards**     | `FeatureCardProps[]` | Array of feature cards to display                        | `[ { icon: 'icon-name1', title: 'Feature 1', description: 'Description of Feature 1' }, ... ]`                                       |
| **image**     | (Optional)           | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |

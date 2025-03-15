# Feature14

The `Feature14` component displays a feature section with a heading, two graphics cards with titles and descriptions, and a list of feature cards with icons and descriptions, all styled and responsive based on the theme and screen size.

{% hint style="info" %}
All available props for the Feature14 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature14.tsx`

**Component usage path:**  `src/app/blocks/feature/feature14/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature14**](https://www.saasable.io/blocks/feature/feature14)

## Props Details

| Prop             | Type                 | Description                              | Displayed as                                                                                                                            |
| ---------------- | -------------------- | ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`             | Main heading for the feature section     | `"Explore Our Features"`                                                                                                                |
| **title**        | `string`             | Title for the first image section        | `"Feature Title 1"`                                                                                                                     |
| **description**  | `string`             | Description for the first image section  | `"This is a detailed description of the first feature."`                                                                                |
| **title2**       | `string`             | Title for the second image section       | `"Feature Title 2"`                                                                                                                     |
| **description2** | `string`             | Description for the second image section | `"This is a detailed description of the second feature."`                                                                               |
| **actionBtn**    | `ButtonProps`        | Props for the main action button         | `{ variant: 'contained', color: 'primary', children: 'Learn More' }`                                                                    |
| **cards**        | `FeatureCardProps[]` | Array of feature cards to display        | `[ { icon: 'icon-name1', title: 'Feature 1', description: 'Description of Feature 1' }, ... ]`                                          |
| **image1**       | `ImageCommonProps`   | Props for the first image                | <p><code>"path-to-image1.svg"</code><br> or <br><code>{ light: 'path-to-image1-light.svg', dark: 'path-to-image1-dark.svg' }</code></p> |
| **image2**       | `ImageCommonProps`   | Props for the second image               | <p><code>"path-to-image2.svg"</code><br> or <br><code>{ light: 'path-to-image2-light.svg', dark: 'path-to-image2-dark.svg' }</code></p> |

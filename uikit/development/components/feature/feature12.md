# Feature12

The `Feature12` component presents a section with a primary heading and caption, followed by a list of feature icons. It includes a secondary section with a heading, caption, and two buttons, one with an icon. Additionally, it displays an optional image in a `GraphicsCard` layout.

{% hint style="info" %}
All available props for the Feature12 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature12.tsx`

**Component usage path:**  `src/app/blocks/feature/feature12/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature12**](https://www.saasable.io/blocks/feature/feature12)

## Props Details

| Prop            | Type                          | Description                                              | Displayed as                                                                                                                         |
| --------------- | ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**     | `string`                      | Main heading for the feature section                     | `"Our Amazing Features"`                                                                                                             |
| **caption**     | `string` (Optional)           | Additional subtitle or description.                      | `"Discover the unique aspects of our product"`                                                                                       |
| **heading2**    | `string`                      | Secondary heading for detailed section                   | `"More Details"`                                                                                                                     |
| **caption2**    | `string`                      | Secondary caption for additional information             | `"Learn more about our additional offerings."`                                                                                       |
| **primaryBtn**  | `ButtonProps`                 | Props for the primary button                             | `{ variant: 'contained', color: 'primary', children: 'Get Started' }`                                                                |
| **primaryBtn2** | `ButtonProps`                 | Props for the secondary button                           | `{ variant: 'outlined', color: 'primary', children: 'Learn More' }`                                                                  |
| **icon**        | `SpriteIconProps` (Optional)  | Props for the primary icon used in the button            | `{ name: 'icon-name', size: 16 }`                                                                                                    |
| **icon2**       | `SpriteIconProps` (Optional)  | Props for the secondary icon used in the button          | `{ name: 'icon-name2', size: 16 }`                                                                                                   |
| **image**       | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **features**    | `IconCardProps[]`             | Array of feature details to display                      | `[ { icon: 'icon-name1', title: 'Feature 1', content: 'Description of Feature 1' }, ... ]`                                           |

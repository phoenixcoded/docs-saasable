# Feature21

The `Feature21` component is a responsive and animated section that features a heading, optional caption, an image with specific styling, and a grid of icon cards. It includes primary and secondary buttons, all enhanced with Framer Motion animations for visual effects.

{% hint style="info" %}
All available props for the Feature21 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature21.tsx`

**Component usage path:**  `src/app/blocks/feature/feature21/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature21**](https://www.saasable.io/blocks/feature/feature21)

## Props Details

| Prop             | Type                          | Description                                              | Displayed as                                                                                                                             |
| ---------------- | ----------------------------- | -------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                      | Main title of the section.                               | `"Our Key Features"`                                                                                                                     |
| **caption**      | `string` (Optional)           | Additional description or subtitle                       | Optional subtitle or descriptive text.                                                                                                   |
| **image**        | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p>     |
| **features**     | `IconCardProps[]`             | Array of features to display as icon cards.              | `[ { "icon": "icon1", "title": "Feature 1", "animationDelay": 0.2 }, { "icon": "icon2", "title": "Feature 2", "animationDelay": 0.3 } ]` |
| **primaryBtn**   | `ButtonProps` (Optional)      | Properties for the primary action button.                | Optional primary button properties.                                                                                                      |
| **secondaryBtn** | `ButtonProps` (Optional)      | Properties for the secondary action button.              | Optional secondary button properties.                                                                                                    |

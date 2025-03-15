# Feature20

The `Feature20` component is a responsive section that displays a heading and caption, a grid of feature cards with icons and text, and action buttons. It uses Material-UI for layout and styling, Framer Motion for animations, and adapts to different screen sizes to ensure a clean presentation.

{% hint style="info" %}
All available props for the Feature20 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature20.tsx`

**Component usage path:**  `src/app/blocks/feature/feature20/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature20**](https://www.saasable.io/blocks/feature/feature20)

## Props Details

| Prop             | Type                          | Description                                              | Displayed as                                                                                                                         |
| ---------------- | ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                      | Main title of the feature section.                       | `"Discover Our Key Features"`                                                                                                        |
| **caption**      | `string`                      | Additional description or subtitle                       | `"Explore the features that make our product stand out."`                                                                            |
| **image**        | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **features**     | `IconCardProps[]`             | Array of feature objects with icons and text.            | `[ { "icon": "icon1", "title": "Feature 1", "content": "Details" }, ... ]`                                                           |
| **actionBtn**    | `ButtonProps` (Optional)      | Properties for the primary action button.                | `{ "variant": "contained", "color": "primary", "children": "Get Started" }`                                                          |
| **secondaryBtn** | `ButtonProps` (Optional)      | Properties for the secondary action button.              | Optional properties for a secondary button.                                                                                          |

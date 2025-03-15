# Feature19

The `Feature19` component is a responsive layout featuring a header with optional caption, content blocks with images and descriptions, and action buttons, utilizing Material-UI for styling and layout, and applying gradient overlays for enhanced visual effects.

{% hint style="info" %}
All available props for the Feature19 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature19.tsx`

**Component usage path:**  `src/app/blocks/feature/feature19/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature19**](https://www.saasable.io/blocks/feature/feature19)

## Props Details

| Prop           | Type                | Description                                                 | Displayed as                                                                                                                                                                                                                          |
| -------------- | ------------------- | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`            | Main title of the feature section.                          | `"Our Exciting Features"`                                                                                                                                                                                                             |
| **caption**    | `string` (Optional) | Additional description or subtitle                          | Optional caption text below the heading.                                                                                                                                                                                              |
| **blockData1** | `BlockProps`        | Properties for the first block, including image and button. | `{ "title": "Feature 1", "description": "Description for feature 1.", "image": { "src": "/path/to/image1.jpg", "alt": "Feature 1 Image" }, "actionBtn": { "variant": "outlined", "color": "primary", "children": "Learn More" } }`    |
| **blockData2** | `BlockProps`        | Properties for the second block, similar to `blockData1`.   | `{ "title": "Feature 2", "description": "Description for feature 2.", "image": { "src": "/path/to/image2.jpg", "alt": "Feature 2 Image" }, "actionBtn": { "variant": "outlined", "color": "primary", "children": "Discover More" } }` |
| **blockData3** | `BlockProps2`       | Properties for the third block, with only description.      | `{ "description": "Description for the third block." }`                                                                                                                                                                               |
| **blockData4** | `BlockProps2`       | Properties for the fourth block, similar to `blockData3`.   | `{ "description": "Description for the fourth block." }`                                                                                                                                                                              |

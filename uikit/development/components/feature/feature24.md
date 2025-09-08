# Feature24

This code defines a React component `Feature24` that displays a section with a heading, optional caption, and a grid of icon cards. Each icon card presents an icon, title, and content. Below the grid, a graphics card may be rendered, containing a secondary heading, caption, and an optional image alongside a primary button. The layout is structured using MUI's `Grid`, `Stack`, and other components for responsive design.

{% hint style="info" %}
All available props for the Feature23 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature24.tsx`

**Component usage path:**  `src/app/blocks/feature/feature24/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/feature/feature23)[**https://stage.saasable.io/blocks/feature/feature24**](https://stage.saasable.io/blocks/feature/feature24)

## Props Details

| Prop        | Type                          | Description                                                                                              | Display As                                                                                                   |
| ----------- | ----------------------------- | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **heading** | `string`                      | The title or heading that is displayed at the top of the section.                                        | Displayed as the main title of the section.                                                                  |
| **caption** | `string` (Optional)           | Optional subtitle or brief description for the section.                                                  | Displayed below the main heading.                                                                            |
| **image**   | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path.                                                 | Displayed as an image on the right side of the card (if provided).                                           |
| **list**    | `FeatureListProps[]`          | An array of objects where each object represents a feature card, containing an icon, title, and content. | Displayed as feature cards in a grid layout.                                                                 |
| description | `string` or `ReactNode`       | A paragraph or component explaining the section in more detail.                                          | If it's a string, it’s displayed as `<Typography variant="h6">` if it's a component, it’s rendered directly. |

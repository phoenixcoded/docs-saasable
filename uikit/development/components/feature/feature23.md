# Feature23

This code defines a React component `Feature23` that displays a section with a heading, optional caption, and a grid of icon cards. Each icon card presents an icon, title, and content. Below the grid, a graphics card may be rendered, containing a secondary heading, caption, and an optional image alongside a primary button. The layout is structured using MUI's `Grid`, `Stack`, and other components for responsive design.

{% hint style="info" %}
All available props for the Feature23 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature23.tsx`

**Component usage path:**  `src/app/blocks/feature/feature23/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/feature/feature23)[**https://www.saasable.io/blocks/feature/feature23**](https://www.saasable.io/blocks/feature/feature23)

## Props Details

| Prop           | Type                          | Description                                                                                              | Display As                                                         |
| -------------- | ----------------------------- | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **heading**    | `string`                      | The title or heading that is displayed at the top of the section.                                        | Displayed as the main title of the section.                        |
| **caption**    | `string` (Optional)           | Optional subtitle or brief description for the section.                                                  | Displayed below the main heading.                                  |
| **heading2**   | `string`                      | The title for the second part of the section (inside the `GraphicsCard`).                                | Displayed as a heading inside the card.                            |
| **caption2**   | `string`                      | Description or caption for the second part of the section (inside the `GraphicsCard`).                   | Displayed below `heading2` as secondary text.                      |
| **primaryBtn** | `ButtonProps` (Optional)      | Contains button properties for the primary button, like `variant`, `color`, etc.                         | Displayed as a primary button (if provided).                       |
| **image**      | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path.                                                 | Displayed as an image on the right side of the card (if provided). |
| **features**   | `IconCardProps[]`             | An array of objects where each object represents a feature card, containing an icon, title, and content. | Displayed as feature cards in a grid layout.                       |

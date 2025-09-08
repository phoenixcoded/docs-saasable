# Feature22

This code defines a React component `Feature22` that dynamically renders a grid of feature cards based on the screen size, with animations using `framer-motion` and layout styling via MUI. Each card includes an image, title, content, and optional action buttons, using responsive design to adjust the number of columns.

{% hint style="info" %}
All available props for the Feature22 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature22.tsx`

**Component usage path:**  `src/app/blocks/feature/feature22/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature22**](https://www.saasable.io/blocks/feature/feature22)

## Props Details

| Prop         | Type               | Description                                                                                                                                            | Display As                                  |
| ------------ | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------- |
| **heading**  | `string`           | The title or heading that is displayed at the top of the feature section.                                                                              | Displayed as the main title of the section. |
| **features** | `ImageCardProps[]` | An array of objects where each object contains data for a feature card. Each card can include an image, title, content, and an optional action button. | Displays feature cards in a grid layout.    |
| caption      | `string`           | A subtitle below the heading, also centered.                                                                                                           | Subheading under `heading`, if provided     |


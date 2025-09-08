# Feature25

This code defines a React component `Feature25` that displays a section with a heading, optional caption, and a grid of icon cards. Each icon card presents an icon, title, and content. Below the grid, a graphics card may be rendered, containing a secondary heading, caption, and an optional image alongside a primary button. The layout is structured using MUI's `Grid`, `Stack`, and other components for responsive design.

{% hint style="info" %}
All available props for the Feature23 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature25.tsx`

**Component usage path:**  `src/app/blocks/feature/feature25/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/feature/feature23)[**https://stage.saasable.io/blocks/feature/feature25**](https://stage.saasable.io/blocks/feature/feature25)

## Props Details

| Prop        | Type                | Description                                                       | Display As                                                                                                                    |
| ----------- | ------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`            | The title or heading that is displayed at the top of the section. | Displayed as the main title of the section.                                                                                   |
| **caption** | `string` (Optional) | Optional subtitle or brief description for the section.           | Displayed below the main heading.                                                                                             |
| topics      | `TopicsProps[]`     | Array of topic objects used to create each tab and its content.   | Each topic is displayed as a tab with icon and title, and its panel shows the image, title, description, and optional button. |

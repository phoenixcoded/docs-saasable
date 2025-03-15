# Feature10

The `Feature10` component displays a section with a heading, caption, and a split grid of animated icon cards. It also includes a video thumbnail that, when clicked, opens a modal with the video player. It supports optional primary and secondary buttons for additional actions.



{% hint style="info" %}
All available props for the Feature10component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature10.tsx`

**Component usage path:**  `src/app/blocks/feature/feature10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature10**](https://www.saasable.io/blocks/feature/feature10)

## Props Details

| Prop                | Type                                                    | Description                                          | Displayed as                                                                                               |
| ------------------- | ------------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                                | Main heading for the feature section                 | `"Explore Our Features"`                                                                                   |
| **caption**         | `string` (Optional)                                     | Additional context or description under the heading. | `"Discover the features that will transform your customer relationships"`                                  |
| **features**        | `IconCardProps[]`                                       | Array of feature details to display                  | `[ { icon: 'icon1', title: 'Feature 1', content: 'Description of Feature 1', animationDelay: 0.3 }, ... ]` |
| **video**           | `{ thumbnail: string; src: string; overlay?: boolean }` | Video thumbnail, source and optional overlay         | `{ thumbnail: '/path/to/thumbnail.jpg', src: '/path/to/video.mp4' }`                                       |
| **typesetPosition** | `StackProps['textAlign']` (Optional)                    | Optional text alignment for heading and caption      | It will display an aligned heading and caption.                                                            |
| **primaryBtn**      | `ButtonProps` (Optional)                                | Optional primary button configuration                | `{ children: 'Buy Figma' }`                                                                                |
| **secondaryBtn**    | `ButtonProps` (Optional)                                | Optional secondary button configuration              | `{ children: 'Live Figma Preview' }`                                                                       |

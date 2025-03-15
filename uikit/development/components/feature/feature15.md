# Feature15

The `Feature15` component renders a section with a heading, optional caption, and four cards, each displaying an image, title, description, and additional features or actions, arranged in a responsive grid layout.

{% hint style="info" %}
All available props for the Feature15 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature15.tsx`

**Component usage path:**  `src/app/blocks/feature/feature15/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature15**](https://www.saasable.io/blocks/feature/feature15)

## Props Details

| Prop           | Type                | Description                                        | Displayed as                                                                                              |
| -------------- | ------------------- | -------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`            | Main heading for the section                       | `"Our Top Features"`                                                                                      |
| **caption**    | `string` (Optional) | Subheading or additional description below heading | `"Discover the standout features that make our product exceptional."`                                     |
| **blockData1** | `BlockProps`        | Data for the first feature block                   | `{ image: { src: 'image1.jpg', alt: 'Image 1' }, title: 'Feature 1', description: 'Description 1', ... }` |
| **blockData2** | `BlockProps`        | Data for the second feature block                  | `{ image: { src: 'image2.jpg', alt: 'Image 2' }, title: 'Feature 2', description: 'Description 2', ... }` |
| **blockData3** | `BlockProps`        | Data for the third feature block                   | `{ image: { src: 'image3.jpg', alt: 'Image 3' }, title: 'Feature 3', description: 'Description 3', ... }` |
| **blockData4** | `BlockProps`        | Data for the fourth feature block                  | `{ image: { src: 'image4.jpg', alt: 'Image 4' }, title: 'Feature 4', description: 'Description 4', ... }` |

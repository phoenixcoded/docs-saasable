# Feature27

`Feature27` is a responsive section component that displays a centered heading and caption followed by animated feature cards with icons, titles, and descriptions.

{% hint style="info" %}
All available props for the Feature27 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature27.tsx`

**Component usage path:**  `src/app/blocks/feature/feature27/page.tsx`

**Preview link:**[ ](https://www.saasable.io/blocks/feature/feature23)[**https://stage.saasable.io/blocks/feature/feature27**](https://stage.saasable.io/blocks/feature/feature27) &#x20;

## Props Details

| Prop    | Type               | Description                                                                 | Display As                                            |
| ------- | ------------------ | --------------------------------------------------------------------------- | ----------------------------------------------------- |
| heading | `string`           | The main title displayed at the top of the section.                         | `"Our Design Features"`                               |
| caption | `string`           | A brief subtitle or description below the heading.                          | `"Discover the power of modern graphics and design."` |
| feature | `ImageCardProps[]` | An array of feature items, each with image, title, and content description. | See table below                                       |

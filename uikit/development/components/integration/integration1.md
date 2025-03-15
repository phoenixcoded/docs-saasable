# Integration1

The `Integration1` component renders a section with two grids, one displaying a headline, caption, and a button, and the other showing a list of animated marquee tags with integration data, all styled with Material UI and Framer Motion for animations.

{% hint style="info" %}
All available props for the Integration1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration1.tsx`

**Component usage path:**  `src/app/blocks/integration/integration1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration1**](https://www.saasable.io/blocks/integration/integration1)

## Props Details

| Prop            | Type                  | Description                                            | Displayed as                                       |
| --------------- | --------------------- | ------------------------------------------------------ | -------------------------------------------------- |
| **headLine**    | `string`              | Main heading text                                      | `"Our Innovative Solutions"`                       |
| **captionLine** | `string`              | Secondary descriptive text                             | `"Discover the features that make us stand out"`   |
| **primaryBtn**  | `ButtonProps`         | Properties for the primary button                      | `{ variant: 'contained', children: 'Learn More' }` |
| **marquees**    | `MarqueesDataProps[]` | Array of marquee sections with properties and tag data | `[{ marqueeProps: { speed: 50 }, data: [...] }]`   |

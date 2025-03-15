# Feature16

The `Feature16` component displays a section with a heading, optional caption, a button, and a list of feature cards within a responsive layout, organized using a grid system and styled with Material-UI components.



{% hint style="info" %}
All available props for the Feature16 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature16.tsx`

**Component usage path:**  `src/app/blocks/feature/feature16/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature16**](https://www.saasable.io/blocks/feature/feature16)

## Props Details

| Prop          | Type                 | Description                        | Displayed as                                                                                   |
| ------------- | -------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------- |
| **heading**   | `string`             | Main title for the feature section | `"Our Innovative Features"`                                                                    |
| **caption**   | `string` (Optional)  | Additional description or subtitle | `"Explore the features that make our product stand out."`                                      |
| **actionBtn** | `ButtonProps`        | Props for the main action button   | `{ variant: 'contained', color: 'primary', children: 'Get Started' }`                          |
| **cards**     | `FeatureCardProps[]` | Array of feature card data         | `[ { icon: 'icon-name1', title: 'Feature 1', description: 'Description of Feature 1' }, ... ]` |

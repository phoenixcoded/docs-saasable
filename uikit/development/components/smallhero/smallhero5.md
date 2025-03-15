# SmallHero5

The `SmallHero5` React component that creates a centered hero section featuring a heading, caption, optional button, and a marquee list of items with chips, using Material-UI for styling and layout, and includes a background of circles.

{% hint style="info" %}
All available props for the SmallHero5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero5.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero5**](https://www.saasable.io/blocks/small-hero/small-hero5)

## Props Details

| Prop           | Type                     | Description                                                                                                | Displayed as                                             |
| -------------- | ------------------------ | ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| **heading**    | `string`                 | The main title or heading of the hero section.                                                             | `"Welcome to Our Latest Collection"`                     |
| **caption**    | `string`                 | An additional description or subheading below the main heading.                                            | `"Explore our range of new and exciting products."`      |
| **exploreBtn** | `ButtonProps` (Optional) | Configuration for an optional button, which can include properties like `href`, `onClick`, and `children`. | `{ href: '/explore', children: 'Explore Now' }`          |
| **list**       | `string[]`               | An array of strings displayed in a scrolling marquee.                                                      | `['Limited Time Offer', 'New Arrivals', 'Best Sellers']` |

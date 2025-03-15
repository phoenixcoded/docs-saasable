---
description: >-
  The SmallHero2 component renders a centered hero section with an optional
  chip, headline, and caption, styled with a background color for the chip.
---

# SmallHero2

{% hint style="info" %}
All available props for the SmallHero2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero2.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero2**](https://www.saasable.io/blocks/small-hero/small-hero2)

## Props Details

| Prop            | Type                                                          | Description                                                                                                 | Displayed as                                                  |
| --------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Displays a badge with optional linking. Can include a text label and a link.                                | `{ label: 'New!', link: { href: '/new', passHref: true } }`   |
| **headLine**    | `string \| ReactElement`                                      | The main heading or title of the hero section. It can be plain text or any React component.                 | `"Introducing Our Latest Product"`                            |
| **captionLine** | `string` (Optional)                                           | A subheading or additional description displayed below the headline. Provides context or additional detail. | `"Discover the features and benefits of our newest release."` |

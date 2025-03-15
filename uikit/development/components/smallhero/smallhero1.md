---
description: >-
  The SmallHero1 component displays a centered hero section with an optional
  chip, a headline, and a caption, all within a styled container.
---

# SmallHero1

{% hint style="info" %}
All available props for the SmallHero1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero1.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero1**](https://www.saasable.io/blocks/small-hero/small-hero1)

## Props Details

| Prop            | Type                                                          | Description                                                                                                            | Displayed as                                                  |
| --------------- | ------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | An optional badge or label, which can include a text label and an optional link.                                       | `{ label: 'New!', link: { href: '/new', passHref: true } }`   |
| **headLine**    | `string \| ReactElement`                                      | Main heading or title for the hero section. It can be a string, JSX, or other renderable React elements.               | `"Introducing Our Latest Product"`                            |
| **captionLine** | `string` (Optional)                                           | Subheading or additional context under the main headline. It can be a string, JSX, or other renderable React elements. | `"Discover the features and benefits of our newest release."` |

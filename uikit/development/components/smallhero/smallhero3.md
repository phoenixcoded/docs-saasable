---
description: >-
  The SmallHero3 component creates a hero section with a chip, headline,
  optional caption, and a configurable "explore" button, all arranged with
  responsive layout and spacing.
---

# SmallHero3

{% hint style="info" %}
All available props for the SmallHero3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero3.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero3**](https://www.saasable.io/blocks/small-hero/small-hero3)

## Props Details

| Prop            | Type                                                          | Description                                                                                  | Displayed as                                                |
| --------------- | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Displays a badge or label, potentially with a hyperlink.                                     | `{ label: 'New!', link: { href: '/new', passHref: true } }` |
| **headLine**    | `string \| ReactElement`                                      | The main title or heading for the hero section. It can be text or any React component.       | `"Explore Our Latest Collection"`                           |
| **captionLine** | `string` (Optional)                                           | A subheading or additional description displayed below the headline.                         | `"Discover the new range of products we just launched."`    |
| **exploreBtn**  | `ButtonProps` (Optional)                                      | Configuration for an optional button, which can include properties like `href` or `onClick`. | `{ href: '/explore', children: 'Explore Now' }`             |

---
description: >-
  The SmallHero6 component presents a hero section with a headline, tagline, an
  email sign-up input with a primary button, and a list of items with icons and
  titles arranged in a grid.
---

# SmallHero6

{% hint style="info" %}
All available props for the SmallHero6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the smallhero section.
{% endhint %}

**Component path**: `src/blocks/small-hero/SmallHero6.tsx`

**Component usage path:**  `src/app/blocks/small-hero/small-hero6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/small-hero/small-hero6**](https://www.saasable.io/blocks/small-hero/small-hero6)

## Props Details

| Prop           | Type                     | Description                                                                     | Displayed as                                                                                 |
| -------------- | ------------------------ | ------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| **headLine**   | `string \| ReactElement` | Main headline or title of the hero section.                                     | `"Join Our Community"`                                                                       |
| **tagline**    | `string`                 | Optional tagline or brief description displayed above the headline.             | `"Stay updated with the latest news and offers"`                                             |
| **list**       | `ListItem[]`             | Array of objects representing items to display, each with a `title` and `icon`. | `[{ title: "Feature 1", icon: "icon-name-1" }, { title: "Feature 2", icon: "icon-name-2" }]` |
| **primaryBtn** | `ButtonProps`            | Properties for the button inside the input field.                               | `{ onClick: handleClick, children: "Subscribe" }`                                            |

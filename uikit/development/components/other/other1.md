---
description: >-
  The Other1, which renders a section with a heading, description, and a list of
  animated cards, each linking to different pages, using Material-UI and Framer
  Motion for styling and animations.
---

# Other1

{% hint style="info" %}
All available props for the Other1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the other section.
{% endhint %}

**Component path**: `src/blocks/other/Other1.tsx`

**Component usage path:**  `src/app/blocks/other/other1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/other/other1**](https://www.saasable.io/blocks/other/other1)

## Props Details

| Prop Name       | Type             | Description                                                                                                                                          | Displayed as                                                                                                                               |
| --------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**     | `string`         | The main title of the component, displayed at the top.                                                                                               | `"Our Solutions"`                                                                                                                          |
| **description** | `string`         | A brief paragraph or text that provides more context about the sections. This is displayed below the sections grid.                                  | `"Discover how our services can help"`                                                                                                     |
| **primaryBtn**  | `ButtonProps`    | An object containing properties for the primary button, such as its text, variant, and click event.                                                  | `{ children: "Learn More", onClick: () => { console.log("Button clicked"); } }`                                                            |
| **sections**    | `SectionProps[]` | An array of section objects, each containing a title, subtitle, image, link, and optional animation delay. These represent different content blocks. | `[{ title: "AI Solutions", subTitle: "Explore our AI-driven tools", image: { src: "/images/ai.png" }, link: "/ai", animationDelay: 0.3 }]` |

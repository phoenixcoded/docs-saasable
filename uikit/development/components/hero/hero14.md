# Hero14

`Hero14` is a promotional hero section with a headline, caption, and tagline, featuring a call-to-action email sign-up form with a button, and a grid of list items with icons, all styled with MUI components and custom graphics.

{% hint style="info" %}
All available props for the Hero14 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero14.tsx`

**Component usage path:**  `src/app/blocks/hero/hero14/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero14**](https://www.saasable.io/blocks/hero/hero14)

## Props Details

| Prop            | Type                     | Description                                         | Displayed as                                                                |
| --------------- | ------------------------ | --------------------------------------------------- | --------------------------------------------------------------------------- |
| **headLine**    | `string \| ReactElement` | Main heading text or component.                     | `"Effortless CRM Management, Seamless BusinessGrowth"`                      |
| **captionLine** | `string` (Optional)      | Subheading or additional descriptive text.          | `"Explore the future of technology with our latest products and services."` |
| **tagline**     | `string`                 | A short, catchy phrase displayed above the heading. | `"Leading the Charge in Innovation"`                                        |
| **list**        | `ListItem[]`             | Array of items with icons and titles.               | `[ { title: "Feature 1", icon: { name: "icon-name-1" } }, ... ]`            |
| **primaryBtn**  | `ButtonProps`            | Properties for the primary button.                  | `{ variant: "contained", color: "primary", children: "Get Started" }`       |

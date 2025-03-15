# Hero12

`Hero12` is a hero section that features a marquee of chips with text, a headline and caption, a call-to-action button, and a decorative background with circles. The design utilizes MUI components and custom elements such as `GradientFab` and `SvgIcon`, with a responsive layout and styling.

{% hint style="info" %}
All available props for the Hero12 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero12.tsx`

**Component usage path:**  `src/app/blocks/hero/hero12/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero12**](https://www.saasable.io/blocks/hero/hero12)

## Props Details

| Prop            | Type                     | Description                                    | Displayed as                                                                                                  |
| --------------- | ------------------------ | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **headLine**    | `string \| ReactElement` | Main heading or title of the section.          | `"Empower Your Cloud Experience with Unmatched Optimization Precision"`                                       |
| **captionLine** | `string \| ReactElement` | Secondary line of text for additional context. | `"Seamlessly fine-tune and optimize your cloud resources using cutting-edge analytics and automation tools."` |
| **list**        | `string[]`               | List of items to display in the marquee.       | `["Feature 1", "Feature 2", "Feature 3", "Feature 4"]`                                                        |
| **exploreBtn**  | `ButtonProps`            | Properties for the "Explore" button.           | `{ variant: "contained", color: "primary", children: "Explore Now" }`                                         |

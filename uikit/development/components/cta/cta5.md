# Cta5

The `Cta5` component is a dynamic call-to-action section that includes a heading, buttons, input fields, sales data, avatar group profiles, and an optional description, utilizing Material UI components and animations from `framer-motion` for smooth transitions.

{% hint style="info" %}
All available props for the Cta5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta5.tsx`

**Component usage path:**  `src/app/blocks/cta/cta5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta5**](https://www.saasable.io/blocks/cta/cta5)

## Props Details

| Prop              | Type                                                   | Description                                            | Displayed as                                                   |
| ----------------- | ------------------------------------------------------ | ------------------------------------------------------ | -------------------------------------------------------------- |
| **heading**       | `string`                                               | Main heading or title of the section.                  | Displayed prominently at the top of the component.             |
| **caption**       | `string`                                               | Subtitle or secondary text below the heading.          | Provides additional context or detail.                         |
| **label**         | `string`                                               | Label or tag to emphasize a feature or characteristic. | Displayed as a `Chip` with a specific style.                   |
| **input**         | `boolean \| CtaInputProps` (Optional)                  | Optional prop for input field.                         | Whether to show an input field, and its properties if enabled. |
| **primaryBtn**    | `ButtonProps` (Optional)                               | Properties for the primary call-to-action button.      | Renders a prominent button for main actions.                   |
| **secondaryBtn**  | `ButtonProps` (Optional)                               | Properties for a secondary button.                     | Provides an alternative action.                                |
| **description**   | `string \| ReactElement` (Optional)                    | Optional prop for additional description.              | Additional descriptive text or content.                        |
| **saleData**      | `CTASaleProps`                                         | Information about a sale or special offer.             | Displayed with visual emphasis on the sale details.            |
| **profileGroups** | `{ avatarGroups: AvatarGroupProps[]; review: string }` | Contains user avatars and a review/testimonial text.   | Displays social proof and user testimonials.                   |

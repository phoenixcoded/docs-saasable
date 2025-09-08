# Hero19

`Hero19` is a responsive and customizable **Hero Section** component for landing pages or feature highlights. It displays a featured image alongside optional text content such as a tagline, headline, description, bullet list, and call-to-action buttons.

{% hint style="info" %}
All available props for the Hero19 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero19.tsx`

**Component usage path:**  `src/app/blocks/hero/hero19/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero19**](https://www.saasable.io/blocks/hero/hero19)

## Props Details

| Prop         | Type                                         | Description                                                                   | Displayed as                                                                     |
| ------------ | -------------------------------------------- | ----------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| image        | `ImageCommonProps`                           | Graphic shown on the left side.                                               | `{ src: '/images/hero-graphic.png', alt: 'Hero Section Graphic' }`               |
| tagline      | `string`                                     | Short label or slogan above the headline.                                     | `"Built for Developers"`                                                         |
| list         | Array<{ primary: string }`> (optional)`      | A bullet list rendered with checkmark icons, each `primary` is one list item. | `Shown as a List with icons and secondary text`                                  |
| headLine     | `{ image: string \| ImageComponentProps }[]` | Main bold title or heading.                                                   | `"Simplify Your Workflow with Our API"`                                          |
| description  | `string`                                     | Supporting text under the headline.                                           | `"Our RESTful API gives you full control, fast integration, and endless power."` |
| primaryBtn   | `ButtonProps`                                | Props for the primary call-to-action button (filled style).                   | `As a "contained" MUI Button`                                                    |
| secondaryBtn | `ButtonProps`                                | Props for the secondary call-to-action button (outlined style).               | `As an "outlined" MUI Button`                                                    |


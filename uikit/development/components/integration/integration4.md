# Integration4

The `Integration4` component displays a section with two grids: one showing a headline, caption, and button using `Typeset`, and the other featuring a rotating grid of integration avatars within a marquee animation, styled with Material UI. The component handles responsive layout adjustments and supports both LTR and RTL themes.

{% hint style="info" %}
All available props for the Integration4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration4.tsx`

**Component usage path:**  `src/app/blocks/integration/integration4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration4**](https://www.saasable.io/blocks/integration/integration4)

## Props Details

| Prop Name       | Type                  | Description                                    | Displayed as                                                                                                               |
| --------------- | --------------------- | ---------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **headLine**    | `string`              | Main heading or title text                     | `"Transform Your Business"`                                                                                                |
| **captionLine** | `string`              | Secondary line of text or caption              | `"Innovative solutions to elevate your company’s performance."`                                                            |
| **primaryBtn**  | `ButtonProps`         |  Properties for the primary button             | `{variant: 'contained', size: 'large', color: 'primary', onClick: () => alert('Button Clicked'), children: 'Get Started'}` |
| **marquees**    | `MarqueesDataProps[]` | Array of marquee objects with images and props | `[{ marqueeProps: { speed: 50 }, data: [...] }]`                                                                           |

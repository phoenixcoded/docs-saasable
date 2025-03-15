# Cta3

The `Cta3` component displays a call-to-action section with a headline, a primary button, marquee text, and optional background images, utilizing Material UI for layout and styling, and `react-fast-marquee` for scrolling elements.

{% hint style="info" %}
All available props for the Cta3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta3.tsx`

**Component usage path:**  `src/app/blocks/cta/cta3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta3**](https://www.saasable.io/blocks/cta/cta3)

## Props Details

| Prop           | Type                      | Description                                                                                              | Displayed as                                    |
| -------------- | ------------------------- | -------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| **bgImage1**   | `BgImageProps` (Optional) | URL of the background image for the first `GraphicsCard`. Optional.                                      | Sets the background image of the first card.    |
| **bgImage2**   | `BgImageProps` (Optional) | URL of the background image for the second `GraphicsCard`. Optional.                                     | Sets the background image of the second card.   |
| **heading**    | `string`                  | Main heading text displayed in the first `GraphicsCard`. Required.                                       | Displays the primary heading in the first card. |
| **primaryBtn** | `ButtonProps`             | Properties for the primary button, such as text, style, and click handlers. Required.                    | Renders a prominent button in the first card.   |
| **marquees**   | `MarqueesDataProps[]`     | Array of objects containing data for multiple `Marquee` components, each with tag information. Required. | Renders scrolling tags in the second card.      |

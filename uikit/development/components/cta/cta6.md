# Cta6

The `Cta6` component renders a call-to-action section featuring a heading, caption, email input with a button, and a client logo slider, using MUI and a custom layout that adjusts styles and behavior based on the theme.

{% hint style="info" %}
All available props for the Cta6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta6.tsx`

**Component usage path:**  `src/app/blocks/cta/cta6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta6**](https://www.saasable.io/blocks/cta/cta6)

## Props Details

| Prop              | Type                     | Description                                                                 | Displayed as                                     |
| ----------------- | ------------------------ | --------------------------------------------------------------------------- | ------------------------------------------------ |
| **heading**       | `string`                 | Main title or heading of the component.                                     | Displayed at the top to draw attention.          |
| **caption**       | `string`                 | Subtitle or secondary text that provides additional context or description. | Displayed below the heading.                     |
| **icon**          | `JSX.Element` (Optional) | Optional prop for displaying your custom icon in `GradientFab`              | Display icon in gradient fab section.            |
| **primaryBtn**    | `ButtonProps`            | Properties for the primary button within the input field.                   | Used as a call-to-action button inside the form. |
| **clienteleList** | `ClienteleListProps[]`   | Array of client logos or images to be displayed in a slider/carousel.       | Rendered as slides in a carousel.                |

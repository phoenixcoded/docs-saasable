# EarlyAccess

`The EarlyAccess` component that creates a responsive section with a full-height graphics card. It features a gradient floating action button with a logo, a typeset heading and caption, an input field with a button for email submissions, and a responsive image that adjusts based on the theme's direction.

{% hint style="info" %}
All available props for the EarlyAccess component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the EarlyAccess section.
{% endhint %}

**Component path**: `src/blocks/EarlyAccess.tsx`

**Component usage path:**  `src/app/blocks/early-access/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/early-access**](https://www.saasable.io/blocks/early-access)

## Props Details

| Prop           | Type               | Description                                                                                       | Displayed as                                                                                                                          |
| -------------- | ------------------ | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`           | A required string for the main title or heading in the component.                                 | `"Join Our Early Access Program"`                                                                                                     |
| **caption**    | `string`           | A required string for additional descriptive text or subtitle.                                    | `"Be the first to experience our new features. Sign up now!"`                                                                         |
| **image**      | `ImageCommonProps` | Image path or object with `light` and `dark` image path.                                          | <p><code>"path-to-image.svg"</code><br>  or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **primaryBtn** | `ButtonProps`      | A required object with properties for the button used as an end adornment in the `OutlinedInput`. | `{ children: 'Subscribe', onClick: () => alert('Subscribed!') }`                                                                      |

# Hero10

The `Hero10` component presents a visually striking section featuring a background image, a chip label, headline and caption text, and a pair of action buttons, with responsive adjustments for mobile and desktop views including a review profile group.

{% hint style="info" %}
All available props for the Hero10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero10.tsx`

**Component usage path:**  `src/app/blocks/hero/hero10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero10**](https://www.saasable.io/blocks/hero/hero10)

## Props Details

| Prop             | Type                                       | Description                                                                      | Displayed as                                                                                                                         |
| ---------------- | ------------------------------------------ | -------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **chipTitle**    | `string`                                   | Title text for the chip component.                                               | `"Featured"`                                                                                                                         |
| **headLine**     | `string \| ReactElement`                   | Main headline text, which can be a string or a React element.                    | `"Effortless Collaboration, Perfect Harmony"`                                                                                        |
| **captionLine**  | `string`                                   | Additional descriptive text below the headline.                                  | `"Experience the ultimate in innovation and technology."`                                                                            |
| **primaryBtn**   | `ButtonProps`                              | Properties for the primary button, including text and event handlers.            | `{ variant: "contained", color: "primary", children: "Get Started" }`                                                                |
| **secondaryBtn** | `ButtonProps`                              | Properties for the secondary button, styled differently from the primary button. | `{ variant: "outlined", color: "primary", children: "Learn More" }`                                                                  |
| **image**        | `ImageCommonProps`                         | Image path or object with `light` and `dark` image path.                         | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **`reviewData`** | `{ avatarList: string[], review: string }` | Data for the review section, including avatars and review text.                  | `{ avatarList: ["/avatars/user1.jpg", "/avatars/user2.jpg"], review: "This is a fantastic product!" }`                               |

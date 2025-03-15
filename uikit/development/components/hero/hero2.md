# Hero2

The `Hero2` component is a customizable hero section that utilizes Material-UI and Framer Motion to create an animated, visually appealing layout with optional chip, headline, caption, and buttons, alongside a background image with a gradient overlay and background dots pattern.

{% hint style="info" %}
All available props for the Hero2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero2.tsx`

**Component usage path:**  `src/app/blocks/hero/hero2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero2**](https://www.saasable.io/blocks/hero/hero2)

## Props Details

| Prop Name        | Type                                                          | Description                                                         | Displayed as                                                                                                                         |
| ---------------- | ------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **chip**         | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip with text and optional link.                          | `{ label: "New Feature", link: { href: "/features", passHref: true } }`                                                              |
| **headLine**     | `string \| ReactElement`                                      | Main headline for the hero section. Can be text or a React element. | `"Effortless CRM Management, Seamless BusinessGrowth"`                                                                               |
| **captionLine**  | `string` (Optional)                                           | Optional caption text for additional information.                   | `"Discover the most advanced features designed for your needs."`                                                                     |
| **image**        | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **primaryBtn**   | `ButtonProps` (Optional)                                      | Optional properties for the primary button.                         | `{ children: "Learn More", href: "/learn-more", variant: "contained", size: "large" }`                                               |
| **secondaryBtn** | `ButtonProps` (Optional)                                      | Optional properties for the secondary button.                       | `{ children: "Get Started", href: "/get-started", variant: "outlined", size: "large" }`                                              |

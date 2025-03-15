---
description: >-
  Hero7 component that displays a headline, caption, primary button, and images
  with decorative patterns, styled according to the theme's direction and
  responsive breakpoints.
---

# Hero7

{% hint style="info" %}
All available props for the Hero7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero7.tsx`

**Component usage path:**  `src/app/blocks/hero/hero7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero7**](https://www.saasable.io/blocks/hero/hero7)

## Props Details



| Prop            | Type                                   | Description                                              | Displayed as                                                                                                                         |
| --------------- | -------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **headLine**    | `ReactElement`                         | Main headline text                                       | `<Typography variant="h1">Innovate with Us</Typography>`                                                                             |
| **captionLine** | `string`                               | Subtitle or descriptive text                             | `"Empowering creativity and technology for the next generation."`                                                                    |
| **primaryBtn**  | `ButtonProps`                          | Properties for the primary button                        | `{ variant: "contained", color: "primary", children: "Get Started" }`                                                                |
| **image1**      | `BgImageProps`                         | Properties for the first background image                | `{ src: "/assets/images/background1.jpg", alt: "Decorative Background" }`                                                            |
| **image2**      | `ImageCommonProps`                     | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **reviewData**  | `{ rating: string; reviews: string; }` | Review rating and text                                   | `{ rating: "4.5/5", reviews: "Based on 250 reviews" }`                                                                               |

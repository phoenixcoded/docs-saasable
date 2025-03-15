# Hero1

The `Hero1` component is a hero section that combines scrolling effects with animations using Framer Motion and Material-UI. It features a customizable layout including optional chip, headline, caption, and buttons, along with a sticky image card that scales based on scroll position.

{% hint style="info" %}
All available props for the Hero1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero1.tsx`

**Component usage path:**  `src/app/blocks/hero/hero1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero1**](https://www.saasable.io/blocks/hero/hero1)

## Props Details

| Prop Name        | Type                                                          | Description                                                         | Displayed as                                                                                                                         |
| ---------------- | ------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **chip**         | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip component with text and an optional link.             | `{ label: "New Feature", link: { href: "/features", passHref: true } }`                                                              |
| **headLine**     | `string \| ReactElement`                                      | Main headline for the hero section. Can be text or a React element. | `"Effortless CRM Management, Seamless BusinessGrowth"`                                                                               |
| **captionLine**  | `string` (Optional)                                           | Optional caption text for additional information.                   | `"Explore the future of technology with our latest products and services."`                                                          |
| **image**        | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path.            | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **primaryBtn**   | `ButtonProps` (Optional)                                      | Optional properties for the primary button.                         | `{ children: "Learn More", href: "/learn-more", variant: "contained", size: "large" }`                                               |
| **secondaryBtn** | `ButtonProps` (Optional)                                      | Optional properties for the secondary button.                       | `{ children: "Get Started", href: "/get-started", variant: "outlined", size: "large" }`                                              |

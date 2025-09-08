# Hero4

The `Hero4` component is a section that includes a headline and caption, an optional chip, and two image blocks with decorative patterns. It features a responsive layout with a `Grid` layout for arranging images and a list of items, each displaying an icon and description, all wrapped in styled `GraphicsCard` components.

{% hint style="info" %}
All available props for the Hero4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero4.tsx`

**Component usage path:**  `src/app/blocks/hero/hero4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero4**](https://www.saasable.io/blocks/hero/hero4)

## Props Details

| Prop            | Type                                                          | Description                                              | Displayed as                                                                                                                                                                                                                                                |
| --------------- | ------------------------------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip component with text and an optional link.  | `{ label: "Learn More", link: { href: "/more-info" } }`                                                                                                                                                                                                     |
| **headLine**    | `string`                                                      | Main heading text                                        | `"Explore Our Latest Innovations"`                                                                                                                                                                                                                          |
| **captionLine** | `string`                                                      | Secondary caption text                                   | `"Discover groundbreaking technology and design."`                                                                                                                                                                                                          |
| **image1**      | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image1.svg"</code><br> or <br><code>{ light: 'path-to-image1-light.svg', dark: 'path-to-image1-dark.svg' }</code></p>                                                                                                                     |
| **image2**      | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image2.svg"</code><br> or <br><code>{ light: 'path-to-image2-light.svg', dark: 'path-to-image2-dark.svg' }</code></p>                                                                                                                     |
| **listData**    | `ListDataProps[]`                                             | List items with icon, title, and description             | `[{ icon: { name: "icon-design" }, title: "Design Excellence", description: "Innovative and user-centric designs." }, { icon: { name: "icon-technology" }, title: "Advanced Technology", description: "Cutting-edge technology for better performance." }]` |

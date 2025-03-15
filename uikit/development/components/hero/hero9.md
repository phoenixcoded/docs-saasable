# Hero9

The `Hero9` component creates a visually engaging hero section with a background featuring dotted patterns, a central content area with a chip label, headline, caption, and a call-to-action button, and a list of icons with titles. It also includes an image with a styled border and radius.

{% hint style="info" %}
All available props for the Hero9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero9.tsx`

**Component usage path:**  `src/app/blocks/hero/hero9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero9**](https://www.saasable.io/blocks/hero/hero9)

## Props Details

| Prop            | Type                            | Description                                                          | Displayed as                                                                                                                         |
| --------------- | ------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **chip**        | `{ label: ChipProps['label'] }` | Chip component with a label, either a string or custom element       | `{ label: 'New Feature' }`                                                                                                           |
| **headLine**    | `string`                        | Main headline text                                                   | `"Discover Our Latest Innovations"`                                                                                                  |
| **captionLine** | `string`                        | Secondary descriptive text                                           | `"Explore the cutting-edge features that are redefining the industry."`                                                              |
| **primaryBtn**  | `ButtonProps`                   | Properties for the primary button, including text and event handlers | `{ variant: "contained", color: "primary", children: "Get Started" }`                                                                |
| **image**       | `ImageCommonProps`              | Image path or object with `light` and `dark` image path.             | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **listData**    | `ListDataProps[]`               | Array of items with icons and titles to display                      | `[{ icon: "tabler-heart", title: "Loved by Users" }, { icon: "tabler-star", title: "Highly Rated" }]`                                |

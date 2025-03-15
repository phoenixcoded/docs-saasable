# Hero5

The `Hero5` component features a hero section with an optional chip, headline, caption, primary button, and a carousel of list items, each displaying an icon and text. It incorporates responsive styling and a background image with gradient effects, adapting to the theme's direction and using `react-slick` for the carousel.

{% hint style="info" %}
All available props for the Hero5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero5.tsx`

**Component usage path:**  `src/app/blocks/hero/hero5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero5**](https://www.saasable.io/blocks/hero/hero5)

## Props Details

| Prop            | Type                                                          | Description                                              | Displayed as                                                                                                                                                                                                                                                          |
| --------------- | ------------------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label']; link?: LinkProps; }` (Optional) | Optional chip component with text and an optional link.  | `{ label: "New Arrival", link: { href: "/new-arrival" } }`                                                                                                                                                                                                            |
| **headLine**    | `string`                                                      | Main heading text                                        | `"Discover the Future of Technology"`                                                                                                                                                                                                                                 |
| **captionLine** | `string`                                                      | Secondary caption text                                   | `"Innovative solutions for a smarter world."`                                                                                                                                                                                                                         |
| **image**       | `ImageCommonProps`                                            | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p>                                                                                                                                  |
| **primaryBtn**  | `ButtonProps` (Optional)                                      | Optional properties for the primary button.              | `{ variant: "contained", color: "primary", children: "Learn More" }`                                                                                                                                                                                                  |
| **listData**    | `ListDataProps[]`                                             | Items for the slider with icon, title, and description   | `[{ icon: { name: "icon-performance" }, title: "High Performance", description: "Experience unparalleled speed and efficiency." }, { icon: { name: "icon-innovation" }, title: "Cutting-Edge Innovation", description: "Stay ahead with the latest advancements." }]` |

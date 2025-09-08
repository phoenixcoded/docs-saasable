# Other3

The Other3 that renders a section with a heading, caption, and a list of cards displaying titles, descriptions, chips, and buttons, utilizing MUI's Stack, Chip, and Typography components for layout and styling.

{% hint style="info" %}
All available props for the Other3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the other section.
{% endhint %}

**Component path**: `src/blocks/other/Other3.tsx`

**Component usage path:**  `src/app/blocks/other/other3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/other/other3**](https://www.saasable.io/blocks/other/other3)

## Props Details

| Prop        | Type             | Description                                                       | Display As                                                          |
| ----------- | ---------------- | ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| **heading** | `string`         | The title or heading that is displayed at the top of the section. | Displayed as the main title of the section.                         |
| **caption** | `string`         | A description or subtitle for the section.                        | Displayed as a subtitle below the main heading.                     |
| exploreMore | ButtonProps      | "Explore More" button config                                      | Renders as a styled MUI `<Button>` with optional `href`             |
| categories  | CategoryProps\[] | Filter chips or tabs above content cards                          | Renders as horizontally scrollable `<Button>` elements (via Slider) |
| items       | Array            | Data for content cards (title, image, etc.)                       | Renders a grid of `<GraphicsCard>` for each item                    |

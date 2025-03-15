# Hero15

The `Hero15` component displays a hero section with a review profile, a heading and caption, an image, benefit data, and two call-to-action buttons, all arranged using MUI's responsive layout and themed with background images and overlays.

{% hint style="info" %}
All available props for the Hero15 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero15.tsx`

**Component usage path:**  `src/app/blocks/hero/hero15/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero15**](https://www.saasable.io/blocks/hero/hero15)

## Props Details

| Prop             | Type                                                              | Description                                              | Displayed as                                                                                                                         |
| ---------------- | ----------------------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **reviewData**   | `{ avatarList: string[]; rating: number; totalReviews: string; }` | User reviews information.                                | `{ avatarList: ['/path/to/avatar1.jpg'], rating: 4.5, totalReviews: '150 Reviews' }`                                                 |
| **heading**      | `string`                                                          | Main heading text for the hero section.                  | `"Discover the Best Services for Your Needs"`                                                                                        |
| **caption**      | `string` (Optional)                                               | Optional subheading or additional descriptive text.      | `"Empowering Businesses with a Customizable, Data-Driven CRM Solution."`                                                             |
| **image**        | `ImageCommonProps`                                                | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **imageBorder**  | `boolean` (Optiona)                                               | Optional prop to apply a border around the image.        | Default it will not show border, If you want it then pass `true` in this prop.                                                       |
| **bgImage**      | `BgImageProps`                                                    | Background image properties for the benefit data card.   | `{ light: '/assets/images/bg-light.svg', dark: '/assets/images/bg-dark.svg' }`                                                       |
| **benefitData**  | `{ counter: string; caption: string; defaultUnit?: string; }`     | Data for the benefit statistics card.                    | `{ counter: '50+', caption: 'Projects Completed', defaultUnit: '+' }`                                                                |
| **primaryBtn**   | `ButtonProps`                                                     | Properties for the primary button.                       | `{ variant: 'contained', color: 'primary', children: 'Get Started' }`                                                                |
| **secondaryBtn** | `ButtonProps`                                                     | Properties for the secondary button.                     | `{ variant: 'outlined', color: 'primary', children: 'Learn More' }`                                                                  |

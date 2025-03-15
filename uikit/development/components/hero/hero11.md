# Hero11

The `Hero11` component renders a hero section with a review profile, call-to-action email input, benefit counters, an image block, and a slider of icons and titles, using MUI and a responsive layout styled based on the theme.

{% hint style="info" %}
All available props for the Hero11 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero11.tsx`

**Component usage path:**  `src/app/blocks/hero/hero11/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero11**](https://www.saasable.io/blocks/hero/hero11)

## Props Details

| Prop            | Type                                                             | Description                                                                             | Displayed as                                                                                                                               |
| --------------- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **headLine**    | `string`                                                         | Main headline text or element.                                                          | `"Effortless CRM Management, Seamless BusinessGrowth"`                                                                                     |
| **captionLine** | `string`                                                         | Supporting text or description below the headline.                                      | `"Discover innovative solutions tailored to your needs."`                                                                                  |
| **reviewData**  | `{ avatarList: string[], rating: number, totalReviews: string }` | Data for displaying user reviews and ratings, including avatars and total review count. | `{ avatarList: ["/avatars/user1.jpg", "/avatars/user2.jpg"], rating: 4.5, totalReviews: "150 reviews" }`                                   |
| **primaryBtn**  | `ButtonProps`                                                    | Properties for the primary action button.                                               | `{ variant: "contained", color: "primary", children: "Subscribe Now" }`                                                                    |
| **helperText**  | `string`                                                         | Text displayed below the email input field.                                             | `"Stay updated with our latest news."`                                                                                                     |
| **image**       | `ImageCommonProps`                                               | Image path or object with `light` and `dark` image path.                                | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p>       |
| **benefitData** | `{ data1: BenefitDataProps, data2: BenefitDataProps }`           | Data for displaying two different benefits, each with a counter and caption.            | `{ data1: { counter: "50+", caption: "Projects Completed", defaultUnit: "+" }, data2: { counter: "20", caption: "Years of Experience" } }` |
| **sliderTitle** | `string`                                                         | Title for the slider section.                                                           | `"Our Key Features"`                                                                                                                       |
| **listData**    | `ListDataProps[]`                                                | List of items to be displayed in the slider, each with an icon and title.               | `[ { icon: "tabler-star", title: "High Quality" }, { icon: "tabler-thumbs-up", title: "Customer Satisfaction" } ]`                         |

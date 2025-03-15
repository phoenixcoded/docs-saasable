---
description: >-
  The Hero16 is a hero section featuring a responsive video player that
  auto-plays when scrolled into view, combined with review data, a headline with
  optional caption, and a secondary button.
---

# Hero16

{% hint style="info" %}
All available props for the Hero16 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero16.tsx`

**Component usage path:**  `src/app/blocks/hero/hero16/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero16**](https://www.saasable.io/blocks/hero/hero16)

## Props Details

| Prop             | Type                                                              | Description                                                                                                                  | Displayed as                                                                                                                         |
| ---------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **reviewData**   | `{ avatarList: string[]; rating: number; totalReviews: string; }` | User reviews information.                                                                                                    | `{ avatarList: ['/images/avatar1.jpg'], rating: 4.7, totalReviews: '150 Reviews' }`                                                  |
| **heading**      | `string`                                                          | Main heading text for the hero section.                                                                                      | `"Discover Our Latest Innovations"`                                                                                                  |
| **caption**      | `string` (Optional)                                               | Optional subheading or additional descriptive text.                                                                          | `"Our SaaS platform delivers a flawless user experience and unmatched results."`                                                     |
| **secondaryBtn** | `ButtonProps`                                                     | Properties for the secondary button.                                                                                         | `{ variant: 'outlined', color: 'primary', children: 'Watch Now' }`                                                                   |
| **poster**       | `ImageComponentProps`                                             | <p>Poster image for the video element.<br>Image path or object with <code>light</code> and <code>dark</code> image path.</p> | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **videoSrc**     | `string`                                                          | Source URL of the video to be played.                                                                                        | `'/videos/hero-video.mp4'`                                                                                                           |

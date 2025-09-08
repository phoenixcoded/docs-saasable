# Hero17

The Hero17 is a visually engaging hero section that includes animated scroll effects, a headline, a caption, interactive chips with images, and a prominent button, all styled with responsive design and motion animations.

{% hint style="info" %}
All available props for the Hero17 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the hero section.
{% endhint %}

**Component path**: `src/blocks/hero/Hero17.tsx`

**Component usage path:**  `src/app/blocks/hero/hero17/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/hero/hero17**](https://www.saasable.io/blocks/hero/hero17)

## Props Details

| Prop            | Type                            | Description                                                        | Displayed as                                                                                                                 |
| --------------- | ------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- |
| **chip**        | `{ label: ChipProps['label'] }` | Data for the Chip component.                                       | `{ label: 'Featured' }`                                                                                                      |
| **headLine**    | `string`                        | Main headline text.                                                | `"Welcome to Our Next Big Thing"`                                                                                            |
| **captionLine** | `string`                        | Supporting caption text.                                           | `"Discover how we're leading the charge in innovation and design."`                                                          |
| **primaryBtn**  | `ButtonProps`                   | Properties for the primary button.                                 | `{ variant: 'contained', color: 'primary', children: 'Explore Now' }`                                                        |
| **videoSrc**    | `string`                        | Source URL of the video to be played.                              | `'/videos/hero-video.mp4'`                                                                                                   |
| **listData**    | `ListDataProps[]`               | Array of data for each Chip.                                       | `[ { image: { src: '/images/icon1.png' }, title: 'Innovation' }, { image: { src: '/images/icon2.png' }, title: 'Design' } ]` |
| videoThumbnail  | `string`                        | Thumbnail image shown before the video plays or if autoplay fails. | Passed as `poster` in the `<Video>`element to provide a fallback image.                                                      |

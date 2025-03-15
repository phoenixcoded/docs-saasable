# Testimonial2

The `Testimonial2` component features a carousel of testimonial videos with associated reviews, using a slider for navigation and a modal for video playback. It handles video modal state and slider control, with responsive adjustments for arrow visibility and playback behavior.

{% hint style="info" %}
All available props for the Testimonial2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial2.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial2**](https://www.saasable.io/blocks/testimonial/testimonial2)

## Props Details

| Prop             | Type                     | Description                                                | Displayed as                                                                                                                                                                                                                    |
| ---------------- | ------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title for the testimonial section                     | `"What Our Clients Are Saying"`                                                                                                                                                                                                 |
| **caption**      | `string` (Optional)      | Subtitle or additional context                             | `"Read about the experiences of our satisfied clients"`                                                                                                                                                                         |
| **testimonials** | `TestimonialDataProps[]` | List of testimonial objects with video and profile details | `[ { bgImage: "/images/bg1.jpg", videoSrc: "/videos/testimonial1.mp4", review: "This service exceeded my expectations!", ratings: 5, profile: { name: "Alice Johnson", title: "Founder", image: "/images/alice.jpg" } }, ... ]` |

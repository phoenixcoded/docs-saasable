---
description: >-
  The Testimonial1 component displays a section with a video testimonial and
  several review cards, using animations for entrance effects and managing video
  playback based on viewport visibility.
---

# Testimonial1

{% hint style="info" %}
All available props for the Testimonial1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial1.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial1**](https://www.saasable.io/blocks/testimonial/testimonial1)

## Props Details

| Prop             | Type                     | Description                                                 | Displayed as                                                                                                                                                                   |
| ---------------- | ------------------------ | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                 | Main title for the testimonial section                      | `"What Our Clients Say"`                                                                                                                                                       |
| **caption**      | `string` (Optional)      | Subtitle or additional context                              | `"Hear from our satisfied clients about their experiences"`                                                                                                                    |
| **testimonials** | `TestimonialDataProps[]` | List of testimonial objects with optional video and profile | `[ { videoSrc: "/videos/testimonial1.mp4", review: "This service was fantastic!", ratings: 5, profile: { name: "John Doe", title: "CEO", image: "/images/john.jpg" } }, ... ]` |
| **link**         | `LinkProps` (Optional)   | Details for a link to related content                       | `{ href: "/more-testimonials", children: "See More Testimonials" }`                                                                                                            |

---
description: >-
  The  Testimonial9 that displays a grid layout of testimonials using two
  horizontally scrolling marquees, with styling and gradient effects determined
  by the theme direction.
---

# Testimonial9

{% hint style="info" %}
All available props for the Testimonial9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial9.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial9**](https://www.saasable.io/blocks/testimonial/testimonial9)

## Props Details

| Prop             | Type                     | Description                                                        | Displayed as                                                                                                 |
| ---------------- | ------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                 | Main title for the testimonial section.                            | `"What Our Clients Say"`                                                                                     |
| **caption**      | `string` (Optional)      | Subtitle or additional text beneath the heading.                   | `"Hear from our satisfied clients about their experience with us."`                                          |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects with profile details and review text. | `[{ review: "Great service!", profile: { name: "John Doe", title: "CEO", avatar: "path_to_avatar" } }, ...]` |

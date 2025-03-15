---
description: >-
  The Testimonial8 component features a slider that showcases testimonials with
  titles, reviews, profile information, and images, using MUI components and
  react-slick for the carousel functionality.
---

# Testimonial8

{% hint style="info" %}
All available props for the Testimonial8  component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial8.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial8**](https://www.saasable.io/blocks/testimonial/testimonial8)

## Props Details

| Prop             | Type                     | Description                                                                         | Displayed as                                                                                                                                                                                                 |
| ---------------- | ------------------------ | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                 | Main title for the testimonial section.                                             | `"Customer Feedback"`                                                                                                                                                                                        |
| **caption**      | `string` (Optional)      | Additional subtitle or description beneath the heading.                             | `` `"See what our customers have to say about our services." ``                                                                                                                                              |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects, each with title, review, profile, and optional image. | `[{ title: "Amazing Experience!", review: "The service was fantastic...", profile: { name: "Alice Johnson", title: "Marketing Specialist", avatar: "path_to_avatar_image" }, image: "path_to_image" }, ...]` |

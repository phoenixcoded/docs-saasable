---
description: >-
  This testimonial11 renders a testimonial section with a centered heading and a
  grid of testimonial cards, each displaying a review, an avatar, and the
  reviewer's name and role.
---

# Testimonial11

{% hint style="info" %}
All available props for the Testimonial11 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial11.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial11/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial11**](https://www.saasable.io/blocks/testimonial/testimonial11)

## Props Details

| Prop             | Type                     | Description                                                                  | Displayed as                                                                                                                      |
| ---------------- | ------------------------ | ---------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title for the testimonial section.                                      | `"What Our Clients Are Saying"`                                                                                                   |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects, including review text and profile information. | `[{ review: "The team was exceptional...", profile: { name: "John Doe", role: "CEO, Company X", avatar: "john_doe.jpg" } }, ...]` |

---
description: >-
  Testimonial12 is a testimonial slider component that showcases user feedback
  in a clean, responsive layout. It displays an avatar, a quote, the user's
  name, and their role.
---

# Testimonial12

{% hint style="info" %}
All available props for the Testimonial12 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial12.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial12/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial12**](https://www.saasable.io/blocks/testimonial/testimonial12)

## Props Details

| Prop             | Type                     | Description                                                                  | Displayed as                                                                                                                      |
| ---------------- | ------------------------ | ---------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects, including review text and profile information. | `[{ review: "The team was exceptional...", profile: { name: "John Doe", role: "CEO, Company X", avatar: "john_doe.jpg" } }, ...]` |

---
description: >-
  The Testimonial7 component presents a vertically scrolling testimonial slider
  alongside a heading and optional primary button, using MUI components and
  react-slick for the carousel functionality.
---

# Testimonial7

{% hint style="info" %}
All available props for the Testimonial7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial7.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial7**](https://www.saasable.io/blocks/testimonial/testimonial7)

## Props Details

| Prop             | Type                     | Description                                                                       | Displayed as                                                                                                             |
| ---------------- | ------------------------ | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                 | Main title or heading for the testimonial section.                                | `"What Our Clients Say"`                                                                                                 |
| **primaryBtn**   | `ButtonProps` (Optional) | Button properties including text and actions.                                     | `{ text: "Learn More", onClick: () => alert('Button clicked!') }`                                                        |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects, each with review text, rating, and profile details. | `[{ review: "Great service!", ratings: 5, profile: { name: "John Doe", title: "CEO", avatar: "path_to_avatar" } }, ...]` |

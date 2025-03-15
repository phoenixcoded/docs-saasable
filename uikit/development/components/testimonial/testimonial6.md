---
description: >-
  The Testimonial6 component is designed to display a carousel of testimonials
  with a focus on integrating avatars and optional images. Here’s a breakdown of
  its features.
---

# Testimonial6

{% hint style="info" %}
All available props for the Testimonial6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial6.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial6**](https://www.saasable.io/blocks/testimonial/testimonial6)

## Props Details

| Prop             | Type                     | Description                                      | Displayed as                                                                                                                                                                                                                                                                                                                                                           |
| ---------------- | ------------------------ | ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title or heading of the testimonial section | `"What Our Clients Say"`                                                                                                                                                                                                                                                                                                                                               |
| **caption**      | `string` (Optional)      | Additional description or subtitle               | `"Here are some comments from our valued clients"`                                                                                                                                                                                                                                                                                                                     |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects                     | `[ { title: 'Exceptional performance', image: { component: 'testimonial/Twitch', type: DynamicComponentType.IMAGE }, review: As a tech enthusiast, I'm blown away by this AI platform. It's not just a tool; it's a game-changer. Exceptional performance and ease of use, profile: { avatar: '/path-to/avatar2.png', name: 'John Carter', role: 'Designer' } }, ...]` |


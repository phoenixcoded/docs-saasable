---
description: >-
  The Login5 component renders a login page featuring a carousel of
  testimonials, a main heading and caption, and authentication forms, with
  responsive design elements and styling.
---

# Login5

{% hint style="info" %}
All available props for the Login5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Login  section.
{% endhint %}

**Component path**: `src/blocks/auth/Login/5.tsx`

**Component usage path:**  `src/app/blocks/auth/login/5/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/auth/login/5](https://www.saasable.io/blocks/auth/login/5)

## Props Details

| Prop Name        | Type                     | Description                                | Displayed as                                                                                             |
| ---------------- | ------------------------ | ------------------------------------------ | -------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title or heading for the page.        | `"What Our Clients Say"`                                                                                 |
| **caption**      | `string` (optional)      | Optional subtitle or additional text.      | `"Real feedback from real customers"`                                                                    |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects with reviews. | `[{ ratings: 5, review: "Excellent!", profile: { avatar: 'url', name: 'John Doe', role: 'Customer' } }]` |


# Testimonial3

The `Testimonial3` component creates a responsive testimonial carousel with two slides visible at a time on larger screens and one on smaller screens, incorporating user reviews, ratings, and profile information in a styled layout.

{% hint style="info" %}
All available props for the Testimonial3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial3.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial3**](https://www.saasable.io/blocks/testimonial/testimonial3)

## Props Details



| Prop             | Type                     | Description                                      | Displayed as                                                                                                                                                                                                                           |
| ---------------- | ------------------------ | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title or heading of the testimonial section | `"What Our Clients Say"`                                                                                                                                                                                                               |
| **caption**      | `string` (Optional)      | Additional description or subtitle               | `"Here’s how our customers feel about our service"`                                                                                                                                                                                    |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects                     | `[ { review: 'The user interface is intuitive, making it easy for our team to adapt and maximize productivity.', ratings: 4, profile: { avatar: '/path-to/avatar2.png', name: 'Sydnie', role: 'Direct Optimization Executive' }, ...]` |

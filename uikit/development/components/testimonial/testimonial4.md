# Testimonial4

The `Testimonial4` component displays a carousel of testimonial reviews, using a `react-slick` slider with autoplay and custom dot styles. The testimonials are centered with styled quotes and profile cards, and the component is designed to be responsive with adjustable padding and alignment.

{% hint style="info" %}
All available props for the Testimonial4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial4.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial4**](https://www.saasable.io/blocks/testimonial/testimonial4)

## Props Details

| Prop             | Type                     | Description                                      | Displayed as                                                                                                                                                                                                                           |
| ---------------- | ------------------------ | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title or heading of the testimonial section | `"Customer Feedback"`                                                                                                                                                                                                                  |
| **caption**      | `string` (Optional)      | Additional description or subtitle               | `"Here’s what our users have to say about us"`                                                                                                                                                                                         |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects                     | `[ { review: 'The user interface is intuitive, making it easy for our team to adapt and maximize productivity.', ratings: 4, profile: { avatar: '/path-to/avatar2.png', name: 'Sydnie', role: 'Direct Optimization Executive' }, ...]` |

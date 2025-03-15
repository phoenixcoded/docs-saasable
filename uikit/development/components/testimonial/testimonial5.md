# Testimonial5

The `Testimonial5` component is a carousel of testimonials that features centered slides with varying opacity for active slides, displays profile cards and optional images, and includes animation effects for smooth transitions.

{% hint style="info" %}
All available props for the Testimonial5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial5.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial5**](https://www.saasable.io/blocks/testimonial/testimonial5)

## Props Details

| Prop             | Type                     | Description                                      | Displayed as                                                                                                                                                                                                                                                                                         |
| ---------------- | ------------------------ | ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title or heading of the testimonial section | `"What Our Clients Are Saying"`                                                                                                                                                                                                                                                                      |
| **caption**      | `string` (Optional)      | Additional description or subtitle               | `"Read the experiences of our satisfied clients"`                                                                                                                                                                                                                                                    |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects                     | `[ { review: 'This AI platform has revolutionized my workflow. Fast, accurate, and indispensable!', profile: { avatar: '/path-to/avatar2.png', name: 'Anne Thompson', role: 'Direct Optimization Executive' }, image: { component: 'clientele/Techlify', type: DynamicComponentType.IMAGE } }, ...]` |

# Testimonial10

The `Testimonial10` component displays testimonials in a Masonry grid layout, with ratings, titles, reviews, and profile information, utilizing MUI components and a radial gradient background for visual emphasis.

{% hint style="info" %}
All available props for the Testimonial10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial10.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial10**](https://www.saasable.io/blocks/testimonial/testimonial10)

## Props Details

| Prop             | Type                     | Description                                                                 | Displayed as                                                                                                                                                    |
| ---------------- | ------------------------ | --------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title for the testimonial section.                                     | `"What Our Clients Say"`                                                                                                                                        |
| **caption**      | `string` (Optional)      | Subtitle or additional context below the heading.                           | `"Read the experiences shared by our satisfied clients."`                                                                                                       |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects including title, review, profile, and ratings. | `[{ title: "Excellent Service", review: "The service was outstanding...", ratings: 5, profile: { name: "Alice Johnson", role: "Marketing Specialist" } }, ...]` |

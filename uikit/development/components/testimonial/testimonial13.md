---
description: >-
  The Testimonial13 component is a responsive testimonial carousel built using
  Material-UI (MUI), react-slick (for the slider), and Framer Motion (for
  animations).
---

# Testimonial13

{% hint style="info" %}
All available props for the Testimonial13 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Testimonial section.
{% endhint %}

**Component path**: `src/blocks/testimonial/Testimonial13.tsx`

**Component usage path:**  `src/app/blocks/testimonial/testimonial13/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/testimonial/testimonial13**](https://www.saasable.io/blocks/testimonial/testimonial13)

## Props Details

| Prop             | Type                     | Description                                                                                                                           | Displayed as                                                                                                                      |
| ---------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| heading          | `string`                 | The heading or title for the section. Displays as the main title above the testimonials.                                              | `"Customer Testimonials"`                                                                                                         |
| **testimonials** | `TestimonialDataProps[]` | Array of testimonial objects, including review text and profile information.                                                          | `[{ review: "The team was exceptional...", profile: { name: "John Doe", role: "CEO, Company X", avatar: "john_doe.jpg" } }, ...]` |
| primaryBtn       | `object`                 | A button to be displayed next to the heading. The children is the text on the button, and onClick is the function triggered on click. | `[ { profile: { name: "John Doe", role: "Product Manager", avatar: "/images/john.png" }, review: "Great platform!" }, ... ]`      |

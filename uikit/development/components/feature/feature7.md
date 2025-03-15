---
description: >-
  The Feature7 component presents a testimonial slider with animated progress
  bars, breadcrumb navigation, and images, using React Slick for carousel
  functionality and styled components.
---

# Feature7

{% hint style="info" %}
All available props for the Feature7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature7.tsx`

**Component usage path:**  `src/app/blocks/feature/feature7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature7**](https://www.saasable.io/blocks/feature/feature7)

## Props Details

| Prop             | Type                     | Description                                                             | Displayed as                                                                                                                                                      |
| ---------------- | ------------------------ | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**      | `string`                 | Main title of the feature section.                                      | `"Our Clients Speak"`                                                                                                                                             |
| **caption**      | `string` (Optional)      | Additional description or subtitle.                                     | `"Hear from those who have used our service"`                                                                                                                     |
| **breadcrumbs**  | `BreadcrumbProps[]`      | List of breadcrumb items for navigation.                                | `[ { title: "Home" }, { title: "Testimonials" }, { title: "Client Feedback" } ]`                                                                                  |
| **testimonials** | `TestimonialDataProps[]` | List of testimonials with details like icon, title, content, and image. | `[ { features: [ { icon: "icon-name", title: "Excellent Service", content: "The service was top-notch..." } ], progress: 75, image: "path-to-image.jpg" }, ... ]` |

---
description: >-
  Cta14 is a responsive MUI component that showcases a product or service. It
  includes an image, avatar, rating, heading, caption, price, and an optional
  action button.
---

# Cta14

{% hint style="info" %}
All available props for the Cta14 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta14.tsx`

**Component usage path:**  `src/app/blocks/cta/cta14/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta14**](https://www.saasable.io/blocks/cta/cta14)

## Props Details

| Prop        | Type                  | Description                                                             | Displayed as                                                    |
| ----------- | --------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------- |
| **heading** | `string`              | Main heading text displayed prominently.                                | Positioned at the top of the section.                           |
| **caption** | `string` (Optional)   | Additional text providing context or details related to the heading.    | Positioned below the heading                                    |
| image       | `string` (image path) | Image URL/path for a person/avatar                                      | Rendered as an avatar using  `<Avatar />`                       |
| name        | `string`              | Name of the person (e.g., testimonial author)                           | Rendered next to avatar as a subtitle                           |
| ratings     | `number`              | A numerical rating score (e.g., 4.5)                                    | Rendered via the custom `<Rating / >`component                  |
| price       | `number`              | The price of the product or service                                     | Rendered as large bold text using `<Typography variant="h3" />` |
| primaryBtn  | `ButtonProps`         | Configuration for the call-to-action button (text, click handler, etc.) | Rendered as a Button inside `<ButtonAnimationWrapper />`        |


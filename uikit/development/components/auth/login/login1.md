---
description: >-
  The Login1 component renders a two-column layout for a login page, featuring a
  login form with social and email options on the left, and a testimonial slider
  with an image on the right.
---

# Login1

{% hint style="info" %}
All available props for the Login1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Login  section.
{% endhint %}

**Component path**: `src/blocks/auth/Login/1.tsx`

**Component usage path:**  `src/app/blocks/auth/login/1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/auth/login/1](https://www.saasable.io/blocks/auth/login/1)

## Props Details

| Prop             | Type                     | Description                                                                                                                                                                     | Displayed as                                                                                                                                                                   |
| ---------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**      | `string`                 | This is the main title or heading for the login section of the component. It typically conveys the primary message or purpose of the page, such as "Login" or "Welcome Back".   | The `heading` is displayed prominently at the top of the left column, inside the `Typeset` component, providing context for the page or section.                               |
| **caption**      | `string` (optional)      | This is an optional subheading or additional text that supports the `heading`. It might provide a brief explanation or welcoming message.                                       | The `caption` appears below the `heading`, also inside the `Typeset` component, offering additional context or guidance to the user.                                           |
| **testimonials** | `TestimonialDataProps[]` | An array of testimonial data objects, where each object contains information like user ratings, reviews, and profile details. This data is shown in a slider on the right side. | Each testimonial is rendered in a `Slider` component, displaying the review, rating (with stars), and user profile details through the `Rating` and `ProfileCard2` components. |
| **image**        | `ImageCommonProps`       | This is an image object representing a graphic element or illustration associated with the login page. It includes properties like the image URL and alt text.                  | The `image` is displayed at the bottom of the right column using the `GraphicsImage` component, enhancing the visual appeal of the page.                                       |

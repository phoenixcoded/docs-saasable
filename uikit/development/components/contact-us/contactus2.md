---
description: >-
  The ContactUs2 component that displays contact information in a responsive
  grid layout with background image and animations, including a form and contact
  details using themed cards and icons.
---

# ContactUs2

{% hint style="info" %}
All available props for the ContactUs2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the contactus section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs2.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us2](https://www.saasable.io/blocks/contact-us/contact-us2)

## Props Details

| Prop               | Type                      | Description                                                                          | Displayed as                                                                       |
| ------------------ | ------------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------- |
| **heading**        | `string`                  | Main title of the contact section.                                                   | `"Get in Touch"`                                                                   |
| **caption**        | `string`                  | Additional description or context for the contact section.                           | `"We'd love to hear from you. Reach out through any of the following methods:"`    |
| **contactDetails** | `ContactProps`            | Contains `address`, `email`, and `phone` for displaying contact information.         | `{ address: "123 Main Street", email: "sales@example.com", phone: "+1234567890" }` |
| **bgImage**        | `BgImageProps` (Optional) | URL for the background image of the `GraphicsCard` component in the contact section. | `"url('/path/to/image.jpg')"`                                                      |

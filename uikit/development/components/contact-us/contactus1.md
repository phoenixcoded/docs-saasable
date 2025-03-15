---
description: >-
  The ContactUs1 defines a "Contact Us" section with a card layout using
  Material UI components, displaying contact information alongside a contact
  form, all wrapped within a responsive grid.
---

# ContactUs1

{% hint style="info" %}
All available props for the ContactUs1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the ContactUs section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs1.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us1/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us1](https://www.saasable.io/blocks/contact-us/contact-us1)

## Props Details

| Prop               | Type           | Description                                                       | Displayed as                                                                        |
| ------------------ | -------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| **heading**        | `string`       | Main title of the contact section.                                | `"Get in Touch"`                                                                    |
| **caption**        | `string`       | Secondary description or context for the contact section.         | `"We're here to assist you. Reach out to us through any of the following methods:"` |
| **contactDetails** | `ContactProps` | Contains `address`, `email`, and `phone` for contact information. | `{ address: "123 Main Street", email: "sales@example.com", phone: "+1234567890" }`  |

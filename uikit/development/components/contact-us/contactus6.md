---
description: >-
  The ContactUs6 component displays a contact section with a map, contact
  details, and a form, using a responsive layout with Material UI and Next.js.
---

# ContactUs6

{% hint style="info" %}
All available props for the ContactUs6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the contactus section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs6.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us6/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us6](https://www.saasable.io/blocks/contact-us/contact-us6)

## Props Details

| Prop               | Type                | Description                                                         | Displayed as                                                                                                               |
| ------------------ | ------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **heading**        | `string`            | Main title of the contact section.                                  | `"Get in Touch"`                                                                                                           |
| **caption**        | `string` (optional) | Additional information or context under the heading.                | `"We are here to assist you. Reach out through any of the following methods:"`                                             |
| **contactDetails** | `ContactProps`      | Contains contact information displayed in `ContactCard` components. | `{ address: "123 Main Street, Hometown", phone: "+1234567890", email: "support@example.com", time: "Mon-Fri: 9am - 6pm" }` |

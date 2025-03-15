# ContactUs3

The`ContactUs3` component that displays heading caption and  a list of contact cards in a responsive grid layout, with dynamic grid sizes based on the number of cards. Each card features an icon, title, content, and an optional link button, using the `ContactCard` and `GraphicsCard` components.

{% hint style="info" %}
All available props for the ContactUs3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the contactus section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs3.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us3/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us3](https://www.saasable.io/blocks/contact-us/contact-us3)

## Props Details

| Prop        | Type                        | Description                                                           | Displayed as                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----------- | --------------------------- | --------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading** | `string`                    | Main title for the contact section.                                   | `"Get in Touch"`                                                                                                                                                                                                                                                                                                                                                                                                  |
| **caption** | `string` (optional)         | Additional description or context under the heading.                  | `"We are here to assist you. Feel free to contact us through the following methods:"`                                                                                                                                                                                                                                                                                                                             |
| **list**    | array of `ContactCardProps` | Array of contact details to be displayed as `ContactCard` components. | `[ { icon: "tabler-map-pin", title: "Visit us", content: "123 Main Street, Hometown", link: { href: "/location", text: "See on map" } }, { icon: "tabler-mail", title: "Email us", content: "support@example.com", link: { href: "mailto:support@example.com", text: "Send Email" } }, { icon: "tabler-phone", title: "Call us", content: "+1234567890", link: { href: "tel:+1234567890", text: "Call Now" } } ]` |

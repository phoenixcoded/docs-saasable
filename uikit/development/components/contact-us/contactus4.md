# ContactUs4

&#x20;The`ContactUs4` component that conditionally renders a contact form (`ContactUsForm2`) and displays a list of contact cards. The form and cards are laid out in a responsive grid, with each card showing an icon, title, content, and an optional link. The form can be toggled on or off using the `showForm` prop.

{% hint style="info" %}
All available props for the ContactUs4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the contactus section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs4.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us4/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us4](https://www.saasable.io/blocks/contact-us/contact-us4)

## Props Details

| Prop         | Type                        | Description                                                           | Displayed as                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------ | --------------------------- | --------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**  | `string` (optional)         | Main title for the contact section.                                   | `"Get in Touch"`                                                                                                                                                                                                                                                                                                                                                                                                  |
| **caption**  | `string` (optional)         | Additional description or context under the heading.                  | `"We're here to help. Reach out to us through any of the following methods:"`                                                                                                                                                                                                                                                                                                                                     |
| **list**     | array of `ContactCardProps` | Array of contact details to be displayed as `ContactCard` components. | `[ { icon: "tabler-map-pin", title: "Visit us", content: "123 Main Street, Hometown", link: { href: "/location", text: "See on map" } }, { icon: "tabler-mail", title: "Email us", content: "support@example.com", link: { href: "mailto:support@example.com", text: "Send Email" } }, { icon: "tabler-phone", title: "Call us", content: "+1234567890", link: { href: "tel:+1234567890", text: "Call Now" } } ]` |
| **showForm** | `boolean` (optional)        | The form can be toggled on or off using this prop.                    | Default it will show form. If you not want it then set `showForm` false.                                                                                                                                                                                                                                                                                                                                          |

# ContactUs5

The  `ContactUs5` component that displays contact information, a contact form (`ContactUsForm1`), and an interactive map (using `react-leaflet`). The layout is structured using a responsive grid, with contact details displayed as cards featuring icons, titles, and links. The map shows a location centered at specific coordinates, and the contact cards allow users to visit, call, or email.

{% hint style="info" %}
All available props for the ContactUs5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the contactus section.
{% endhint %}

**Component path**: `src/blocks/contact-us/ContactUs5.tsx`

**Component usage path:**  `src/app/blocks/contact-us/contact-us5/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/contact-us/contact-us5](https://www.saasable.io/blocks/contact-us/contact-us5)

## Props Details

| Prop               | Type                | Description                                                         | Displayed as                                                                                   |
| ------------------ | ------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **heading**        | `string`            | Main title of the contact section.                                  | `"Contact Us"`                                                                                 |
| **caption**        | `string` (optional) | Additional information or context under the heading.                | `"Get in touch with us through any of the following methods. We are here to assist you!"`      |
| **contactDetails** | `ContactProps`      | Contains contact information displayed in `ContactCard` components. | `{ address: "123 Main Street, Hometown", phone: "+1234567890", email: "support@example.com" }` |

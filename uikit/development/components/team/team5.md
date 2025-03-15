# Team5

The `Team5` component creates a team section with a responsive layout that includes a heading, caption, optional action button, description, image, and a slider showcasing team members in chunks based on screen size.

{% hint style="info" %}
All available props for the Team5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team5.tsx`

**Component usage path:**  `src/app/blocks/team/team5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team5**](https://www.saasable.io/blocks/team/team5)

## Props Details

| Prop            | Type                          | Description                                                          | Displayed as                                                                                                                         |
| --------------- | ----------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**     | `string`                      | Main title of the section.                                           | `"Meet Our Team"`                                                                                                                    |
| **caption**     | `string` (Optional)           | Additional context or subtitle.                                      | `"Dedicated professionals driving our success."`                                                                                     |
| **members**     | `ProfileProps[]`              | Contains data for each team member to be displayed in profile cards. | `[{ name: "John Doe", role: "CEO", avatar: "path/to/avatar.jpg" }, ...]`                                                             |
| **image**       | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path.             | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **actionBtn**   | `ButtonProps` (Optional)      | Optional button for additional actions.                              | `{ href: "/contact", children: "Contact Us" }`                                                                                       |
| **description** | `string` (Optional)           | Description or additional text for the image section.                | `"Our team is composed of highly skilled individuals who are passionate about delivering excellence."`                               |

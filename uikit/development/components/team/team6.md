# Team6

The `Team6` component showcases a team section with a centered heading, optional action button, and a description image. Below the image and description, it displays team members in a responsive grid using `ProfileCard3`. The layout adapts for different screen sizes, and the avatar sizes adjust accordingly.

{% hint style="info" %}
All available props for the Team6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Team section.
{% endhint %}

**Component path**: `src/blocks/team/Team6.tsx`

**Component usage path:**  `src/app/blocks/team/team6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/team/team6**](https://www.saasable.io/blocks/team/team6)

## Props Details

| Prop            | Type                          | Description                                                    | Displayed as                                                                                                                         |
| --------------- | ----------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**     | `string`                      | Main title of the section                                      | `"Meet Our Team"`                                                                                                                    |
| **caption**     | `string` (Optional)           | Subtitle or additional text below the heading                  | `"Our team consists of dedicated professionals..."`                                                                                  |
| **members**     | `ProfileProps[]`              | List of team members with their details                        | `[ { "name": "John Doe", "role": "CEO", "avatar": "/path/to/john-avatar.jpg" } ]`                                                    |
| **image**       | `ImageCommonProps` (Optional) | Image path or object with `light` and `dark` image path.       | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **actionBtn**   | `ButtonProps` (Optional)      | Configuration for an action button, including text and handler | `{ "text": "Contact Us", "onClick": () => alert('Button clicked!') }`                                                                |
| **description** | `string`                      | Brief description or additional information about the team     | `"Our team is passionate about delivering top-notch solutions..."`                                                                   |

# Process3

The `Process3` component renders a section with an accordion-style list of cards and an optional image, allowing users to expand and view details for each card while presenting an image alongside the content.

{% hint style="info" %}
All available props for the Process3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process3.tsx`

**Component usage path:**  `src/app/blocks/process/process3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process3**](https://www.saasable.io/blocks/process/process3)

## Props Details

| Prop                | Type                 | Description                                                                                                                                           | Displayed as                                                                                                                         |
| ------------------- | -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **heading**         | `string`             | Main title of the section.                                                                                                                            | `"Our Workflow"`                                                                                                                     |
| **caption**         | `string`             | Subheading or additional description related to the heading.                                                                                          | `"Discover the step-by-step process that we follow to deliver successful projects."`                                                 |
| **image**           | `ImageCommonProps`   | <p>Properties for the image displayed alongside the cards.<br>pass Image path or object with <code>light</code> and <code>dark</code> image path.</p> | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **cards**           | `ProcessCardProps[]` | Array of card objects for rendering accordion panels.                                                                                                 | `[ { title: 'Initial Consultation', description: 'We discuss...', ... }, { title: 'Design Phase', ... } ]`                           |
| **defaultExpanded** | `string` (Optional)  | The panel to expand by default when the component first loads.                                                                                        | `"panel0"`                                                                                                                           |

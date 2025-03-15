# Process5

The `Process5` component displays a series of styled cards with alternating image and text layouts, each featuring a rounded avatar, title, description, and a list of items, all within a responsive grid layout.

{% hint style="info" %}
All available props for the Process5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process5.tsx`

**Component usage path:**  `src/app/blocks/process/process5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process5**](https://www.saasable.io/blocks/process/process5)

## Props Details



| Prop        | Type                  | Description                                                                      | Displayed as                                                                                              |
| ----------- | --------------------- | -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **heading** | `string`              | Main title for the section                                                       | `"Our Key Processes"`                                                                                     |
| **caption** | `string`              | Additional description or context                                                | `"Explore the essential stages of our process, each represented with detailed descriptions and visuals."` |
| **cards**   | `ProcessCardProps2[]` | Array of process cards with number, title, description, image, and optional list | See example data above                                                                                    |

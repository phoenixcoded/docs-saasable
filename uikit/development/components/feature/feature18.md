# Feature18

The `Feature18` component provides a tabbed interface where each tab displays a section with an image, title, description, and a list of features. It includes an optional action button for each section and is styled to adjust layout and appearance based on the selected tab and screen size.

{% hint style="info" %}
All available props for the Feature18 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature18.tsx`

**Component usage path:**  `src/app/blocks/feature/feature18/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature18**](https://www.saasable.io/blocks/feature/feature18)

## Props Details

| Prop        | Type                | Description                                   | Displayed as                                       |
| ----------- | ------------------- | --------------------------------------------- | -------------------------------------------------- |
| **heading** | `string`            | Main heading for the section.                 | `"Explore Our Features"`                           |
| **caption** | `string` (Optional) | Additional description or subtitle            | Optional caption or description below the heading. |
| **topics**  | `TopicsProps[]`     | Array of tab topics with content and actions. | See `topics` example above                         |

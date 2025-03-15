---
description: >-
  The Feature1 component renders a section with a heading and caption, displays
  two image blocks side-by-side, and includes a third block with an image,
  title, description, and an optional action button
---

# Feature1

{% hint style="info" %}
All available props for the Feature1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the feature section.
{% endhint %}

**Component path**: `src/blocks/feature/Feature1.tsx`

**Component usage path:**  `src/app/blocks/feature/feature1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/feature/feature1**](https://www.saasable.io/blocks/feature/feature1)

## Props Details

| Prop           | Type                     | Description                                                                                     | Displayed as                                                                                                              |
| -------------- | ------------------------ | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **heading**    | `string`                 | Main title for the feature section.                                                             | Passed to `Typeset` component to display the main heading.                                                                |
| **caption**    | `string` (Optional)      | Secondary text providing additional context.                                                    | Passed to `Typeset` component to display below the main heading.                                                          |
| **blockData1** | `BlockProps`             | Data for the first block, including image, title, and description.                              | Used in `ImageBlock` to render the first image block with associated title and description.                               |
| **blockData2** | `BlockProps`             | Data for the second block, including image, title, and description.                             | Used in `ImageBlock` to render the second image block with associated title and description, aligned differently (right). |
| **blockData3** | `BlockProps`             | Data for the third block, including image, title, and description, plus optional action button. | Used to render a larger block with both image and text content, along with an optional button if `actionBtn` is provided. |
| **actionBtn**  | `ButtonProps` (Optional) | Properties for an optional action button.                                                       | Rendered inside `ButtonAnimationWrapper` in the third block if provided, enabling user interaction.                       |

---
description: >-
  Process8 is a responsive UI component that displays a heading, caption, image,
  and a list of process steps—each with an icon, title, and description—using
  Material-UI layout and styling.
---

# Process8

{% hint style="info" %}
All available props for the Process8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process8.tsx`

**Component usage path:**  `src/app/blocks/process/process8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process8**](https://www.saasable.io/blocks/process/process8)

## Props Details

| Prop        | Type                 | Description                                                                                                 | Displayed as                                                                                                                                                                         |
| ----------- | -------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading** | `string`             | The main title or heading displayed at the top of the section.                                              | `"Our 3-Step Process"`                                                                                                                                                               |
| **caption** | `string`             | A short description or subtitle under the main heading that explains the content or process in more detail. | `"A simple, step-by-step guide to how we work."`                                                                                                                                     |
| image       | `ImageCommonProps`   | Image object containing at least src and alt. Displayed on the left side of the section.                    | `{ src: '/assets/process.png', alt: 'Illustration of the process' }`                                                                                                                 |
| **cards**   | `ProcessCardProps[]` | An array of process cards containing individual steps, each with an icon, title, and description.           | <p><code>[{ title: 'Automated Scaling Process', description: 'Ensures optimal performance without manual intervention.', icon: 'tabler-artboard' },</code><br><code>... ]</code></p> |

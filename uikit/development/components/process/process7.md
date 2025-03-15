---
description: >-
  The Process7 component presents a responsive layout with two images, a title
  and caption, and dynamically rendered process steps in either a timeline or
  stepper format, depending on screen size.
---

# Process7

{% hint style="info" %}
All available props for the Process7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process7.tsx`

**Component usage path:**  `src/app/blocks/process/process7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process7**](https://www.saasable.io/blocks/process/process7)

## Props Details

| Prop        | Type                 | Description                                                                                                                                                                      | Displayed as                                                                                                                                                                         |
| ----------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **heading** | `string`             | The main title or heading displayed at the top of the section.                                                                                                                   | `"Our Process"`                                                                                                                                                                      |
| **caption** | `string`             | A short description or subtitle under the main heading that explains the content or process in more detail.                                                                      | `"A simple, step-by-step guide to how we work."`                                                                                                                                     |
| **image1**  | `ImageCommonProps`   | <p>The first image to be displayed, usually as part of the process visualization.<br><br>Pass image path or object with <code>light</code> and <code>dark</code> image path.</p> | <p><code>"path-to-image1.svg"</code><br> or <br><code>{ light: 'path-to-image-light1.svg', dark: 'path-to-image1-dark.svg' }</code></p>                                              |
| **image2**  | `ImageCommonProps`   | <p>The second image to be displayed, complementing the first in the layout.<br><br>Pass image path or object with <code>light</code> and <code>dark</code> image path.</p>       | <p><code>"path-to-image2.svg"</code><br> or <br><code>{ light: 'path-to-image2-light.svg', dark: 'path-to-image2-dark.svg' }</code></p>                                              |
| **cards**   | `ProcessCardProps[]` | An array of process cards containing individual steps, each with an icon, title, and description.                                                                                | <p><code>[{ title: 'Automated Scaling Process', description: 'Ensures optimal performance without manual intervention.', icon: 'tabler-artboard' },</code><br><code>... ]</code></p> |

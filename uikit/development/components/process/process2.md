---
description: >-
  The Process2 component renders a section with a background image card and a
  list of feature cards, displaying a heading, caption, and each feature card’s
  title, description, and icon.
---

# Process2

{% hint style="info" %}
All available props for the Process2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Process section.
{% endhint %}

**Component path**: `src/blocks/process/Process2.tsx`

**Component usage path:**  `src/app/blocks/process/process2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/process/process2**](https://www.saasable.io/blocks/process/process2)

## Props Details

| Prop        | Type                 | Description                                                  | Displayed as                                                                                      |
| ----------- | -------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| **heading** | `string`             | Main title of the section.                                   | `"Our Process"`                                                                                   |
| **caption** | `string`             | Subheading or additional description related to the heading. | `"Discover how we bring ideas to life with our streamlined process."`                             |
| **bgImage** | `BgImageProps`       | Background image settings for the `GraphicsCard` component.  | `{ src: 'https://example.com/background-image.jpg', alt: 'Background Image' }`                    |
| **cards**   | `ProcessCardProps[]` | Array of objects containing data for each card.              | `[ { title: 'Step 1', description: 'Initial consultation...', icon: 'consultation-icon' }, ... ]` |

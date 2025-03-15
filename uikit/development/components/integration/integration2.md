---
description: >-
  Integration2 that displays a section with a headline, caption, a list of tags
  with optional icons, and a primary button, all styled with Material-UI and
  animated with Framer Motion.
---

# Integration2

{% hint style="info" %}
All available props for the Integration2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration2.tsx`

**Component usage path:**  `src/app/blocks/integration/integration2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration2**](https://www.saasable.io/blocks/integration/integration2)

## Props Details

| Prop            | Type          | Description                                                                                                            | Displayed as                                               |
| --------------- | ------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| **headLine**    | `string`      | A title or main heading text that will be displayed at the top of the component.                                       | `"Explore Our Integrations"`                               |
| **captionLine** | `string`      | A subtitle or descriptive text that will be displayed beneath the headline, usually in a smaller font.                 | `"Seamless connections for your business needs"`           |
| **primaryBtn**  | `ButtonProps` | The configuration for the primary button. Includes button properties like label, onClick action, and style.            | `{ children: "Get Started", onClick: handleStart }`        |
| **tagList**     | `TagProps[]`  | An array of integration tags that will be displayed as chips (or labels). Each tag includes a label and optional icon. | `[{ label: "Slack", icon: "slack" }, { label: "Zapier" }]` |

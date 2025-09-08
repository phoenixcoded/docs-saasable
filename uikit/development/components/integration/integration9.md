---
description: >-
  The Integration9 component displays a two-column layout with a heading,
  caption, and button on the left and a vertically auto-scrolling list of
  integration tags on the right using a React-Slick slider
---

# Integration9



{% hint style="info" %}
All available props for the Integration9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration9.tsx`

**Component usage path:**  `src/app/blocks/integration/integration9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration9**](https://www.saasable.io/blocks/integration/integration8)

## Props Details

| Prop            | Type          | Description                                               | Displayed as                                                                          |
| --------------- | ------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| **headLine**    | `string`      | Main heading or title of the section.                     | `"Seamless Integrations"`                                                             |
| **captionLine** | `string`      | Subheading or caption providing additional context.       | `"Connect with your favorite tools effortlessly"`                                     |
| **primaryBtn**  | `ButtonProps` | Properties for the primary button (e.g., variant, color). | `{ variant: 'contained', color: 'primary', onClick: () => alert('Button clicked!') }` |
| tagList         | `TagProps[]`  | List of integrations (icon + label)                       | Image-like vertical scroll items                                                      |


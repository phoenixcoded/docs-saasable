---
description: >-
  Integration8 that displays a series of integration icons in a responsive
  layout with customizable heading, caption, and primary button, using
  Material-UI components for styling and layout.
---

# Integration8

{% hint style="info" %}
All available props for the Integration8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration8.tsx`

**Component usage path:**  `src/app/blocks/integration/integration8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration8**](https://www.saasable.io/blocks/integration/integration8)

## Props Details

| Prop            | Type          | Description                                               | Displayed as                                                                          |
| --------------- | ------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| **headLine**    | `string`      | Main heading or title of the section.                     | `"Seamless Integrations"`                                                             |
| **captionLine** | `string`      | Subheading or caption providing additional context.       | `"Connect with your favorite tools effortlessly"`                                     |
| **primaryBtn**  | `ButtonProps` | Properties for the primary button (e.g., variant, color). | `{ variant: 'contained', color: 'primary', onClick: () => alert('Button clicked!') }` |

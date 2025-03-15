---
description: >-
  Cta7 component renders a call-to-action section featuring an optional
  headline, a caption, and a primary button, all set against a styled background
  with a radial gradient and dotted pattern
---

# Cta7

{% hint style="info" %}
All available props for the Cta7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta7.tsx`

**Component usage path:**  `src/app/blocks/cta/cta7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta7**](https://www.saasable.io/blocks/cta/cta7)

## Props Details

| Prop           | Type           | Description                                                                              | Displayed as                            |
| -------------- | -------------- | ---------------------------------------------------------------------------------------- | --------------------------------------- |
| **headLine**   | `ReactElement` | A React element representing the main headline or message. Can be a complex JSX element. | Displayed prominently on the left side. |
| **caption**    | `string`       | Additional text providing context or secondary information.                              | Displayed below the headline.           |
| **primaryBtn** | `ButtonProps`  | Properties for the primary button (e.g., text, color, variant).                          | Rendered below the caption as a CTA.    |

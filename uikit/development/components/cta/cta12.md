---
description: >-
  The Cta12 component displays a call-to-action section with a heading, caption,
  and a primary button on one side, and a styled image on the other. It uses
  animations to reveal content on scroll.
---

# Cta12

{% hint style="info" %}
All available props for the Cta12 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the cta section.
{% endhint %}

**Component path**: `src/blocks/cta/Cta12.tsx`

**Component usage path:**  `src/app/blocks/cta/cta12/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/cta/cta12**](https://www.saasable.io/blocks/cta/cta12)

## Props Details

| Prop           | Type                      | Description                                                                           | Displayed as                                     |
| -------------- | ------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------ |
| **heading**    | `string`                  | Main heading text displayed prominently.                                              | Positioned at the top of the section.            |
| **caption**    | `string`                  | Additional text providing context or details related to the heading.                  | Positioned below the heading                     |
| **primaryBtn** | `ButtonProps`  (Optional) | Properties for the primary button, such as text, style, and click handlers. Required. | Renders a button for user interaction or action. |
| **image**      | `ImageCommonProps`        | Properties for the image, including source, alt text, and styling options.            | Displayed as a visual element or background.     |

---
description: >-
  The  Faq5 component that displays a FAQ section with accordion panels, an
  optional image, and a "Get in Touch" call-to-action, using MUI and custom
  components for layout and styling.
---

# Faq5

{% hint style="info" %}
All available props for the Faq5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq5.tsx`

**Component usage path:**  `src/app/blocks/faq/faq5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq5**](https://www.saasable.io/blocks/faq/faq5)

## Props Details

| Prop                | Type                                          | Description                                                            | Displayed as                                                                                                                                                                  |
| ------------------- | --------------------------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | Main title of the FAQ section.                                         | `"Frequently Asked Questions"`                                                                                                                                                |
| **caption**         | `string` (Optional)                           | Subtitle or additional description for the FAQ section.                | `"Here are answers to some of the most common questions we receive."`                                                                                                         |
| **defaultExpanded** | `string` or `false`                           | Which FAQ panels are expanded by default.                              | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                                                               |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "What is your return policy?", answer: "You can return items within 30 days of purchase." }, ...]`                                                              |
| **image**           | `ImageCommonProps`                            | Image related to the FAQ content, displayed in a `GraphicsCard`.       | `"https://via.placeholder.com/400x300.png"` or `<GraphicsImage {...{ image }} />`                                                                                             |
| **getInTouch**      | `GetInTouchProps`                             | Information and link related to contacting support or additional help. | `{ title: "Need More Help?", description: "If you have further questions or need assistance, feel free to contact us.", link: { href: "/contact", children: "Contact Us" } }` |

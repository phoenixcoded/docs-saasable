---
description: >-
  The  Faq7 component that renders a FAQ section with expandable accordions and
  a "Get in Touch" button, using MUI and custom styling.
---

# Faq7

{% hint style="info" %}
All available props for the Faq7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq7.tsx`

**Component usage path:**  `src/app/blocks/faq/faq7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq7**](https://www.saasable.io/blocks/faq/faq7)

## Props Details

| Prop                | Type                                          | Description                                                            | Displayed as                                                                                                                                                                  |
| ------------------- | --------------------------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | Main title of the FAQ section.                                         | `"Common Questions"`                                                                                                                                                          |
| **caption**         | `string` (Optional)                           | Subtitle or additional description for the FAQ section.                | `"Here are some answers to frequently asked questions about our services."`                                                                                                   |
| **defaultExpanded** | `string` (Optional)                           | Determines which FAQ panels are expanded by default.                   | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                                                               |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "What is your return policy?", answer: "You can return items within 30 days of purchase." }, ...]`                                                              |
| **getInTouch**      | `GetInTouchProps`                             | Information and link related to contacting support or additional help. | `{ title: "Need More Help?", description: "If you have additional questions or need support, feel free to contact us.", link: { href: "/contact", children: "Contact Us" } }` |

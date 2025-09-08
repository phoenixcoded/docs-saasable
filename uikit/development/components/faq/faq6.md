---
description: >-
  The  Faq6 component that renders a FAQ section with animated accordion panels,
  a "Get in Touch" button, and  topic slider using MUI, Framer Motion, and React
  Slick for enhanced interactivity and style
---

# Faq6

{% hint style="info" %}
All available props for the Faq6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq6.tsx`

**Component usage path:**  `src/app/blocks/faq/faq6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq6**](https://www.saasable.io/blocks/faq/faq6)

## Props Details

| Prop                | Type                                                                                     | Description                                                            | Displayed as                                                                                                                                                                                  |
| ------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                                                                 | Main title of the FAQ section.                                         | `"Frequently Asked Questions"`                                                                                                                                                                |
| **caption**         | `string` (Optional)                                                                      | Subtitle or additional description for the FAQ section.                | `"Find answers to common questions and get more information here."`                                                                                                                           |
| **defaultExpanded** | `string` (Optional)                                                                      | Which FAQ panels are expanded by default.                              | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                                                                               |
| **faqList**         | `Array<{question: string; answer: AnswerProps \| string; category?: string \| number;}>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "What are your operating hours?", answer: "We are open from 9 AM to 5 PM, Monday through Friday.", category: "General" }, ...]`                                                 |
| **getInTouch**      | `GetInTouchProps`                                                                        | Information and link related to contacting support or additional help. | `{ title: "Need Further Assistance?", description: "If you have more questions or need additional help, don't hesitate to contact us.", link: { href: "/contact", children: "Contact Us" } }` |
| **categories**      | `string[]`                                                                               | Array of category labels for filtering or categorizing FAQ items.      | `["General", "Billing", "Technical Support"]`                                                                                                                                                 |
| **activeCategory**  | `string` (Optional)                                                                      | The currently active or selected category from the `categories` array. | `"General"` or `undefined`                                                                                                                                                                    |

---
description: >-
  The Faq2 component renders an FAQ section with expandable accordion panels and
  a "Get in Touch" card, adapting layout and styles based on screen size and
  user focus.
---

# Faq2

{% hint style="info" %}
All available props for the Faq2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq2.tsx`

**Component usage path:**  `src/app/blocks/faq/faq2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq2**](https://www.saasable.io/blocks/faq/faq2)

## Props Details

| Prop                | Type                                          | Description                                                            | Displayed as                                                                                                                             |
| ------------------- | --------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | The main title of the FAQ section.                                     | `"Frequently Asked Questions"`                                                                                                           |
| **caption**         | `string` (Optional)                           | A subtitle or additional description for the FAQ section.              | `"Find answers to the questions most frequently asked by our customers."`                                                                |
| **defaultExpanded** | `string` (Optional)                           | Which FAQ panels are expanded by default.                              | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                          |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "How can I contact customer support?", answer: "You can contact us via email or phone." }, ...]`                           |
| **getInTouch**      | `GetInTouchProps`                             | Information and link related to contacting support or additional help. | `{ title: "Need More Help?", description: "Our support team is here to help you.", link: { href: "/contact", children: "Contact Us" } }` |

---
description: >-
  The Faq4 component that renders a FAQ section with accordion panels, styled
  with MUI components, and includes a call-to-action button for users to get in
  touch.
---

# Faq4

{% hint style="info" %}
All available props for the Faq4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq4.tsx`

**Component usage path:**  `src/app/blocks/faq/faq4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq4**](https://www.saasable.io/blocks/faq/faq4)

## Props Details

| Prop                | Type                                          | Description                                                            | Displayed as                                                                                                                                                                      |
| ------------------- | --------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | Main title of the FAQ section.                                         | `"Frequently Asked Questions"`                                                                                                                                                    |
| **caption**         | `string` (Optional)                           | Subtitle or additional description for the FAQ section.                | `"Find answers to the most common questions our users have."`                                                                                                                     |
| **defaultExpanded** | `string` or `false`                           | Which FAQ panels are expanded by default.                              | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                                                                   |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "How can I reset my password?", answer: "You can reset your password from the account settings page." }, ...]`                                                      |
| **getInTouch**      | `GetInTouchProps`                             | Information and link related to contacting support or additional help. | `{ title: "Need More Assistance?", description: "If you have any further questions, please reach out to our support team.", link: { href: "/contact", children: "Contact Us" } }` |

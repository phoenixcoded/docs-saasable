---
description: >-
  The Faq1 component displays an FAQ section with animated accordion panels and
  a styled header, featuring motion effects on scroll.
---

# Faq1

{% hint style="info" %}
All available props for the Faq1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq1.tsx`

**Component usage path:**  `src/app/blocks/faq/faq1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq1**](https://www.saasable.io/blocks/faq/faq1)

## Props Details

| Prop                | Type                                          | Description                                            | Displayed as                                                                                                     |
| ------------------- | --------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | The main title of the FAQ section.                     | `"Frequently Asked Questions"`                                                                                   |
| **caption**         | `string` (Optional)                           | A subtitle or additional context for the FAQ section.  | `"Here you'll find answers to the most common questions we receive."`                                            |
| **defaultExpanded** | `string` or `false`                           | Controls which FAQ panels are expanded by default.     | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                  |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer. | `[{ question: "What is your return policy?", answer: "You can return items within 30 days of purchase." }, ...]` |

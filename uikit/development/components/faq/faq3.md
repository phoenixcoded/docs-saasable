---
description: >-
  The Faq3 component displays a section with a heading, description, and a list
  of FAQs in collapsible panels, alongside a "Get in Touch" card with a
  background image.
---

# Faq3

{% hint style="info" %}
All available props for the Faq3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the faq section.
{% endhint %}

**Component path**: `src/blocks/faq/Faq3.tsx`

**Component usage path:**  `src/app/blocks/faq/faq3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/faq/faq3**](https://www.saasable.io/blocks/faq/faq3)

## Props Details

| Prop                | Type                                          | Description                                                            | Displayed as                                                                                                                                        |
| ------------------- | --------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**         | `string`                                      | Main title of the FAQ section.                                         | `"Frequently Asked Questions"`                                                                                                                      |
| **caption**         | `string` (Optional)                           | Subtitle or additional description for the FAQ section.                | `"Here you can find answers to the most common questions about our services."`                                                                      |
| **defaultExpanded** | `string` (Optional)                           | Which FAQ panels are expanded by default.                              | `"panel0"` (expands the first panel) or `false` (no panels expanded by default)                                                                     |
| **faqList**         | `Array<{ question: string, answer: string }>` | List of FAQ items, each with a question and an answer.                 | `[{ question: "What is the return policy?", answer: "Returns are accepted within 30 days." }, ...]`                                                 |
| **getInTouch**      | `GetInTouchProps`                             | Information and link related to contacting support or additional help. | `{ title: "Need More Help?", description: "Contact our support team for further assistance.", link: { href: "/contact", children: "Contact Us" } }` |
| **bgImage**         | `BgImageProps`                                | Background image URL for the `GraphicsCard`.                           | `"https://example.com/background.jpg"`                                                                                                              |

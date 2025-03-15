---
description: >-
  The Pricing7 component displays a pricing section with toggleable monthly and
  yearly views, featuring a main plan card with price details and a benefits
  list with icons and descriptions.
---

# Pricing7

{% hint style="info" %}
All available props for the Pricing7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing7.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing7**](https://www.saasable.io/blocks/pricing/pricing7)

## Props Details

| Prop            | Type                 | Description                                                                                    | Displayed as                                                               |
| --------------- | -------------------- | ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| **heading**     | `string`             | Main heading for the pricing section                                                           | `"Our Pricing Plans"`                                                      |
| **caption**     | `string`             | Additional context or description for the heading                                              | `"Choose the plan that best fits your needs"`                              |
| **defaultUnit** | `string`             | Default time unit for pricing display (`'monthly'` or `'yearly'`)                              | `"per month"`                                                              |
| **plans**       | `Pricing3PlanProps`  | Details about a specific pricing plan, including title, description, price, features, and link | `{ title: "Pro Plan", ... }`                                               |
| **benefitList** | `BenefitListProps[]` | List of benefits with icons, titles, and descriptions                                          | `[ { icon: { name: "tabler-crown" }, title: "Exclusive Features", ... } ]` |

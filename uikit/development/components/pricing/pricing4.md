---
description: >-
  The Pricing4 component displays two pricing plans with a toggle to switch
  between monthly and yearly pricing, featuring detailed plan information, a
  list of features, and action buttons.
---

# Pricing4

{% hint style="info" %}
All available props for the Pricing4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing4.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing4**](https://www.saasable.io/blocks/pricing/pricing4)

## Props Details

| Prop            | Type                  | Description                                                                       | Displayed as                                                                                |
| --------------- | --------------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| **heading**     | `string`              | Main title of the pricing section                                                 | `"Our Pricing Options"`                                                                     |
| **caption**     | `string`              | Subtitle or description for additional context                                    | `"Select a plan that suits your needs. Enjoy flexibility with monthly or yearly billing."`  |
| **defaultUnit** | `string`              | Unit of measurement for pricing                                                   | `"per month"`                                                                               |
| **plans**       | `Pricing3PlanProps[]` | Array of plan objects with details like title, description, price, features, etc. | Array of plan objects, e.g., `[ { title: "Basic Plan", ... }, { title: "Pro Plan", ... } ]` |

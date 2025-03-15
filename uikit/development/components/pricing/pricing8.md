---
description: >-
  The Pricing8 component presents a pricing section with toggleable monthly and
  yearly plans, featuring cards for each plan that include a price, quantity
  controls, and a list of features.
---

# Pricing8

{% hint style="info" %}
All available props for the Pricing8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing8.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing8**](https://www.saasable.io/blocks/pricing/pricing8)

## Props Details

| Prop            | Type                  | Description                        | Displayed as                                                                    |
| --------------- | --------------------- | ---------------------------------- | ------------------------------------------------------------------------------- |
| **heading**     | `string`              | Main title for the pricing section | `"Choose Your Plan"`                                                            |
| **caption**     | `string` (Optional)   | Additional description or context  | `"Select a plan that fits your needs"`                                          |
| **defaultUnit** | `string` (Optional)   | Default time unit for pricing      | `"monthly"`                                                                     |
| **features**    | `FeatureProps[]`      | Array of available features        | `[{ id: 1, label: "Basic support" }, ...]`                                      |
| **plans**       | `Pricing5PlanProps[]` | Array of pricing plan details      | `[{ title: "Basic Plan", description: "For individuals...", price: "9", ... }]` |

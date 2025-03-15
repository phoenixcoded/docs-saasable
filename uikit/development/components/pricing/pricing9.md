---
description: >-
  The Pricing9 component displays a pricing section with animated cards for
  different plans, each featuring a title, price, list of features, and buttons
  for exploring or linking to more information.
---

# Pricing9

{% hint style="info" %}
All available props for the Pricing9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing9.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing9**](https://www.saasable.io/blocks/pricing/pricing9)

## Props Details

| Property     | Type                  | Description                                  | Displayed as                                       |
| ------------ | --------------------- | -------------------------------------------- | -------------------------------------------------- |
| **heading**  | `string`              | Main title for the pricing section           | `"Our Pricing Plans"`                              |
| **caption**  | `string` (Optional)   | Optional additional description or context   | `"Choose a plan that suits your needs"`            |
| **plans**    | `Pricing5PlanProps[]` | Array of pricing plan details                | `[{ title: "Basic Plan", price: "19", ... }, ...]` |
| **features** | `FeatureProps[]`      | Array of features available in pricing plans | `[{ id: 1, label: "24/7 Support" }, ...]`          |

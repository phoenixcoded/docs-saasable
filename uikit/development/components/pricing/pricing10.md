---
description: >-
  Pricing10 displays animated pricing cards with monthly/yearly toggle, showing
  plan icons, titles, prices, features, and action buttons.
---

# Pricing10



{% hint style="info" %}
All available props for the Pricing10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing10.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing10**](https://www.saasable.io/blocks/pricing/pricing10)

## Props Details

| Property    | Type                  | Description                                | Displayed as                                       |
| ----------- | --------------------- | ------------------------------------------ | -------------------------------------------------- |
| **heading** | `string`              | Main title for the pricing section         | `"Our Pricing Plans"`                              |
| **caption** | `string`              | Optional additional description or context | `"Choose a plan that suits your needs"`            |
| **plans**   | `Pricing5PlanProps[]` | Array of pricing plan details              | `[{ title: "Basic Plan", price: "19", ... }, ...]` |

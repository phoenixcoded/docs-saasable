# Pricing6

The `Pricing6` component is designed to present pricing plans and features in a structured format. It combines visual components with tabular data to provide a clear comparison of different plans and their features.

{% hint style="info" %}
All available props for the Pricing6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing6.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing6**](https://www.saasable.io/blocks/pricing/pricing6)

## Props Details

| Prop         | Type                  | Description                                                                          | Displayed as                                                                                                                                                |
| ------------ | --------------------- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**  | `string`              | Main heading or title of the pricing section.                                        | `"Our Pricing Plans"`                                                                                                                                       |
| **caption**  | `string` (Optional)   | Optional subtitle or description for additional context.                             | `"Choose the plan that's right for you."`                                                                                                                   |
| **features** | `FeatureProps[]`      | Array of features compared across different plans.                                   | `[{ id: 1, label: "Feature A" }, { id: 2, label: "Feature B" }]`                                                                                            |
| **plans**    | `Pricing4PlanProps[]` | Array of pricing plans with details such as title, price, description, and features. | `[ { title: "Basic", price: "$10", description: "Basic plan", features: [1] }, { title: "Pro", price: "$20", description: "Pro plan", features: [1, 2] } ]` |

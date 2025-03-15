# Pricing3

The `Pricing3` component renders a responsive pricing section with detailed plan cards that display features, pricing, and additional information, organized in a grid layout and including buttons for exploring each plan.

{% hint style="info" %}
All available props for the Pricing3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing3.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing3**](https://www.saasable.io/blocks/pricing/pricing3)

## Props Details

| Prop            | Type                | Description                                                             | Displayed as                              |
| --------------- | ------------------- | ----------------------------------------------------------------------- | ----------------------------------------- |
| **heading**     | `string`            | Main title of the pricing section                                       | `"Our Pricing Plans"`                     |
| **caption**     | `string` (Optional) | Optional subtitle or description                                        | `"Choose the plan that's right for you."` |
| **defaultUnit** | `string`            | Unit of measurement for pricing                                         | `"per month"`                             |
| **plans**       | `PlanProps[]`       | Array of plan objects with details like title, description, price, etc. | See example in code above                 |

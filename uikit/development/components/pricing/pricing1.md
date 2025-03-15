# Pricing1

The `Pricing1` component displays a responsive pricing section with animated card elements for different pricing plans. It includes a heading and optional caption, renders each plan's title, price, features, and description, and provides a button for exploring each plan.

{% hint style="info" %}
All available props for the Pricing1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing1.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing1**](https://www.saasable.io/blocks/pricing/pricing1)

## Props Details

| Prop            | Type                | Description                                               | Displayed as                                                  |
| --------------- | ------------------- | --------------------------------------------------------- | ------------------------------------------------------------- |
| **heading**     | `string`            | Main heading text of the section.                         | `"Our Pricing Plans"`                                         |
| **caption**     | `string` (Optional) | Additional caption below the heading (optional).          | `"Choose the plan that's right for you."`                     |
| **defaultUnit** | `string`            | Unit of currency or measurement (optional).               | `"per month"`                                                 |
| **plans**       | `PlanProps[]`       | Array of plan objects with details for each pricing plan. | `[ { title: "Basic Plan", price: "29", features: [ ... ] } ]` |

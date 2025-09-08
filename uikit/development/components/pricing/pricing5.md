# Pricing5

The `Pricing5` component offers a flexible pricing layout with options to toggle between monthly and yearly plans, and displays a set of pricing options with detailed plan information, feature lists, and action buttons.

{% hint style="info" %}
All available props for the Pricing5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing5.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing5**](https://www.saasable.io/blocks/pricing/pricing5)

## Props Details

| Prop            | Type                | Description                                                             | Displayed as                                                                                |
| --------------- | ------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| **heading**     | `string`            | Main heading for the pricing section                                    | `"Choose Your Plan"`                                                                        |
| **caption**     | `string` (Optional) | Optional caption providing additional context                           | `"Choose the plan that's right for you."`                                                   |
| **defaultUnit** | `string` (Optional) | Optional unit of measurement or billing cycle description               | `"per month"`                                                                               |
| **user**        | `string` (Optional) | Optional label or identifier for the type of user                       | `"Best for 1-50 users"`                                                                     |
| **plans**       | `PlanProps[]`       | Array of plan objects with details such as title, price, features, etc. | Array of plan objects, e.g., `[ { title: "Basic Plan", ... }, { title: "Pro Plan", ... } ]` |


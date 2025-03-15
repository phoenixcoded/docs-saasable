# Pricing2

The `Pricing2` component is a responsive pricing table that displays feature-based plans with options to toggle between monthly and yearly billing, showing detailed pricing and feature availability for each plan.

{% hint style="info" %}
All available props for the Pricing2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the pricing section.
{% endhint %}

**Component path**: `src/blocks/pricing/Pricing2.tsx`

**Component usage path:**  `src/app/blocks/pricing/pricing2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/pricing/pricing2**](https://www.saasable.io/blocks/pricing/pricing2)

## Props Details

| Prop            | Type                  | Description                                      | Displayed as                                      | Usage                                           |
| --------------- | --------------------- | ------------------------------------------------ | ------------------------------------------------- | ----------------------------------------------- |
| **heading**     | `string`              | Main title of the pricing section                | `"Our Pricing Plans"`                             | Displays the main heading                       |
| **caption**     | `string` (Optional)   | Optional subtitle or additional context          | `"Find the best plan that suits your needs."`     | Provides additional context below heading       |
| **defaultUnit** | `string` (Optional)   | Default billing unit (`'monthly'` or `'yearly'`) | `'monthly'`                                       | Sets the initial view for pricing               |
| **features**    | `FeatureProps[]`      | List of features for comparison                  | `[ { id: 'feature1', label: 'Feature 1' }, ... ]` | Lists features in the comparison table          |
| **plans**       | `Pricing2PlanProps[]` | Array of pricing plans with details              | `[ { title: 'Basic Plan', ... }, ... ]`           | Provides pricing plans, descriptions, and links |

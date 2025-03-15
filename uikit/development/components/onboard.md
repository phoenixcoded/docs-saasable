# Onboard

The OnBoard component that renders a full-height onboarding section with a gradient floating action button, a logo, decorative circles, and optional primary and secondary buttons, all within a styled container

{% hint style="info" %}
All available props for the Onboard component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Onboard section.
{% endhint %}

**Component path**: `src/blocks/Onboard.tsx`

**Component usage path:**  `src/app/blocks/onboard/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/onboard**](https://www.saasable.io/blocks/onboard)

## Props Details

| Prop             | Type          | Description                                                                               | Displayed as                                                                     |
| ---------------- | ------------- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| **heading**      | `string`      | A required string for the main heading or title in the `Typeset` component.               | `"Welcome to Our Platform"`                                                      |
| **caption**      | `string`      | A required string for additional descriptive text or subtitle in the `Typeset` component. | `"Get started by exploring the features we offer and sign up for early access."` |
| **primaryBtn**   | `ButtonProps` | A required object with properties for the primary `Button` component.                     | `{ children: 'Get Started', onClick: () => alert('Primary Button Clicked!') }`   |
| **secondaryBtn** | `ButtonProps` | A required object with properties for the secondary `Button` component.                   | `{ children: 'Learn More', onClick: () => alert('Secondary Button Clicked!') }`  |

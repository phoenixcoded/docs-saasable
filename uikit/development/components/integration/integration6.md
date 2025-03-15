# Integration6

`Integration6` that displays a series of overlapping circular icons and an array of brand icons within a centered grid layout, along with a headline, caption, and a primary button, using Material-UI for styling and layout.

{% hint style="info" %}
All available props for the Integration6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration6.tsx`

**Component usage path:**  `src/app/blocks/integration/integration6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration6**](https://www.saasable.io/blocks/integration/integration6)

## Props Details

| Prop            | Type          | Description                              | Displayed as                                                              |
| --------------- | ------------- | ---------------------------------------- | ------------------------------------------------------------------------- |
| **headLine**    | `string`      | Main heading or title of the section     | `"Connect with top-tier tools available Interface"`                       |
| **captionLine** | `string`      | Additional descriptive text or subtitle  | `"Discover the features that will transform your customer relationships"` |
| **primaryBtn**  | `ButtonProps` | Properties for the primary action button | `{ variant: "contained", color: "primary", children: "Get Started" }`     |

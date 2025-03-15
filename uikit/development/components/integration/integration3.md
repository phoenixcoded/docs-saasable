# Integration3

The `Integration3` component displays a section with a centered headline, caption, and button, followed by a grid of integration logos (as avatars) laid out in a responsive grid. The component uses Material UI for styling, and avatars are rendered using the `IntegrationAvatar` component, with each logo represented by an image.

{% hint style="info" %}
All available props for the Integration3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the integration section.
{% endhint %}

**Component path**: `src/blocks/integration/Integration3.tsx`

**Component usage path:**  `src/app/blocks/integration/integration3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/integration/integration3**](https://www.saasable.io/blocks/integration/integration3)

## Props Details

| Prop            | Type          | Description                                   | Displayed as                                                       |
| --------------- | ------------- | --------------------------------------------- | ------------------------------------------------------------------ |
| **headLine**    | `string`      | Main headline or title of the section.        | `"Integrate with the Best"`                                        |
| **captionLine** | `string`      | Secondary text or caption below the headline. | `"Seamlessly connect with popular platforms"`                      |
| **primaryBtn**  | `ButtonProps` | Props for the primary button.                 | `{ variant: "contained", size: "large", children: "Get Started" }` |

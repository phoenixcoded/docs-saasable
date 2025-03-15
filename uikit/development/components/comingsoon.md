# ComingSoon

The `ComingSoon` component that displays a full-screen section with a centered "Coming Soon" graphic, an optional chip with a caption, a description text, and an email input field with a primary button for submissions. The background includes a decorative circles SVG, and the layout is styled to be responsive and centered.

{% hint style="info" %}
All available props for the ComingSoon component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the comingsoon section.
{% endhint %}

**Component path**: `src/blocks/ComingSoon.tsx`

**Component usage path:**  `src/app/blocks/coming-soon/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/coming-soon**](https://www.saasable.io/blocks/coming-soon)

## Props Details

| Prop            | Type                                 | Description                                                                                                 | Displayed as                                                     |
| --------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| **chip**        | `{ chipCaption: string }` (Optional) | An optional object that represents the caption text for a chip. If not provided, no chip is displayed.      | `{ chipCaption: 'New Feature' }`                                 |
| **description** | `string`                             | A required string that describes the "Coming Soon" message.                                                 | `"We are working on something amazing. Stay tuned for updates!"` |
| **primaryBtn**  | `ButtonProps`                        | A required object for the button properties that appears as the end adornment in the `OutlinedInput` field. | `{ children: 'Subscribe', onClick: () => alert('Subscribed!') }` |

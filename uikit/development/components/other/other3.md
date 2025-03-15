# Other3

The Other3 that renders a section with a heading, caption, and a list of cards displaying titles, descriptions, chips, and buttons, utilizing MUI's Stack, Chip, and Typography components for layout and styling.

{% hint style="info" %}
All available props for the Other3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the other section.
{% endhint %}

**Component path**: `src/blocks/other/Other3.tsx`

**Component usage path:**  `src/app/blocks/other/other3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/other/other3**](https://www.saasable.io/blocks/other/other3)

## Props Details

| Prop        | Type               | Description                                                                                   | Display As                                      |
| ----------- | ------------------ | --------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| **heading** | `string`           | The title or heading that is displayed at the top of the section.                             | Displayed as the main title of the section.     |
| **caption** | `string`           | A description or subtitle for the section.                                                    | Displayed as a subtitle below the main heading. |
| **other**   | `OtherListProps[]` | An array of objects, each representing a card with a title, description, chips, and a button. | Displays feature cards in a list layout.        |

# Error500

`Error500Page` displays a full-page error 500 message with an illustration, heading, and optional button, all within a styled container.

{% hint style="info" %}
All available props for the Error 500 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Error 500 section.
{% endhint %}

**Component path**: `src/blocks/maintenance/Error500.tsx`

**Component usage path:**  `src/app/blocks/error500/page.tsx`&#x20;

**Preview link: https://www.saasable.io/blocks/maintenance/error500**

## Props Details

| Prop        | Type          | Description                                                                          | Displayed as                        |
| ----------- | ------------- | ------------------------------------------------------------------------------------ | ----------------------------------- |
| **heading** | `string`      | A required string for the main title or heading in the component.                    | `"Join Our Early Access Program"`   |
| primaryBtn  | `ButtonProps` | Material UI `Button` props object. If passed, it renders a button below the heading. | A button (e.g., “Go Back”, “Retry”) |

# NavbarContent2

This code defines a responsive navigation bar component (`NavbarContent2`) that displays a logo, navigation menu, localization selector, and a "Get Started" button, with adjustments for different screen sizes using Material-UI's breakpoints and conditional rendering.

{% hint style="info" %}
All available props for the NavbarContent2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent2.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar2**](https://www.saasable.io/blocks/navbar/navbar2)

## Props Details

| Prop              | Type                                                               | Description                                                         | Displayed as                                                |
| ----------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------- | ----------------------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details.          | It will display navigation items and sections.              |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                         | `{ children: 'Get Started' }`                               |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.                       | `{ children: 'Buy Now' }`                                   |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.                     | It will display theme customization section.                |
| landingBaseUrl    | `string`                                                           | The base URL for the landing page; used for the logo redirect.      | A **clickable logo** that sends users to the given page.    |
| animated          | `boolean`                                                          | Whether to animate the primary button with a pulsing shadow effect. | Animation on primary button                                 |
| selectedTheme     | `Theme`                                                            | The currently selected theme mode.                                  | Passed to `<Customization selectedTheme={selectedTheme} />` |

# NavbarContent1

This component navbarcontent1 is designed to create a dynamic, responsive navigation bar that adjusts its layout based on screen size. The navbar includes a logo, navigation items, social media icons, and a "Get Started" button. On smaller screens, a popper/drawer-based navigation system is used to improve usability in a compact space.

{% hint style="info" %}
All available props for the NavbarContent1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent1.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar1**](https://www.saasable.io/blocks/navbar/navbar1)

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


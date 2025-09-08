# NavbarContent7

This `NavbarContent7` component is a responsive navigation bar that adapts to different screen sizes using Material-UI. It features a logo, a navigation menu, a "Get Started" button, and a popper menu for smaller screens.

{% hint style="info" %}
All available props for the NavbarContent7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent7.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar7**](https://www.saasable.io/blocks/navbar/navbar7)

## Props Details

| Prop              | Type                                                               | Description                                                    | Displayed as                                                |
| ----------------- | ------------------------------------------------------------------ | -------------------------------------------------------------- | ----------------------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details.     | It will display navigation items and sections.              |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                    | `{ children: 'Get Started' }`                               |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.                  | `{ children: 'Buy Now' }`                                   |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.                | It will display theme customization section.                |
| landingBaseUrl    | `string`                                                           | The base URL for the landing page; used for the logo redirect. | A **clickable logo** that sends users to the given page.    |
| selectedTheme     | `Theme`                                                            | The currently selected theme mode.                             | Passed to `<Customization selectedTheme={selectedTheme} />` |


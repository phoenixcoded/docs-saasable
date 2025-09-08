# NavbarContent8

This component, `NavbarContent8`, dynamically displays a responsive navigation bar that splits provided navigation items into two groups for larger screens and utilizes a popper menu for smaller screens, incorporating a logo and a "Get Started" button.

{% hint style="info" %}
All available props for the NavbarContent8 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent8.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar8/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar8**](https://www.saasable.io/blocks/navbar/navbar8)

## Props Details

| Prop              | Type                                                               | Description                                                    | Displayed as                                                |
| ----------------- | ------------------------------------------------------------------ | -------------------------------------------------------------- | ----------------------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details.     | It will display navigation items and sections.              |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                    | `{ children: 'Get Started' }`                               |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.                  | `{ children: 'Buy Now' }`                                   |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.                | It will display theme customization section.                |
| landingBaseUrl    | `string`                                                           | The base URL for the landing page; used for the logo redirect. | A **clickable logo** that sends users to the given page.    |
| selectedTheme     | `Theme`                                                            | The currently selected theme mode.                             | Passed to `<Customization selectedTheme={selectedTheme} />` |

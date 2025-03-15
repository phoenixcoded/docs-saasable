# NavbarContent9

This component, `NavbarContent9`, renders a responsive navigation bar featuring a logo, navigation menus for larger screens, and a popper menu for smaller screens, including options for user sign-in and a "Get Started" button.

{% hint style="info" %}
All available props for the NavbarContent9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent9.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar9**](https://www.saasable.io/blocks/navbar/navbar9)

## Props Details

| Prop              | Type                                                               | Description                                                | Displayed as                                   |
| ----------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details. | It will display navigation items and sections. |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                | `{ children: 'Get Started' }`                  |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.              | `{ children: 'Buy Now' }`                      |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.            | It will display theme customization section.   |

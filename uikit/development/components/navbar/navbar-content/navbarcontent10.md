# NavbarContent10

This component, `NavbarContent10`, implements a responsive navigation bar featuring a logo, navigation menu, user sign-in, and "Get Started" buttons, along with customizable theme and direction settings through a settings popper for larger screens, while adapting to smaller screens with a collapsible menu.

{% hint style="info" %}
All available props for the NavbarContent10 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent10.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar10/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar10**](https://www.saasable.io/blocks/navbar/navbar10)

## Props Details

| Prop              | Type                                                               | Description                                                | Displayed as                                   |
| ----------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details. | It will display navigation items and sections. |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                | `{ children: 'Get Started' }`                  |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.              | `{ children: 'Buy Now' }`                      |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.            | It will display theme customization section.   |

# NavbarContent3

This code defines a responsive navigation bar component (`NavbarContent3`) that includes a logo, navigation menu, search input, and "Get Started" button, with layout and visibility adjustments based on screen size using Material-UI's breakpoints and conditional rendering.

{% hint style="info" %}
All available props for the NavbarContent3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent3.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar3**](https://www.saasable.io/blocks/navbar/navbar3)

## Props Details

| Prop              | Type                                                               | Description                                                | Displayed as                                   |
| ----------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details. | It will display navigation items and sections. |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                | `{ children: 'Get Started' }`                  |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.              | `{ children: 'Buy Now' }`                      |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.            | It will display theme customization section.   |

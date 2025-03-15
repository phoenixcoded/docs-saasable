# NavbarContent5

This code defines a responsive navigation bar component (`NavbarContent5`) that includes a logo, navigation menu, "Get Started" button, and a collapsible search input. It adjusts the layout and visibility of these elements based on screen size using Material-UI's breakpoints, with a popper menu on smaller screens and conditional rendering for a search bar with an icon trigger.

{% hint style="info" %}
All available props for the NavbarContent5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent5.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar5**](https://www.saasable.io/blocks/navbar/navbar5)

## Props Details

| Prop              | Type                                                               | Description                                                | Displayed as                                   |
| ----------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details. | It will display navigation items and sections. |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                | `{ children: 'Get Started' }`                  |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.              | `{ children: 'Buy Now' }`                      |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.            | It will display theme customization section.   |

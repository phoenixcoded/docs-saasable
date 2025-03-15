# NavbarContent6

This code defines a responsive navigation bar component (`NavbarContent6`) with specific features for different screen sizes. It uses Material-UI components and styles to adjust the layout for smaller and larger screens, managing navigation items, logos, and icons efficiently.

{% hint style="info" %}
All available props for the NavbarContent6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the NavbarContent section.
{% endhint %}

**Component path**: `src/blocks/navbar/navbar-content/NavbarContent6.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar6**](https://www.saasable.io/blocks/navbar/navbar6)

## Props Details

| Prop              | Type                                                               | Description                                                | Displayed as                                   |
| ----------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- | ---------------------------------------------- |
| **navItems**      | Array of [`NavItemProps`](../navmenu.md#navitems-props) (Optional) | nav items using `NavItemProps` interface for item details. | It will display navigation items and sections. |
| **primaryBtn**    | `ButtonProps` (Optional)                                           | Optional properties for the primary button.                | `{ children: 'Get Started' }`                  |
| **secondaryBtn**  | `ButtonProps` (Optional)                                           | Optional properties for the secondary button.              | `{ children: 'Buy Now' }`                      |
| **customization** | `boolean` (Optional)                                               | Optional prop to display customization section.            | It will display theme customization section.   |

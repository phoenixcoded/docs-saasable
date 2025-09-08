# Navbar9

`Navbar9` is a responsive navigation bar component that utilizes MUI's `AppBar`, `Toolbar`, and `Box`, allowing for customizable content through the `children` prop, with responsive styling and padding adjustments based on screen size.

{% hint style="info" %}
All available props for the Navbar9 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Navbar section.
{% endhint %}

**Component path**: `src/blocks/navbar/Navbar9.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar9/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar9**](https://www.saasable.io/blocks/navbar/navbar9)

## Props Details

| Prop         | Type           | Description                                                                                                                                                                                                                     | Display as                                                                                                  |
| ------------ | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **children** | `ReactElement` | A single React element or component that will be rendered inside the `StyledToolbar` of the `AppBar`. This prop allows for custom content such as logos, navigation links, or any other elements to be displayed in the navbar. | Elements that will be displayed inside the navigation bar                                                   |
| isFixed      | `boolean`      | Determines if the navbar stays fixed at the top when scrolling. true = fixed, false = static position.                                                                                                                          | If `true`: `position: fixed` with spacing offset below it. If `false`: `position: static`, no offset added. |
| ...props     | `object`       | Additional props passed down to `ElevationScroll` and `AppBar`.                                                                                                                                                                 | Any valid props like `id, className, sx,` etc., are spread to internal components.                          |


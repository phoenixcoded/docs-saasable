# Navbar2

`Navbar2` is a responsive navigation bar component that uses MUI's `AppBar`, `Toolbar`, and `Box`, providing customizable content through the `children` prop, while applying specific styling and padding based on the screen size.

{% hint style="info" %}
All available props for the Navbar2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Navbar section.
{% endhint %}

**Component path**: `src/blocks/navbar/Navbar2.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar2/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar2**](https://www.saasable.io/blocks/navbar/navbar2)

## Props Details

| Prop         | Type           | Description                                                                                                                                                                                                                     | Display as                                                |
| ------------ | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| **children** | `ReactElement` | A single React element or component that will be rendered inside the `StyledToolbar` of the `AppBar`. This prop allows for custom content such as logos, navigation links, or any other elements to be displayed in the navbar. | Elements that will be displayed inside the navigation bar |

# Navbar6

`Navbar6` is a centered navigation bar component utilizing MUI's `AppBar` and `Toolbar`, allowing customizable content through the `children` prop, while implementing responsive styling and padding adjustments for various screen sizes.

{% hint style="info" %}
All available props for the Navbar6 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Navbar section.
{% endhint %}

**Component path**: `src/blocks/navbar/Navbar6.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar6/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar6**](https://www.saasable.io/blocks/navbar/navbar6)

## Props Details

| Prop         | Type           | Description                                                                                                                                                                                                                     | Display as                                                |
| ------------ | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| **children** | `ReactElement` | A single React element or component that will be rendered inside the `StyledToolbar` of the `AppBar`. This prop allows for custom content such as logos, navigation links, or any other elements to be displayed in the navbar. | Elements that will be displayed inside the navigation bar |

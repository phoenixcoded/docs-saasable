---
description: >-
  The MegaMenu4 component renders a grid of menu items as clickable cards,
  optionally including a footer section, with customizable width and footer
  styling.
---

# MegaMenu4

{% hint style="info" %}
All available props for the MegaMenu4 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the megamenu section.
{% endhint %}

**Component path**: `src/blocks/mega-menu/MegaMenu4.tsx`

**Component usage path:**  `src/app/blocks/megamenu/megamenu4/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/megamenu/megamenu4**](https://www.saasable.io/blocks/megamenu/megamenu4)

## Props Details

| Prop            | Type                   | Description                                                                          | Displayed as                                                                                                                                       |
| --------------- | ---------------------- | ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| **menuItems**   | `MenuItemsProps[]`     | Array of menu item objects, each with `link` and other properties for `PreviewCard`. | <p>Displays a grid-based layout of menu items </p><p>where each item appears as a clickable card using the <code>PreviewCard</code> component.</p> |
| **footerData**  | `ReactNode` (Optional) | Content to be displayed in the footer. Can be any valid React element.               | Renders a footer section beneath the grid, which can display custom content like links, text, or buttons.                                          |
| **popperWidth** | `number` (Optional)    | Maximum width of the mega menu. Defaults to `936`.                                   | Determines the maximum width of the menu container. Defaults to 936px and adjusts responsively for smaller screens.                                |
| **footerSX**    | `SxProps` (Optional)   | Style object for customizing the footer's appearance.                                | Allows customization of the footer’s styles, enabling changes to padding, colors, or layout to better align with design requirements.              |

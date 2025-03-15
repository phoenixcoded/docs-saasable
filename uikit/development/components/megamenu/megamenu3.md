---
description: >-
  The MegaMenu3 component displays a responsive menu with icons and text, and
  optionally includes a footer section. It supports customizable popper width
  and styling for the footer.
---

# MegaMenu3

{% hint style="info" %}
All available props for the MegaMenu3 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the megamenu section.
{% endhint %}

**Component path**: `src/blocks/mega-menu/MegaMenu3.tsx`

**Component usage path:**  `src/app/blocks/megamenu/megamenu3/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/megamenu/megamenu3**](https://www.saasable.io/blocks/megamenu/megamenu3)

## Props Details

| Prop            | Type                   | Description                                                            | Displayed as                                                                                                                                                                                                         |
| --------------- | ---------------------- | ---------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **menuItems**   | `MenuItemsProps[]`     | Array of menu item objects, each with `icon`, `title`, and `content`.  | Renders a grid-style menu where each item appears as a button which containing a title, an optional icon  and additional content. The items are styled for responsiveness, adapting their layout on smaller screens. |
| **footerData**  | `ReactNode` (Optional) | Content to be displayed in the footer. Can be any valid React element. | Adds a footer section below the menu items, displaying any content passed as a React node.                                                                                                                           |
| **popperWidth** | `number` (Optional)    | Maximum width of the mega menu. Defaults to `725`.                     | Adjusts the maximum width of the entire menu container. Defaults to 725px but adapts to smaller screens for responsive design.                                                                                       |
| **footerSX**    | `SxProps` (Optional)   | Style object for customizing the footer's appearance.                  | Customizes the appearance of the footer section, including its padding, background color, or any additional styles that alter its layout or look.                                                                    |

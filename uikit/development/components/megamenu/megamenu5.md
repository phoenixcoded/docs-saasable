# MegaMenu5

This code defines a React component `MegaMenu5` that creates a responsive mega menu layout using MUI components. It features a grid with optional `bannerData` on the left and menu items on the right. Each menu category includes a title and a list of links, where each item can have a title, content, and an optional icon. The layout adjusts dynamically based on the number of menu items, and the menu uses MUI's `List` and `ListItemButton` components for interactivity and styling.

{% hint style="info" %}
All available props for the MegaMenu5 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the megamenu section.
{% endhint %}

**Component path**: `src/blocks/mega-menu/MegaMenu5.tsx`

**Component usage path:**  `src/app/blocks/megamenu/megamenu5/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/megamenu/megamenu5**](https://www.saasable.io/blocks/megamenu/megamenu5)

## Props Details

| Prop            | Type                   | Description                                                                                                                                                      | Display in UI                                                                                                                                           |
| --------------- | ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **menuItems**   | `MenuItemsProps[]`     | An array of objects, each containing a `title` and an `itemsList`. `itemsList` contains the individual menu options, each with a `title`, `content`, and `link`. | Menu items are displayed in a grid format. Each section has a subheader (the title), followed by a list of clickable items with descriptions (content). |
| **bannerData**  | `ReactNode` (Optional) | Custom content (e.g., an image or banner) displayed on the left side of the menu if provided.                                                                    | The banner is displayed on the left side in a box with padding and a background color.                                                                  |
| **popperWidth** | `number` (Optional)    | Defines the width of the menu's pop-up (popover) when it is rendered. The default width is **750px**, but this can be customized.                                | The pop-up width affects how wide the entire menu layout appears on the screen. It adjusts the container that holds the menu and banner.                |

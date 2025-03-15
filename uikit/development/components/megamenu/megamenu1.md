# MegaMenu1

The `MegaMenu1` component displays a responsive menu with icon-based list items and an optional footer section containing a title, button, and additional list items, styled with Material UI components and custom styling.

{% hint style="info" %}
All available props for the MegaMenu1 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the megamenu section.
{% endhint %}

**Component path**: `src/blocks/mega-menu/MegaMenu1.tsx`

**Component usage path:**  `src/app/blocks/megamenu/megamenu1/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/megamenu/megamenu1**](https://www.saasable.io/blocks/megamenu/megamenu1)

## Props Details

| Prop           | Type                         | Description                                                                | Displayed as                                                                                                                                                                                                |
| -------------- | ---------------------------- | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **menuItems**  | `MenuItemsProps[]`           | Array of menu item objects, each with `icon`, `title`, and `content`.      | Displays a vertical list of menu options, with each option containing a title, an optional icon  and additional content. The items are styled for responsiveness, adapting their layout on smaller screens. |
| **footerData** | `MenuFooterProps` (Optional) | Object for footer section, including `title`, `link`, and optional `list`. | Renders a footer section below the menu items. The footer includes a title with a hover effect, a button linking to additional content, and an optional list for more detailed information.                 |
| **footerSX**   | `SxProps` (Optional)         | Style object for customizing the footer's appearance.                      | Customizes the appearance of the footer section, including its padding, background color, or any additional styles that alter its layout or look.                                                           |

# NavMenu

This common shared component provides a flexible and responsive navigation system for a website. It adapts navigation behavior based on screen size and uses dynamic rendering for enhanced usability.

**Component path**: `src/components/navbar/NavItems.tsx`

## NavMenu Props

<table><thead><tr><th>Prop</th><th width="216">Type</th><th width="205">Description</th><th>Display as</th></tr></thead><tbody><tr><td><strong>navItems</strong></td><td>Array of <a href="navmenu.md#navitems-props"><code>NavItemProps</code></a></td><td>nav items using <code>NavItemProps</code> interface for item details.</td><td>It will display navigation items and sections.</td></tr><tr><td><strong>menuTextColor</strong></td><td><code>string</code> (Optional)</td><td>The color for menu item text.</td><td>This will affect on navigation button's text color.</td></tr></tbody></table>

## NavItems Props&#x20;

<table><thead><tr><th>Prop</th><th width="216">Type</th><th width="205">Description</th><th>Display as</th></tr></thead><tbody><tr><td><strong>id</strong></td><td><code>string | number</code></td><td>Unique identifier for the navigation item.</td><td>Used internally to identify and manage the nav item.</td></tr><tr><td><strong>title</strong></td><td><code>string</code></td><td>The display title of the navigation item.</td><td>Displayed text for the navigation item (e.g., "Home").</td></tr><tr><td><strong>link</strong></td><td><code>string</code> (Optional)</td><td>Link for the navigation item (URL).</td><td>Hyperlink target (where the user goes when the item is clicked).</td></tr><tr><td><strong>target</strong></td><td><code>string</code> (Optional)</td><td>Target attribute (e.g., <code>_blank</code> for opening in a new tab).</td><td>Defines how the link will open (e.g., same tab or new tab).</td></tr><tr><td><strong>icon</strong></td><td><code>SpriteIconProps</code> (Optional)</td><td>Icon for the navigation item, defined by the <code>SpriteIconProps</code> type.</td><td>An icon displayed next to the title (e.g., home icon).</td></tr><tr><td><strong>expanded</strong></td><td><code>boolean</code> (Optional)</td><td>Indicates whether the item is expanded (used for dropdowns or mega menus).</td><td>Shows whether the dropdown/mega menu for this item is open.</td></tr><tr><td><strong>megaMenu</strong></td><td><a href="navmenu.md#navmegamenu-props"><code>NavMegamenuProps</code></a> (Optional)</td><td>Mega menu data, using the <code>NavMegamenuProps</code> interface for details.</td><td>Displays a mega menu when hovering or clicking on the nav item.</td></tr></tbody></table>

## NavMegamenu Props&#x20;

| Prop              | Type                                                                          | Description                                                               | Display as                                                        |
| ----------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| **type**          | `MegaMenuType`                                                                | Defines the type of the mega menu (e.g. MEGAMENU1, MEGAMENU2 etc.)        | Used to determine the menu's layout or variants.                  |
| **toggleBtn**     | `ButtonProps`                                                                 | MUI's `ButtonProps` defines the button that toggles the mega menu.        | A button that the user clicks to open the mega menu.              |
| **menuItems**     | Array of [`MenuItemsProps`](navmenu.md#menuitems-props)                       | An array of menu items, each described by the `MenuItemsProps` interface. | The items displayed within the mega menu (e.g., links, sections). |
| **footerData**    | `ReactElement \|` [`MenuFooterProps`](navmenu.md#menufooter-props) (Optional) |  Footer content for the menu, can be a React element or footer props.     | Footer section at the bottom of the mega menu.                    |
| **bannerData**    | `ReactElement` (Optional)                                                     | Banner content displayed within the menu.                                 | An banner displayed at the top or side of the mega menu.          |
| **popperOffset**  | `number` (Optional)                                                           | Vertical offset for the menu popper (dropdown positioning).               | Adjusts vertical positioning of the mega menu dropdown.           |
| **popperOffsetX** | `number` (Optional)                                                           | Horizontal offset for the menu popper.                                    | Adjusts horizontal positioning of the mega menu dropdown.         |
| **popperWidth**   | `number` (Optional)                                                           | Width for the mega menu popper (dropdown).                                | The width of the dropdown menu when opened.                       |

## MenuItems Props <a href="#menuitems-props" id="menuitems-props"></a>

| Prop          | Type                           | Description                                              | Display as                                                                                                                           |
| ------------- | ------------------------------ | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **icon**      | `SpriteIconProps` (Optional)   | Icon for the menu item.                                  | Icon shown next to the title (e.g., a small image or symbol).                                                                        |
| **title**     | `string`                       | The display title of the menu item.                      | Main text or label for the menu item (e.g., "Dashboard").                                                                            |
| **content**   | `string` (Optional)            | Additional content or description for the menu item.     | A description or additional information below the title.                                                                             |
| **selected**  | `boolean` (Optional)           | Whether this item is currently selected.                 | Indicates if the item is highlighted or in a "selected" state.                                                                       |
| **theme**     | `Themes` (Optional)            |  Theme-specific styling for the menu item.               | Changes appearance based on the current theme (e.g., AI, CRM).                                                                       |
| **image**     | `ImageCommonProps`  (Optional) | Image path or object with `light` and `dark` image path. | <p><code>"path-to-image.svg"</code><br> or <br><code>{ light: 'path-to-image-light.svg', dark: 'path-to-image-dark.svg' }</code></p> |
| **link**      | `LinkProps` (Optional)         | Link to the page the item navigates to.                  | A clickable link for this menu item.                                                                                                 |
| **status**    | `string` (Optional)            |  Status label or badge (e.g., "new", "beta").            | Displays a small status label next to the title.                                                                                     |
| **itemsList** | `MenuItemsProps[]` (Optional)  | Sub-menu or grouped items list.                          | A group or dropdown of related sub-items.                                                                                            |

## MenuFooter Props

| Prop      | Type               | Description                                           | Display as                                           |
| --------- | ------------------ | ----------------------------------------------------- | ---------------------------------------------------- |
| **title** | `string`           | The display title of the footer.                      | The footer section's title (e.g., "More Resources"). |
| **link**  | `ButtonProps`      | A button link in the footer that navigates somewhere. | A clickable button (e.g., "View All").               |
| **list**  | `MenuItemsProps[]` | A list of menu items to display in the footer.        | List of menu items within the footer section.        |

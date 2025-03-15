---
description: >-
  This guide provides an overview of how to use, manage, and customize the menu
  configuration in your project.
---

# Menu

The menu is configured at **`src/menu/index.tsx`**

Each menu item supports properties like `id`, `title`, `icon`, `url`, `type`, and `roles` for fine-grained control.

### Adding or Removing Menu Items

*   **Adding a New Menu Group**\
    1\. Create a new file (e.g., **`newGroup.tsx`**) in the same folder as `manage.tsx` and `other.tsx`.\
    2\. Define the menu group structure as a **`NavItemType`** object:\


    {% code title="src/menu/newGroup.tsx" %}
    ```typescript
    import { FormattedMessage } from 'react-intl';

    const newGroup: NavItemType = {
      id: 'group-new',
      title: <FormattedMessage id="newGroup" />,
      icon: 'IconNew',
      type: 'group',
      children: [
        {
          id: 'new-item',
          title: <FormattedMessage id="newItem" />,
          type: 'item',
          url: '/new-item',
          icon: 'IconLink'
        }
      ]
    };

    export default newGroup;
    ```
    {% endcode %}

    \
    3\. Import and add the new group in **`index.tsx`**:\
    &#x20;

    {% code title="src/menu/index.tsx" %}
    ```typescript
    import newGroup from './newGroup';

    const menuItems: { items: NavItemType[] } = {
      items: [manage, other, newGroup]
    };

    export default menuItems;
    ```
    {% endcode %}


*   **Removing an Existing Menu Group**\
    1\. Open **`index.tsx`**.\
    2\. Remove the corresponding group from the **`items`** array:\


    {% code title="src/menu/index.tsx" %}
    ```typescript
    const menuItems: { items: NavItemType[] } = {
      items: [manage] // Removed "other" menu group
    };
    ```
    {% endcode %}


*   **Adding a New Menu Item**\
    1\. Open the desired group file (e.g., `manage.tsx`).\
    2\. Add a new item to the **`children`** array:\


    ```typescript
    {
      id: 'reports',
      title: <FormattedMessage id="reports" />,
      type: 'item',
      url: '/reports',
      icon: 'IconReport'
    }
    ```


* **Removing a Menu Item**\
  1\. Open the desired group file.\
  2\. Remove the specific item from the **`children`** array.

### Changing Icons

To change an icon for a menu item:\
1\. Identify the **`icon`** property of the menu item.\
2\. Replace it with the desired icon name:

```typescript
icon: 'IconNewIcon'
```

\
Ensure the new icon exists in your icon library.

### Managing Roles

The **`roles`** property controls which user roles can access specific menu items. for more details refer [documentation of role guard](guards/role-guard.md).

*   **Adding Roles**\
    1\. Open the file where the menu item is defined.\
    2\. Add the desired roles to the **`roles`** array:\


    ```typescript
    roles: [AuthRole.ADMIN, AuthRole.USER]
    ```


*   **Removing Roles**\
    1\. Remove the role from the **`roles`** array\


    ```typescript
    roles: [AuthRole.ADMIN] // Removed AuthRole.USER
    ```


*   **Making a Menu Item Public**\
    To make a menu item accessible to all users, remove the **`roles`** property:\


    ```typescript
    {
      id: 'dashboard',
      title: <FormattedMessage id="dashboard" />,
      type: 'item',
      url: '/dashboard/analytics',
      icon: 'IconLayoutGrid'
      // No roles property here
    }
    ```

### Translation Keys

Menu titles use the **`FormattedMessage`** component for internationalization.\
\
Internationalization is set up in the **`src/utils/locales`** folder, which currently contains JSON files for four languages.\
\
1\. **`en.json`** English\
2\. **`fr.json`** French\
3\. **`ro.json`** Romanian\
4\. **`zh.json`** Chinese (Simplified)

*   **Adding a New Translation Key**\
    1\. Add the key to your translation files:\


    ```json
    {
      "newGroup": "New Group",
      "newItem": "New Item"
    }
    ```

    \
    2\. Use the key in the menu definition:\


    ```typescript
    title: <FormattedMessage id="newGroup" />
    ```

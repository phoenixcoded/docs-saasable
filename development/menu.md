---
description: >-
  This guide provides an overview of how to use, manage, and customize the menu
  configuration in your project.
---

# Menu

The menu is configured at **`src/menu/index.tsx`**

Each menu item supports properties like `id`, `title`, `icon`, `url`, `type`, and `roles` for fine-grained control.

### Adding or Removing Menu Items

* **Adding a New Menu Group**\
  1\. Create a new file (e.g., **`newGroup.tsx`**) in the same folder as `manage.tsx` and `other.tsx`.\
  2\. Define the menu group structure as a **`NavItemType`** object:

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript
const manage: NavItemType = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      id: 'dashboard',
      title: 'dashboard',
      type: 'item',
      url: '/dashboard/analytics/overview',
      icon: 'IconLayoutGrid'
    },
  ]
};

export default manage;
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript
const manage = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      id: 'dashboard',
      title: 'dashboard',
      type: 'item',
      url: '/dashboard/analytics/overview',
      icon: 'IconLayoutGrid'
    },
  ]
};

export default manage;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript
 const manage: NavItemType = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      id: 'dashboard',
      title: 'dashboard',
      type: 'item',
      url: '/dashboard/analytics',
      icon: 'IconLayoutGrid'
    },
  ]
};

export default manage;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript
const manage = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      id: 'dashboard',
      title: 'dashboard',
      type: 'item',
      url: '/dashboard/analytics',
      icon: 'IconLayoutGrid'
    }
  ]
};

export default manage;
```
{% endcode %}
{% endtab %}
{% endtabs %}

\
3\. Import and add the new group in **`index.tsx`**:

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src/menu/index.tsx"><code class="lang-typescript">import uiElements from './ui-elements';

const menuItems: { items: NavItemType[] } = {
<strong>  items: [manage, uiElements, pages, other]
</strong>};

export default menuItems;
</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-typescript" data-title="src/menu/index.jsx"><code class="lang-typescript">import uiElements from './ui-elements';
<strong>
</strong><strong>const menuItems = {
</strong>  items: [manage, uiElements, pages, other]
};

export default menuItems;
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/index.tsx" %}
```typescript
import uiElements from './ui-elements';

const menuItems: { items: NavItemType[] } = {
  items: [manage, uiElements, pages, other]
};

export default menuItems;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/index.jsx" %}
```typescript
import uiElements from './ui-elements';

const menuItems = {
  items: [manage, uiElements, pages, other]
};

export default menuItems;
```
{% endcode %}
{% endtab %}
{% endtabs %}



* **Removing an Existing Menu Group**\
  1\. Open **`index.tsx`**.\
  2\. Remove the corresponding group from the **`items`** array:

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src/menu/index.tsx"><code class="lang-typescript">import uiElements from './ui-elements';

const menuItems: { items: NavItemType[] } = {
<strong>  items: [manage] // Removed "other" menu group
</strong>};

export default menuItems;
</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-typescript" data-title="src/menu/index.jsx"><code class="lang-typescript">import uiElements from './ui-elements';

const menuItems = {
<strong>  items: [manage] // Removed "other" menu group
</strong>};

export default menuItems;import uiElements from './ui-elements';
</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/index.tsx" %}
```typescript
import uiElements from './ui-elements';

const menuItems: { items: NavItemType[] } = {
  items: [manage] // Removed "other" menu group
};

export default menuItems;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/index.jsx" %}
```typescript
import uiElements from './ui-elements';

const menuItems = {
  items: [manage]  // Removed "other" menu group
};

export default menuItems;
```
{% endcode %}
{% endtab %}
{% endtabs %}

* **Adding a New Menu Item**\
  1\. Open the desired group file (e.g., `manage.tsx`).\
  2\. Add a new item to the **`children`** array:

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript
 {
   id: 'dashboard',
   title: 'dashboard',
   type: 'item',
   url: '/dashboard/analytics',
   icon: 'IconLayoutGrid'
 },
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript
{
   id: 'dashboard',
   title: 'dashboard',
   type: 'item',
   url: '/dashboard/analytics',
   icon: 'IconLayoutGrid'
 },
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript
{
  id: 'dashboard',
  title: 'dashboard',
  type: 'item',
  url: '/dashboard/analytics',
  icon: 'IconLayoutGrid'
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript
{
  id: 'dashboard',
  title: 'dashboard',
  type: 'item',
  url: '/dashboard/analytics',
  icon: 'IconLayoutGrid'
}
```
{% endcode %}
{% endtab %}
{% endtabs %}



* **Removing a Menu Item**\
  1\. Open the desired group file.\
  2\. Remove the specific item from the **`children`** array.

### Changing Icons

To change an icon for a menu item:\
1\. Identify the **`icon`** property of the menu item.\
2\. Replace it with the desired icon name:

```typescript
icon: 'IconLayoutGrid'
```

\
Ensure the new icon exists in your icon library.

### Managing Roles

The **`roles`** property controls which user roles can access specific menu items. for more details refer [documentation of role guard](guards/role-guard.md).

*   **Adding Roles**\
    1\. Open the file where the menu item is defined.\
    2\. Add the desired roles to the **`roles`** array:\


    ```typescript
    roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN]
    ```


*   **Removing Roles**\
    1\. Remove the role from the **`roles`** array\


    ```typescript
    roles: [AuthRole.SUPER_ADMIN] // Removed AuthRole.USER
    ```


*   **Making a Menu Item Public**\
    To make a menu item accessible to all users, remove the **`roles`** property:\


    <pre class="language-typescript"><code class="lang-typescript"> {
       id: 'dashboard',
       title: 'dashboard',
       type: 'item',
       url: '/dashboard/analytics',
       icon: 'IconLayoutGrid'
       // No roles property here
    <strong> }
    </strong></code></pre>

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
      "dashboard": "Dashboard",
      "account": "Account"
    }
    ```

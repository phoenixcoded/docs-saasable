# Icons

Use the third-party library `@tabler/icons-react`. To view all available icons, visit the official site: [Tabler Icons Documentation](https://tabler.io/docs/icons/react).

### How to add icons in any files?

{% hint style="info" %}
**Note:** Ensure each icon you use is imported at the top of the file.
{% endhint %}

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src\components\Breadcrumbs.tsx"><code class="lang-typescript">// @assets
<strong>import { IconChevronRight } from '@tabler/icons-react';
</strong>
/***************************  BREADCRUMBS  ***************************/

export default function Breadcrumbs() {
 ...

  return (
    &#x3C;MuiBreadcrumbs aria-label="breadcrumb" separator={&#x3C;IconChevronRight size={16} />}>
      ...
    &#x3C;/MuiBreadcrumbs>
  );

</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src\components\Breadcrumbs.jsx" %}
```javascript
// @assets
import { IconChevronRight } from '@tabler/icons-react';

/***************************  BREADCRUMBS  ***************************/

export default function Breadcrumbs() {
 ...

  return (
    <MuiBreadcrumbs aria-label="breadcrumb" separator={<IconChevronRight size={16} />}>
      ...
    </MuiBreadcrumbs>
  );

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
<pre class="language-typescript" data-title="src\components\Breadcrumbs.tsx"><code class="lang-typescript">// @assets
<strong>import { IconChevronRight } from '@tabler/icons-react';
</strong>
/***************************  BREADCRUMBS  ***************************/

export default function Breadcrumbs() {
 ...

  return (
<strong>    &#x3C;MuiBreadcrumbs aria-label="breadcrumb" separator={&#x3C;IconChevronRight size={16} />}>
</strong>      ...
    &#x3C;/MuiBreadcrumbs>
  );

</code></pre>
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src\components\Breadcrumbs.jsx" %}
```javascript
// @assets
import { IconChevronRight } from '@tabler/icons-react';

/***************************  BREADCRUMBS  ***************************/

export default function Breadcrumbs() {
 ...

  return (
    <MuiBreadcrumbs aria-label="breadcrumb" separator={<IconChevronRight size={16} />}>
      ...
    </MuiBreadcrumbs>
  );

```
{% endcode %}
{% endtab %}
{% endtabs %}

### How to add dynamic icon?

Create a common component for rendering dynamic icons, named `DynamicIcon.tsx`, located in the folder path `src/components/`.&#x20;

#### Props Details

<table><thead><tr><th>Prop</th><th width="201">Type</th><th>Description</th></tr></thead><tbody><tr><td><strong>name</strong></td><td><code>keyof typeof TablerIcons</code></td><td>Use icon name from Tabler library e.g., <code>IconLayoutGrid</code></td></tr><tr><td><strong>size</strong></td><td><code>number</code> (Optional)</td><td>Sets the size of the icon. Pass a numeric value to adjust the icon's width and height proportionally.</td></tr><tr><td><strong>color</strong></td><td><code>string</code> (Optional)</td><td>Defines the color of the icon.</td></tr><tr><td><strong>stroke</strong></td><td><code>number</code> (Optional)</td><td>Sets the stroke width of the icon's lines. Adjust this value to make the lines thicker or thinner.</td></tr></tbody></table>

Add dynamic icon in menu (sidebar)

{% tabs %}
{% tab title="VITE(TS)" %}
<pre class="language-typescript" data-title="src/layouts/AdminLayout/Drawer/DrawerContent/MiniDrawer/NavItem.tsx"><code class="lang-typescript">interface Props {
  item: NavItemType;
  level?: number;
}

/***************************  MINI DRAWER - ITEM  ***************************/

export default function NavItem({ item, level = 0 }: Props) {
 ...

  return (
    ...
    
<strong>              &#x3C;DynamicIcon
</strong><strong>                name={item.icon as DynamicIconProps['name']}
</strong><strong>                size={22}
</strong><strong>                stroke={1.5}
</strong><strong>                color={isSelected ? theme.palette.text.primary : theme.palette.text.secondary}
</strong><strong>              />
</strong>           ...
      )}
      ...
    &#x3C;/ListItemButton>
  );
}

</code></pre>
{% endtab %}

{% tab title="VITE(JS)" %}
<pre class="language-typescript" data-title="src/layouts/AdminLayout/Drawer/DrawerContent/MiniDrawer/NavItem.jsx"><code class="lang-typescript">/***************************  MINI DRAWER - ITEM  ***************************/

export default function NavItem({ item, level = 0 }) {
 ...

  return (
    ...
    
<strong>              &#x3C;DynamicIcon
</strong><strong>                name={item.icon}
</strong><strong>                size={22}
</strong><strong>                stroke={1.5}
</strong><strong>                color={isSelected ? theme.palette.text.primary : theme.palette.text.secondary}
</strong><strong>              />
</strong>           ...
      )}
      ...
    &#x3C;/ListItemButton>
  );
}

</code></pre>
{% endtab %}

{% tab title="NEXT(TS)" %}
<pre class="language-typescript" data-title="src/layouts/AdminLayout/Drawer/DrawerContent/MiniDrawer/NavItem.tsx"><code class="lang-typescript">interface Props {
  item: NavItemType;
  level?: number;
}

/***************************  MINI DRAWER - ITEM  ***************************/

export default function NavItem({ item, level = 0 }: Props) {
 ...

  return (
    ...
    
<strong>              &#x3C;DynamicIcon
</strong><strong>                name={item.icon as DynamicIconProps['name']}
</strong><strong>                size={22}
</strong><strong>                stroke={1.5}
</strong><strong>                color={isSelected ? theme.palette.text.primary : theme.palette.text.secondary}
</strong><strong>              />
</strong>           ...
      )}
      ...
    &#x3C;/ListItemButton>
  );
}

</code></pre>
{% endtab %}

{% tab title="NEXT(JS)" %}
<pre class="language-javascript" data-title="src/layouts/AdminLayout/Drawer/DrawerContent/MiniDrawer/NavItem.jsx"><code class="lang-javascript">/***************************  MINI DRAWER - ITEM  ***************************/

export default function NavItem({ item, level = 0 }) {
 ...

  return (
    ...
    
<strong>              &#x3C;DynamicIcon
</strong><strong>                name={item.icon}
</strong><strong>                size={22}
</strong><strong>                stroke={1.5}
</strong><strong>                color={isSelected ? theme.palette.text.primary : theme.palette.text.secondary}
</strong><strong>              />
</strong>           ...
      )}
      ...
    &#x3C;/ListItemButton>
  );
}

</code></pre>
{% endtab %}
{% endtabs %}

Pass icon from menu list.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript

/***************************  MENU ITEMS - APPLICATIONS  ***************************/

const manage: NavItemType = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      ...,
      icon: 'IconLayoutGrid'
    },
    ...
  ]
};

export default manage;

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript

/***************************  MENU ITEMS - APPLICATIONS  ***************************/

const manage = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      ...,
      icon: 'IconLayoutGrid'
    },
    ...
  ]
};

export default manage;
7
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/manage.tsx" %}
```typescript

/***************************  MENU ITEMS - APPLICATIONS  ***************************/

const manage: NavItemType = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      ...,
      icon: 'IconLayoutGrid'
    },
    ...
  ]
};

export default manage;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/manage.jsx" %}
```typescript

/***************************  MENU ITEMS - APPLICATIONS  ***************************/

const manage = {
  id: 'group-manage',
  title: 'manage',
  icon: 'IconBrandAsana',
  type: 'group',
  children: [
    {
      ...,
      icon: 'IconLayoutGrid'
    },
    ...
  ]
};

export default manage;

```
{% endcode %}
{% endtab %}
{% endtabs %}

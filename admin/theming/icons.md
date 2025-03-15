# Icons

Use the third-party library `@tabler/icons-react`. To view all available icons, visit the official site: [Tabler Icons Documentation](https://tabler.io/docs/icons/react).

### How to add icons in any files ?

{% hint style="info" %}
**Note:** Ensure each icon you use is imported at the top of the file.
{% endhint %}

{% tabs %}
{% tab title="Breadcrumbs.tsx" %}
<pre class="language-typescript"><code class="lang-typescript">// @assets
<strong>import { IconChevronRight } from '@tabler/icons-react';
</strong>
/***************************  BREADCRUMBS  ***************************/

export default function Breadcrumbs({ data }: { data?: NavItemType[] }) {
 ...

  return (
<strong>    &#x3C;MuiBreadcrumbs aria-label="breadcrumb" separator={&#x3C;IconChevronRight size={16} />}>
</strong>      ...
    &#x3C;/MuiBreadcrumbs>
  );

</code></pre>
{% endtab %}
{% endtabs %}

### How to add dynamic icon ?

Create a common component for rendering dynamic icons, named `DynamicIcon.tsx`, located in the folder path `src/components/`.&#x20;

#### Props Details

<table><thead><tr><th>Prop</th><th width="201">Type</th><th>Description</th></tr></thead><tbody><tr><td><strong>name</strong></td><td><code>keyof typeof TablerIcons</code></td><td>Use icon name from Tabler library e.g., <code>IconLayoutGrid</code></td></tr><tr><td><strong>size</strong></td><td><code>number</code> (Optional)</td><td>Sets the size of the icon. Pass a numeric value to adjust the icon's width and height proportionally.</td></tr><tr><td><strong>color</strong></td><td><code>string</code> (Optional)</td><td>Defines the color of the icon.</td></tr><tr><td><strong>stroke</strong></td><td><code>number</code> (Optional)</td><td>Sets the stroke width of the icon's lines. Adjust this value to make the lines thicker or thinner.</td></tr></tbody></table>

Add dynamic icon in menu (sidebar)

{% tabs %}
{% tab title="src/layouts/AdminLayout/Drawer/DrawerContent/MiniDrawer/NavItem.tsx" %}
<pre class="language-typescript"><code class="lang-typescript">
/***************************  LIST ITEM BUTTON - STYLE  ***************************/


interface Props {
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
{% endtabs %}

Pass icon from menu list.

{% tabs %}
{% tab title="src/menu/manage/tsx" %}
<pre class="language-typescript"><code class="lang-typescript">
/***************************  MENU ITEMS - APPLICATIONS  ***************************/

const manage: NavItemType = {
  id: 'group-manage',
  title: &#x3C;FormattedMessage id="manage" />,
<strong>  icon: 'IconBrandAsana',
</strong>  type: 'group',
  children: [
    {
      ...,
<strong>      icon: 'IconLayoutGrid'
</strong>    },
    ...
  ]
};

export default manage;

</code></pre>
{% endtab %}
{% endtabs %}

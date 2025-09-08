# Role Guard

A **Role Guard** restricts access to specific pages based on the user's role, such as "admin" or "user". It ensures that only users with the appropriate permissions can view or interact with certain sections, enhancing security and access control. 🛡️👤

### Role-based page access

**Role guard** is configured at **`src/utils/route-guard/RoleGuard.tsx`**

To use it, just wrap the component with **RoleGuard**, as below.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/routes/MainRoutes.tsx" %}
```typescript
const MainRoutes = {
  path: '/',
  element: (
    <AuthProvider>
      <AuthGuard>
        <RoleGuard>
          <AdminLayout />
        </RoleGuard>
      </AuthGuard>
    </AuthProvider>
  )
  ...
};

export default MainRoutes;
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/MainRoutes.jsx" %}
```typescript
const MainRoutes = {
  path: '/',
  element: (
    <AuthProvider>
      <AuthGuard>
        <RoleGuard>
          <AdminLayout />
        </RoleGuard>
      </AuthGuard>
    </AuthProvider>
  )
  ...
};

export default MainRoutes;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/(admin)/layout.tsx" %}
```typescript
export default function Layout({ children }: ChildrenProps) {
  return (
    <AuthProvider>
      <AuthGuard>
        <RoleGuard>
          <AdminLayout>{children}</AdminLayout>
        </RoleGuard>
      </AuthGuard>
    </AuthProvider>
  );
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
<pre class="language-javascript" data-title="src/app/(admin)/layout.jsx"><code class="lang-javascript"><strong>export default function Layout({ children }) {
</strong>  return (
    &#x3C;AuthProvider>
      &#x3C;AuthGuard>
        &#x3C;RoleGuard>
          &#x3C;AdminLayout>{children}&#x3C;/AdminLayout>
        &#x3C;/RoleGuard>
      &#x3C;/AuthGuard>
    &#x3C;/AuthProvider>
  );
}

Layout.propTypes = { children: PropTypes.any };
</code></pre>
{% endtab %}
{% endtabs %}



### Role-based menu access

We have also implemented **role-based menu access**, ensuring that users see only the menu options relevant to their specific roles and permissions. To manage this, we utilise a key named **`roles`** Within the menu data, which contains an array of roles associated with each menu item.&#x20;

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/menu/ui-elements.tsx" %}
```typescript
const uiElements: NavItemType = {
  id: 'group-ui-elements',
  title: 'ui-elements',
  icon: 'IconDotsVertical',
  type: 'group',
  children: [
    {
      id: 'components',
      title: 'components',
      type: 'collapse',
      icon: 'IconAppWindow',
      roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN],
      children: [
        {
          id: 'avatar',
          title: 'avatar',
          type: 'item',
          url: '/data-display/avatar'
        },
        {
          id: 'button',
          title: 'button',
          type: 'item',
          url: '/inputs/button'
        },
      
      ]
    }
  ]
};


export default uiElements;
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/menu/ui-elements.jsx" %}
```typescript
const uiElements = {
  id: 'group-ui-elements',
  title: 'ui-elements',
  icon: 'IconDotsVertical',
  type: 'group',
  children: [
    {
      id: 'components',
      title: 'components',
      type: 'collapse',
      icon: 'IconAppWindow',
      roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN],
      children: [
        {
          id: 'avatar',
          title: 'avatar',
          type: 'item',
          url: '/data-display/avatar'
        },
        {
          id: 'button',
          title: 'button',
          type: 'item',
          url: '/inputs/button'
        },
      
      ]
    }
  ]
};


export default uiElements;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/menu/ui-elements.tsx" %}
```typescript
const uiElements: NavItemType = {
  id: 'group-ui-elements',
  title: 'ui-elements',
  icon: 'IconDotsVertical',
  type: 'group',
  children: [
    {
      id: 'components',
      title: 'components',
      type: 'collapse',
      icon: 'IconAppWindow',
      roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN],
      children: [
        {
          id: 'avatar',
          title: 'avatar',
          type: 'item',
          url: '/data-display/avatar'
        },
        {
          id: 'button',
          title: 'button',
          type: 'item',
          url: '/inputs/button'
        },
      ]
    }
  ]
};

export default uiElements;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/menu/ui-elements.jsx" %}
```typescript
const uiElements = {
  id: 'group-ui-elements',
  title: 'ui-elements',
  icon: 'IconDotsVertical',
  type: 'group',
  children: [
    {
      id: 'components',
      title: 'components',
      type: 'collapse',
      icon: 'IconAppWindow',
      roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN],
      children: [
        {
          id: 'avatar',
          title: 'avatar',
          type: 'item',
          url: '/data-display/avatar'
        },
        {
          id: 'button',
          title: 'button',
          type: 'item',
          url: '/inputs/button'
        }
      ]
    }
  ]
};

export default uiElements;

```
{% endcode %}
{% endtab %}
{% endtabs %}

**Menu access strategy :**

1. **Default Access**:\
   If no roles are assigned to a menu item, it is accessible to all users.
2. **Role-Specific Access**:\
   If roles are specified for a menu item, that item is only accessible to the designated roles.
3. **Parent-Child Role Requirement**:\
   If both parent and child menu items have assigned roles, the parent must include the specific role for any child item to be visible to that role.

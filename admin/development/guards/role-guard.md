# Role Guard

A **Role Guard** restricts access to specific pages based on the user's role, such as "admin" or "user". It ensures that only users with the appropriate permissions can view or interact with certain sections, enhancing security and access control. 🛡️👤

### Role based page access

**Role guard** is configured at **`src/utils/route-guard/RoleGuard.tsx`**

To use it just wrap component with **RoleGuard**, same as below.

{% code title="src/app/(admin)/layout.tsx" %}
```typescript
<AuthProvider>
    <AuthGuard>
        <RoleGuard>
            <AdminLayout>{children}</AdminLayout>
        </RoleGuard>
    </AuthGuard>
</AuthProvider>
```
{% endcode %}

### Role based menu access

We have also implemented **role-based menu access**, ensuring that users see only the menu options relevant to their specific roles and permissions. To manage this, we utilize a key named **`roles`** within the menu data, which contains an array of roles associated with each menu item.&#x20;

```

  {
      id: 'components',
      title: <FormattedMessage id="components" />,
      type: 'collapse',
      icon: 'IconAppWindow',
      roles: [AuthRole.SUPER_ADMIN, AuthRole.ADMIN],
      children: [
        {
          id: 'avatar',
          title: <FormattedMessage id="avatar" />,
          type: 'item',
          url: '/data-display/avatar'
        },
        {
          id: 'button',
          title: <FormattedMessage id="button" />,
          type: 'item',
          url: '/inputs/button'
        },
      ]
  }
```

**Menu access strategy :**

1. **Default Access**:\
   If no roles are assigned to a menu item, it is accessible to all users.
2. **Role-Specific Access**:\
   If roles are specified for a menu item, that item is only accessible to the designated roles.
3. **Parent-Child Role Requirement**:\
   If both parent and child menu items have assigned roles, the parent must include the specific role for any child item to be visible to that role.

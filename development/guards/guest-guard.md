# Guest Guard

A **Guest Guard** restricts access to certain pages for authenticated users, redirecting them away from areas like login or signup if they’re already logged in. Ideal for enhancing user flow and preventing redundant actions.\
\
**Guest guard** is configured at **`src/utils/route-guard/GuestGuard.tsx`**\
\
We have used it the same as follows:

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/routes/authRoutes.tsx" %}
```typescript
const AuthRoutes = {
  path: '/',
  element: (
    <GuestGuard>
      <AuthLayout />
    </GuestGuard>
 )
 ...
};

export default AuthRoutes;
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/authRoutes.jsx" %}
```typescript
const AuthRoutes = {
  path: '/',
  element: (
    <GuestGuard>
      <AuthLayout />
    </GuestGuard>
  )
  ...
}

export default AuthRoutes;
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/(auth)/layout.tsx" %}
```typescript
export default function Layout({ children }: ChildrenProps) {
  return (
    <GuestGuard>
      <AuthLayout>{children}</AuthLayout>
    </GuestGuard>
  );
}
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/(auth)/layout.jsx" %}
```javascript
export default function Layout({ children }) {
  return (
    <GuestGuard>
      <AuthLayout>{children}</AuthLayout>
    </GuestGuard>
  );
}

Layout.propTypes = { children: PropTypes.any };
```
{% endcode %}
{% endtab %}
{% endtabs %}

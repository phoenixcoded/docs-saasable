# Auth Guard

An **Auth Guard** protects specific pages by ensuring only authenticated users can access them.

Auth Guard is configured at **`src/utils/route-guard/AuthGuard.tsx`**\
\
To use it, just wrap the component with **AuthGuard**, as shown below

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/routes/MainRoutes.tsx" %}
```typescript
element: (
    <AuthProvider>
      <AuthGuard>
        <RoleGuard>
          <AdminLayout />
        </RoleGuard>
      </AuthGuard>
    </AuthProvider>
  ),
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/MainRoutes.jsx" %}
```typescript
element: (
    <AuthProvider>
      <AuthGuard>
        <RoleGuard>
          <AdminLayout />
        </RoleGuard>
      </AuthGuard>
    </AuthProvider>
  ),
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

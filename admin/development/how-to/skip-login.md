---
description: How to set Dashboards First page instead Login
---

# Skip Login

This section explains how to set the Dashboard page as the default starting page, skipping the Login page, for cases where it is not needed.

1. Open the file:  **`src\app\page.tsx`** and edit the code below.

**To:**&#x20;

{% tabs %}
{% tab title="Typescript" %}
{% code title="src\app\page.tsx" %}
```typescript
// @next
import dynamic from 'next/dynamic';
 
// @project
 const AuthLayout = dynamic(() => import('@/layouts/AuthLayout'));
 const AuthLogin = dynamic(() => import('@/views/auth/login'));
 
/***************************  MAIN - DEFAULT PAGE  ***************************/
 
export default function Home() {
  
   return (
     <AuthLayout>
       <AuthLogin />
     </AuthLayout>
   );
}
```
{% endcode %}
{% endtab %}

{% tab title="Javascript" %}
{% code title="src\app\page.jsx" %}
````javascript
// @next
import dynamic from 'next/dynamic';

// @project
const AuthLayout = dynamic(() => import('@/layouts/AuthLayout'));
const AuthLogin = dynamic(() => import('@/views/auth/login'));

/***************************  MAIN - DEFAULT PAGE  ***************************/

export default function Home() {
  return (
    <AuthLayout>
      <AuthLogin />
    </AuthLayout>
  );
}
```
````
{% endcode %}
{% endtab %}
{% endtabs %}

**From:**

{% tabs %}
{% tab title="Typescript" %}
{% code title="src\app\page.tsx" %}
```typescript
'use client';
 
// @next
import { useRouter } from 'next/navigation';
 
import { useEffect } from 'react';

/***************************  MAIN - DEFAULT PAGE  ***************************/
 
export default function Home() {
  const router = useRouter();
 
  useEffect(() => {
    router.replace('/dashboard/analytics/overview');
  }, [router]);
 
  return null;
  
}
```
{% endcode %}
{% endtab %}

{% tab title="Javascript" %}
{% code title="src\app\page.jsx" %}
```javascript
'use client';
 
// @next
import { useRouter } from 'next/navigation';
 
import { useEffect } from 'react';

/***************************  MAIN - DEFAULT PAGE  ***************************/
 
export default function Home() {
  const router = useRouter();
 
  useEffect(() => {
    router.replace('/dashboard/analytics/overview');
  }, [router]);
 
  return null;
  
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

2. Comment out the **`AuthGuard & RoleGuard`** wrapper for the routes. :

{% tabs %}
{% tab title="Typescript" %}
{% code title="src\app\(admin)\layout.tsx" %}
```typescript
// @next
import dynamic from 'next/dynamic';
 
// @types
import { ChildrenProps } from '@/types/root';
 
// @project
import { AuthProvider } from '@/contexts/AuthContext';
const AdminLayout = dynamic(() => import('@/layouts/AdminLayout'));
// const AuthGuard = dynamic(() => import('@/utils/route-guard/AuthGuard'));
// const RoleGuard = dynamic(() => import('@/utils/route-guard/RoleGuard'));
 
/***************************  LAYOUT - ADMIN  ***************************/
 
export default function Layout({ children }: ChildrenProps) {
  return (
    <AuthProvider>
      {/* <AuthGuard>
        <RoleGuard> */}
      <AdminLayout>{children}</AdminLayout>
      {/* </RoleGuard>
      </AuthGuard> */}
    </AuthProvider>
  );
}
```
{% endcode %}
{% endtab %}

{% tab title="Javascript" %}
<pre class="language-javascript" data-title="src\app\(admin)\layout.jsx"><code class="lang-javascript">
import PropTypes from 'prop-types';

<strong>// @next
</strong>import dynamic from 'next/dynamic';
 
// @project
import { AuthProvider } from '@/contexts/AuthContext';
const AdminLayout = dynamic(() => import('@/layouts/AdminLayout'));
// const AuthGuard = dynamic(() => import('@/utils/route-guard/AuthGuard'));
// const RoleGuard = dynamic(() => import('@/utils/route-guard/RoleGuard'));
 
/***************************  LAYOUT - ADMIN  ***************************/
 
export default function Layout({ children }) {
  return (
    &#x3C;AuthProvider>
      {/* &#x3C;AuthGuard>
        &#x3C;RoleGuard> */}
      &#x3C;AdminLayout>{children}&#x3C;/AdminLayout>
      {/* &#x3C;/RoleGuard>
      &#x3C;/AuthGuard> */}
    &#x3C;/AuthProvider>
  );
}

Layout.propTypes = { children: PropTypes.any };
</code></pre>
{% endtab %}
{% endtabs %}

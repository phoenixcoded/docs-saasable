---
description: How to set Dashboards First page instead Login
---

# Skip Login

This section explains how to set the Dashboard page as the default starting page, skipping the Login page, for cases where it is not needed.

1. Remove the file at **`src/routes/AuthRoutes.tsx`**
2. **Vite** : Open the file:  **`src/routes/index.tsx`** and edit the code below.
3. Next : Open the file:&#x20;**&#x20;`src/app/page.tsx`** and edit the code below.

**To:**&#x20;

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/routes/index.tsx" %}
```typescript
import { createBrowserRouter } from 'react-router-dom';

// @routes
import AuthRoutes from './AuthRoutes';
import MainRoutes from './MainRoutes';
import PagesRoutes from './PagesRoutes';

/***************************  ROUTING RENDER  ***************************/

const router = createBrowserRouter([AuthRoutes, MainRoutes, PagesRoutes], {
  basename: import.meta.env.VITE_APP_BASE_URL
});

export default router;

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/index.jsx" %}
```javascript
import { createBrowserRouter } from 'react-router-dom';

// @routes
import AuthRoutes from './AuthRoutes';
import MainRoutes from './MainRoutes';
import PagesRoutes from './PagesRoutes';

/***************************  ROUTING RENDER  ***************************/

const router = createBrowserRouter([AuthRoutes, MainRoutes, PagesRoutes], {
  basename: import.meta.env.VITE_APP_BASE_URL
});

export default router;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/page.tsx" %}
```typescript
// @next
import dynamic from 'next/dynamic';

// @project
import GuestGuard from '@/utils/route-guard/GuestGuard';

const AuthLayout = dynamic(() => import('@/layouts/AuthLayout'));
const AuthLogin = dynamic(() => import('@/views/auth/login'));

/***************************  MAIN - DEFAULT PAGE  ***************************/

export default function Home() {
  return (
    <GuestGuard>
      <AuthLayout>
        <AuthLogin />
      </AuthLayout>
    </GuestGuard>
  );
}

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/page.jsx" %}
```javascript
// @next
import dynamic from 'next/dynamic';

// @project
import GuestGuard from '@/utils/route-guard/GuestGuard';

const AuthLayout = dynamic(() => import('@/layouts/AuthLayout'));
const AuthLogin = dynamic(() => import('@/views/auth/login'));

/***************************  MAIN - DEFAULT PAGE  ***************************/

export default function Home() {
  return (
    <GuestGuard>
      <AuthLayout>
        <AuthLogin />
      </AuthLayout>
    </GuestGuard>
  );
}

```
{% endcode %}
{% endtab %}
{% endtabs %}

**From:**

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/routes/index.tsx" %}
```typescript
import { createBrowserRouter } from 'react-router-dom';

// @routes
import MainRoutes from './MainRoutes';
import PagesRoutes from './PagesRoutes';

/***************************  ROUTING RENDER  ***************************/

const router = createBrowserRouter([ MainRoutes, PagesRoutes], {
  basename: import.meta.env.VITE_APP_BASE_URL
});

export default router;

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/index.jsx" %}
```javascript
import { createBrowserRouter } from 'react-router-dom';

// @routes
import MainRoutes from './MainRoutes';
import PagesRoutes from './PagesRoutes';

/***************************  ROUTING RENDER  ***************************/

const router = createBrowserRouter([ MainRoutes, PagesRoutes], {
  basename: import.meta.env.VITE_APP_BASE_URL
});

export default router;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/page.tsx" %}
```typescript
'use client';

// @next
import { useRouter } from 'next/navigation';

import { useEffect } from 'react';

/***************************  ANALYTICS  ***************************/

export default function Analytics() {
  const router = useRouter();

  useEffect(() => {
    router.replace('/dashboard/analytics/overview');
  }, [router]);

  return null;
}

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/page.jsx" %}
```javascript
'use client';

// @next
import { useRouter } from 'next/navigation';

import { useEffect } from 'react';

/***************************  ANALYTICS  ***************************/

export default function Analytics() {
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
{% tab title="VITE(TS)" %}
{% code title="src/routes/MainRoutes.tsx" %}
```typescript
import { lazy } from 'react';
import { Navigate } from 'react-router-dom';

// @project
import Loadable from '@/components/Loadable';
import { AuthProvider } from '@/contexts/AuthContext';
import AdminLayout from '@/layouts/AdminLayout';
// import AuthGuard from '@/utils/route-guard/AuthGuard';
// import RoleGuard from '@/utils/route-guard/RoleGuard';


const MainRoutes = {
  path: '/',
  element: (
    <AuthProvider>
      {/* <AuthGuard> */}
      {/* <RoleGuard> */}
      <AdminLayout />
      {/* </RoleGuard> */}
      {/* </AuthGuard> */}
    </AuthProvider>
  ),
   children: [
   ...
  ]
};

export default MainRoutes;

```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/routes/MainRoutes.jsx" %}
```javascript
import { lazy } from 'react';
import { Navigate } from 'react-router-dom';

// @project
import Loadable from '@/components/Loadable';
import { AuthProvider } from '@/contexts/AuthContext';
import AdminLayout from '@/layouts/AdminLayout';
// import AuthGuard from '@/utils/route-guard/AuthGuard';
// import RoleGuard from '@/utils/route-guard/RoleGuard';


const MainRoutes = {
  path: '/',
  element: (
    <AuthProvider>
      {/* <AuthGuard> */}
      {/* <RoleGuard> */}
      <AdminLayout />
      {/* </RoleGuard> */}
      {/* </AuthGuard> */}
    </AuthProvider>
  ),
   children: [
   ...
  ]
};

export default MainRoutes;

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
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

{% tab title="NEXT(JS)" %}
{% code title="src\app\(admin)\layout.jsx" %}
```javascript
import PropTypes from 'prop-types';
// @next
import dynamic from 'next/dynamic';

// @project
import { AuthProvider } from '@/contexts/AuthContext';
const AdminLayout = dynamic(() => import('@/layouts/AdminLayout'));
// const AuthGuard = dynamic(() => import('@/utils/route-guard/AuthGuard'));
// const RoleGuard = dynamic(() => import('@/utils/route-guard/RoleGuard'));

/***************************  LAYOUT - ADMIN  ***************************/

export default function Layout({ children }) {
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

Layout.propTypes = { children: PropTypes.any };

```
{% endcode %}
{% endtab %}
{% endtabs %}
